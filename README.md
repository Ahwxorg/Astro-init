# Astro-init

> Since I do these steps every single time, I decided to make a repository that I can easily clone instead of wasting time.

## Stack consists of:

* [Astro](https://astro.build), of course...
* [TailwindCSS](https://tailwindcss.com/)

## Getting started

* Edit `/src/config.ts`, fill in your information
* Run `yarn astro dev`
* Navigate to 'http://localhost:4321' using your browser
* Enjoy!

## Deployment:

* Use `Yarn`
  * yarn.lock

* Use `Docker`
  * Dockerfile
  * Building Docker images using GitHub Actions

## See example:

```sh
mkdir astro-init
cd astro-init
cat <<EOF | tee docker-compose.yml
version: "3"
services:
  astro-init-example: # Container name
    ports:
      - 4321:8080 # Change the first number to any port you like
    image: ghcr.io/ahwxorg/astro-init # Change to your repository
EOF
docker compose up -d
```
