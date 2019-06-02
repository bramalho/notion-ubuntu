# Notion
> Notion web app for Ubuntu

## Set up
```bash
ln -s -r app snap/app
```
```bash
docker pull snapcore/snapcraft
```

## Build
```bash
cd snap
```
```bash
docker run --rm -v "$PWD":/build -w /build snapcore/snapcraft bash \
      -c "apt update && snapcraft"
```

## Install
```bash
snap install --dangerous notion_1.0.0_amd64.snap
```

## Run
```bash
notion
```
