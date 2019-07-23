# Customization

## Grub (thèmes)

Pour donner un loog un peu plus sympa à grub, on install le thème

```shell
trizen -S grub-themes-vimix
```

Et on le configure via l'application `grub-customizer`

## Thèmes et icones

On ajoute quelques thèmes GTK et icones

```shell
trizen -S numix-gtk-theme arc-{gtk-theme,icon-theme,solid-gtk-theme}
```

## Widgets

Pour ceux qui aiment les beaux widgets sur leur bureau

```shell
trizen -S conky-manager conky
```

## Wallpapers

### Nitrogen

Ce utilitaire permet de configurer des wallpapers différents en configuration multi-écran OU de configurer un wallpaper couvrant l'ensemble de ceux-ci.

Malheureusement, le prix à payer est la désactivation des icones sur le bureau.

On install nitrogen

```shell
trizen -S nitrogen
```

On l'ajoute dans les applications à démarrer lors de la session (Panneau de configuration), avec cette commande :

```shell
sh -c "sleep 5; nitrogen --restore"
```

Et on désactive la gestion des icones du bureau par Caja (MATE)

```shell
gsettings set org.mate.background draw-background false
gsettings set org.mate.background show-desktop-icons false
```

## Docks

### Plank

Dock léger et bien fini en provenance de ElementaryOS.

```shell
trizen -S plank
```

### Docky

Autre Dock léger et bien fini.

```shell
trizen -S docky
```