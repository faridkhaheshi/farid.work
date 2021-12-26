# farid.work
This is the personal website of Farid Khaheshi

## Setting up the required credentials

Add a `.credentials/farid.work-ssl/` directoty with the following files:

1. `cloudflare-ca-cert.crt`: The origin CA certificate of cloudflare,
2. `farid.work-origin-cert.pem`: The SSL certificate from cloudflare,
3. `farid.work-private-key.pem`: The private key used to create the SSL certificate.

Also make sure that the SSL/TLS encryption mode is set to full on Cloudflare.

Also add a `.env` file with the information for setting up the wordpress. Use the `.env.example` file as an example.

## Running the server:

Go to the project directory and run `docker-compose up -d`.
