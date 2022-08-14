# pistachio-on-vss

[![Deploy vss site to Pages](https://github.com/pistachiostudio/pistachio-on-vss/actions/workflows/pages.yml/badge.svg)](https://github.com/pistachiostudio/pistachio-on-vss/actions/workflows/pages.yml)

testing for pistachiostudio.net on vss static site generator

[https://dev.pistachiostudio.net/](https://dev.pistachiostudio.net/)

## vss

https://github.com/zztkm/vss

## Deploy

build
```
./vss build
```

Copy static files
```
cp -r js css dist
cp favicon.ico manifest* manifest.json CNAME apple-touch-icon.png dist 
rm -rf README.md
```

```
python3 -m venv venv
source venv/bin/activate

pip install -r requirements.txt 
```

```
ghpages dist
```
