# Zeal Packaging: Flatpak

This contains a prototype packaging source for Zeal.

### Quick Start
#### Build Requirements
```sh
flatpak install flathub org.flatpak.Builder
alias flatpak-builder=org.flatpak.Builder
```

#### Dependencies
```sh
flatpak install flathub org.kde.Sdk//5.10
flatpak install flathub org.kde.Platform//5.10
```

#### Build & Install
```sh
flatpak-builder --force-clean --user --install zeal org.zealdocs.Zeal.json
```
