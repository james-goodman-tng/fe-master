# World Clock Dashboard - Master Frontend

Master frontend that embeds all five city clock components as iframes.

## Architecture

This master frontend loads the following components:
- Tokyo Clock (http://localhost:8081)
- London Clock (http://localhost:8082)
- New York Clock (http://localhost:8083)
- Sydney Clock (http://localhost:8084)
- Mumbai Clock (http://localhost:8085)

Each component is served from its own independent repository and container.

## Running Locally

Open `index.html` in a browser (requires all 5 frontend components to be running).

## Running with Docker

```bash
docker build -t fe-master .
docker run -p 8080:80 fe-master
```