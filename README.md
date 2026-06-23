# Minishell

Projet **minishell** réalisé dans le cadre de l'école **42**, en collaboration avec **maximevanvelthoven**.

## Description

Minishell est une implémentation simplifiée d'un shell Unix.  
Le programme lit une commande, la parse, construit un AST, puis exécute les commandes avec gestion des redirections, pipes et builtins.

## Fonctionnalités

- Prompt interactif avec `readline`
- Gestion des quotes et de l'expansion des variables d'environnement
- Exécution de commandes externes
- Builtins implémentés :
  - `echo`
  - `cd`
  - `pwd`
  - `export`
  - `unset`
  - `env`
  - `exit`
- Redirections :
  - `>`
  - `>>`
  - `<`
  - `<<` (heredoc)
- Pipes (`|`)
- Gestion de signaux de base

## Compilation

Depuis la racine du dépôt :

```bash
make
```

Le projet dépend de la bibliothèque **readline** (headers et lib).

## Lancer le shell

```bash
./minishell
```

## Nettoyage

```bash
make clean
make fclean
make re
```