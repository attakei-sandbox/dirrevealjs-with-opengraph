# Reproduction project

## Reproduction

```console
pip install -r requirements.txt
make html dirhtml revealjs dirrevealjs
```

## Result

`og:url` patterns

| builder      | index.rst   | sample.rst   |       | 
| ------------ | ----------- | ------------ | ----- |
| html         | /index.html | /sample.html | Right |
| dirhtml      | /           | /sample/     | Right |
| revealjs     | index.html  | /sample.html | Right |
| dirrevealjs  | /           | /sample.html | Wrong |
