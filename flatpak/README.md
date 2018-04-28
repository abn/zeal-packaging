# Zeal Packaging: Flatpak

This contains a prototype packaging source for Zeal.

### Quick Start
#### Build Requirements
```sh
flatpak install flathub org.flatpak.Builder
alias flatpak-builder=org.flatpak.Builder
```

#### Prepare Repository
```sh
flatpak --user remote-add --no-gpg-verify --if-not-exists zealdocs zealdocs
```

#### Dependencies
```sh
flatpak install flathub org.kde.Sdk//5.10
flatpak install flathub org.kde.Platform//5.10
```

#### Build
```sh
flatpak-builder --repo=zealdocs zeal org.zealdocs.Zeal.json --force-clean
```

#### Install
```sh
flatpak --user install zealdocs org.zealdocs.Zeal
```
