# Docker Build

The generic TeX Live image does not include all fonts required by Awesome-CV. The project Dockerfile installs Roboto and Source Sans 3 before compiling the example documents.

From the repository root, build the image:

```bash
docker build --pull -f docker/Dockerfile -t awesome-cv .
```

Then mount the repository at `/doc` and run the image:

```bash
docker run --rm -v /absolute/path/to/Awesome-CV:/doc awesome-cv
```

The image uses the repository Makefile as its default command. A specific target can be appended, for example `resume.pdf`.
