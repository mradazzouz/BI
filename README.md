
# BMEVIAUAC01 Data-driven systems

![Build docs](https://github.com/bmeviauac01/datadriven/workflows/Build%20docs/badge.svg?branch=master)

[BMEVIAUAC01 Data-driven systems](https://www.aut.bme.hu/Course/ENVIAUAC01/) course lecture notes, seminar materials and homework exercises.

The content in built using MkDocs and is published to GitHub Pages at: <https://bmeviauac01.github.io/datadriven/en/>

## Render website (with Docker)

You need Docker in order to build and run the documentation. On a local machine with Windows [Docker Desktop](https://www.docker.com/products/docker-desktop/) could be the right tooling or you could use any cloud based development environment like GitHub Codespaces.

This repository contains a Dockerfile which need to be built and run.

1. Open a terminal on the repository's root.
2. Run the following commands on Windows (PowerShell), Linux or MacOS:

   ```cmd
   docker build -t mkdocs .
   docker run -it --rm -p 8000:8000 -v ${PWD}:/docs mkdocs --config-file=mkdocs.en.yml
   ```

3. Open <http://localhost:8000> or codespace's port forwarded address in a browser.
4. Edit Markdown files. After saving any file the webpage should refresh automatically.
