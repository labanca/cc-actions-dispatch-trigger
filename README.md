# cc-dispatch-trigger

[![Updated](https://github.com/splor-mg/cc-dispatch-trigger/actions/workflows/all.yaml/badge.svg)](https://github.com/splor-mg/cc-dispatch-trigger/actions/)

## Pré-requisitos

Esse projeto utiliza Docker para gerenciamento das dependências. Para fazer _build_  da imagem execute:

```bash
docker build --tag cc-dispatch-trigger .
```

## Uso

Para executar o container

```bash
docker run -it --rm --mount type=bind,source=$(PWD),target=/project cc-dispatch-trigger bash
```

Uma vez dentro do container execute os comandos do make

```bash
make all
```

_Gerado a partir de [cookiecutter-datapackage@3e5db85](https://github.com/splor-mg/cookiecutter-datapackage/commit/3e5db856ba8a4ba4c5a157ed8a0357ebea4f24ce)_
