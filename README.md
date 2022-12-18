# Reproduction project

## Reproduction

### Actually

```console
pip install -r requirements.txt
make clean html dirhtml revealjs dirrevealjs
```

### Expects

```console
pip install -r requirements.txt
pip install git+https://github.com/attakei/sphinxext-opengraph@support-dirhtml-extends
make clean html dirhtml revealjs dirrevealjs
```

## Result

`og:url` patterns

| builder      | index.rst   | sample.rst   |       | 
| ------------ | ----------- | ------------ | ----- |
| html         | /index.html | /sample.html | Right |
| dirhtml      | /           | /sample/     | Right |
| revealjs     | /index.html | /sample.html | Right |
| dirrevealjs  | /index.html | /sample.html | Wrong |
