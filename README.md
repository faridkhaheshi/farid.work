# farid.work
This is the web server for farid.work.

## Setting up the required credentials

You have to enter two pieces of information regarding the SSL certificates required on any domain:
1. add a `.env` file with the template provided in `.env.example`. You should specify an email address that will be used for generating the SSL certificates using *certbot*. 
2. Add the list of all subdomains for which you need SSL certificates under the `supported_domains` folder. You should add one file for every primary domain name. Each file should include a list of all subdomains. Here, I have included the file for `rooster.farid.work`.


## Running the server:

Go to the project directory and run `docker-compose up -d`. It will take few seconds the first time because it will generate the ssl certificates.


## Restarting nginx

Just send a HUP signal to the container by running `docker kill --signal=HUP nginx`
