# Saleor Docker Compose example for Production Environment

To install Saleor in a Production Environment, there are no instruction from the official website.

There is a community repository [Deploy Saleor](https://github.com/thewhiterabbit/Deploy_Saleor) for production deployment but it is obsoleted and not work now.

There is also an official repository [saleor-platform](https://github.com/saleor/saleor-platform.git) which use Docker Compose and recommended by Official, however, it is designed for development only.

Hence, I tried to create a docker-compose of Saleor for <https://foobar.store>.

Unluckily, there is a bit buggy (such as cannot create order) after the deployment with my own server.

So, I have already switched to another system. You may try it yourself if you would like to use Saleor.

## Requirements 
- Docker
- Docker Compose
- Reverse Proxy (Optional but recommended)

## How to use?
1. Put your own RSA Private Key in `private_key.env` (**Keep the double quote**)
2. Put your RSA Private Key Passphrase in `key_passphrase.env` if your key require a password
3. Change the settings (ports, volumes, environment configs) in the `docker-compose.yml`
4. `docker compose up -d` to deploy the containers in background