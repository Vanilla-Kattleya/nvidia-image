# Vanilla OS Nvidia Image

Containerfile for building a Vanilla OS Plasma+Nvidia image.

This image is based on top of [Plasma Image](https://github.com/Vanilla-Kattleya/plasma-image/pkgs/container/plasma) and offers the Vanilla OS Desktop experience with KDE Plasma and Nvidia drivers.

## Build

> [!NOTE]
> The fsguard compiled plugin `.so` file should be downloaded from the [latest release](https://github.com/Vanilla-OS/vib-fsguard/releases/latest) and be placed under a `plugins` directory beside the `recipe.yml` file.

```bash
vib build recipe.yml
podman image build -t nvidia .
```
