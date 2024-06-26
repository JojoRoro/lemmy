#Documentation Devcontainer

##Setup

This Project can be opened in a Devcontainer by using the button bellow.

[![Open in Dev Container](https://img.shields.io/badge/devcontainer-open-blue?logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/JojoRoro/lemmy)


Before running the application you must create a .env file in  the project root according to the env-schema.txt file, also in the root.
Please fill it out accordingly.

##Structure of the DevContainer

This DevCOntainer is based on the image mcr.microsoft.com/devcontainers/rust:1-1-bullseye as the project is in Rust.

There are some Plugins included in the base image, which are helpful to the development of this project. I have also included the Plugins Code Spell checker and Github copilot, as I find them useful and they are recommended on the internet.

Sadly I took a bad project for this Module. I like Lemmy as an Open Source Project, but it was far to complex to do as the LB in this Module.

The Project includes a dockerfile and a docker compose file in the ./docker directory, which can be used to build the project. In the Subfolder ./docker/federation there are further files to start multiple instances of the project with different properties ( some defederated, some not etc.).
