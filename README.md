# Bootloader Tutorial - STM32

Ce projet est un tutoriel de bootloader pour STM32. Il montre comment démarrer le microcontrôleur avec un bootloader, faire clignoter une LED, puis sauter vers une application utilisateur.

## Fonctionnement

1. Au démarrage, le bootloader fait clignoter une LED.
2. Il vérifie si une application valide est présente.
3. Il saute vers cette application si elle est trouvée.

## Structure du projet

- `/Bootloader/` : code du bootloader
- `/Application/` : code de l'application utilisateur
- `linker_boot.ld` : script de liaison pour le bootloader
- `linker_app.ld` : script de liaison pour l'application

## Compilation

Utiliser Makefile, STM32CubeIDE ou autre outil selon votre configuration.

## Flash

```bash
st-flash write bootloader.bin 0x08000000
st-flash write application.bin 0x08004000

3. **Ajoute et commit le fichier** :

```bash
git add README.md
git commit -m "Update README with project description"
"# Bootloader-toturail" 
