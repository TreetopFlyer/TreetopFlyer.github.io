

// up here accellerations are reset

for (int i = 0; i < n; ++i)
{
    const float rhoi = rho[i];
    for (int j = i+1; j < n; ++j)
    {
        float dx = x[2*i+0]-x[2*j+0];
        float dy = x[2*i+1]-x[2*j+1];
        float r2 = dx*dx + dy*dy;


        if (r2 < h2)
        {
            const float rhoj = rho[j];

            float q = sqrt(r2)/h; ////////// distance as a percent of particle radius
            float u = 1-q; ///////////////// inverse distance

            float w0 = C0 * u/rhoi/rhoj;
            float wp = w0 * Cp * (rhoi+rhoj-2*rho0) * u/q;
            float wv = w0 * Cv;

            float dvx = v[2*i+0]-v[2*j+0]; 
            float dvy = v[2*i+1]-v[2*j+1];


            // weighted difference in position plus weighted difference in velocity
            // is added to the ith particle's accelleration and subtracted from the jth particle's accelleration
            // (becomes a force between the particles)
            a[2*i+0] += (wp*dx + wv*dvx);
            a[2*i+1] += (wp*dy + wv*dvy);
            a[2*j+0] -= (wp*dx + wv*dvx);
            a[2*j+1] -= (wp*dy + wv*dvy);
        }
    }
}