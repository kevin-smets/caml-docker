# CAML

caml-docker provides an easy way to cascade YAML files. More info can be found on the [CAML Github page](https://github.com/kevin-smets/caml).

## Quick example

Directory structure:

```
.
├── a.yml
└── b.yml
```

Run:

```bash
docker build . -t caml
docker run --rm -ti -v ${PWD}:/code caml -f a b -j config.json -y config.yml
```
