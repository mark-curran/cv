# cv

Files that format and host my CV and blog.

## Local Site

This repo includes a [devcontainer specification](https://code.visualstudio.com/docs/devcontainers/containers) that can be run using the [VSCode Remote Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) or by simply running the `local` service in the `devcontainer/docker-compose.yml` file.

Start the docker container with port 4000 forwarded to a port on the localhost. Inside the docker contianer navigate to the `/docs` directory and run the following command to start hosting the site

```bash
bundle install && bundle exec jekyll serve
```

Open `http://localhost:XXXX` in a webbrowser where `XXXX` is the port on the localhost that is receiving traffic from the container.
