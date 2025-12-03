# Benchmark des langages de script : Bash, PowerShell, Python
> Comparer 3 langages de scripts : Bash, PowerShell, Python, avec leurs avantages, limites, cas d’usage et un petit exemple.

🐧 1. Bash

✔️ Points forts

- Natif sur Linux/macOS

- Simple pour les tâches système

- Léger et rapide

- Idéal DevOps / CI/CD

❌ Points faibles

- Complexe pour les gros scripts

- Peu adapté à Windows

- Moins lisible que Python

🎯 Cas d’usage

- Automatisation Linux

- Déploiement

- Scripts système

🧩 Exemple

```
#!/bin/bash
A=$1
B=$2

echo "Addition : $((A + B))"
echo "Soustraction : $((A - B))"
echo "Multiplication : $((A * B))"
echo "Division : $((A / B))"
```

🪟 2. PowerShell

✔️ Points forts

- Parfait Windows et AD

- Très puissant pour systèmes Microsoft

- Manipulation d’objets native

- Multi-plateforme

❌ Points faibles

- Verbeux

- Plus lent

- Moins utilisé Linux

🎯 Cas d’usage

- Administration Windows

- Automatisation AD/GPO

- Scripts système avancés

🧩 Exemple

```
param($A, $B)

Write-Output "Addition : $($A + $B)"
Write-Output "Soustraction : $($A - $B)"
Write-Output "Multiplication : $($A * $B)"
Write-Output "Division : $($A / $B)"
```

🐍 3. Python

✔️ Points forts

- Simple et lisible

- Fonctionne partout

- Puissant (automation, data, web, IA)

- Beaucoup de modules

❌ Points faibles

- Plus lent

- Installation nécessaire

- Gestion des dépendances

🎯 Cas d’usage

- Automation avancée

- Dev (API, scripts)

- Gestion cloud

- Machine learning

🧩 Exemple

```
import sys

A = int(sys.argv[1])
B = int(sys.argv[2])

print("Addition :", A + B)
print("Soustraction :", A - B)
print("Multiplication :", A * B)
print("Division :", A / B)
```

🏁 Conclusion

| Langage        | Points forts         | Cas d’usage              |
| -------------- | -------------------- | ------------------------ |
| **Bash**       | Léger, Linux natif   | Automatisation Linux     |
| **PowerShell** | Parfait Windows + AD | Admin systèmes Microsoft |
| **Python**     | Polyvalent           | Automation, IA, scripts  |

🧪 Fonctionnement du projet

Ce projet contient trois scripts d’opérations mathématiques écrits en Bash, PowerShell et Python.
Chaque script exécute :

- une addition

- une soustraction

- une multiplication

- une division

L’objectif est de comparer les langages en théorie (benchmark) et en pratique (scripts) tout en apprenant un workflow Git complet.

🧱 Structure du projet
```
initiation-git/
│── README.md        → Documentation du projet
│── script.sh        → Script Bash
│── script.ps1       → Script PowerShell
└── script.py        → Script Python
```


Chaque fichier représente une implémentation du même exercice dans un langage différent.

🔧 Exécution des scripts

▶️ Bash
`
bash script.sh 10 5
`

▶️ PowerShell
`
pwsh ./script.ps1 -A 10 -B 5
`

▶️ Python
`
python script.py 10 5
`

## Workflow Git utilisé pour créer ce projet

> Ce projet a été réalisé en appliquant un workflow Git moderne, proche des pratiques DevOps.

1️⃣ Création d’une branche par script

Chaque langage a été développé dans sa propre branche :

- `feat/script_bash`

- `feat/script_pwsh`

- `feat/script_python`

Cela permet de travailler proprement sans toucher à **main**.

2️⃣ Développement du script dans la branche

Exemples :
```
touch script.sh
code script.sh
```

Écriture du code → sauvegarde.

3️⃣ Ajout et commit des changements
```
git add script.sh
git commit -m "feat: ajout script Bash"
```

Chaque commit est clair et décrit une action précise.

4️⃣ Push de la branche vers GitHub
```
git push -u origin feat/script_bash
```

GitHub crée automatiquement la branche distante.

5️⃣ Création d’une Pull Request (PR)

Depuis VSCode ou GitHub :

- comparaison entre la branche et **main**

- review du code

- validation

Tu as utilisé des titres tels que :

- feat: ajout script Bash

- feat: ajout script PowerShell

- feat: ajout script Python

6️⃣ Merge de la PR dans main

Tu as choisi la méthode :

✔️ Create Merge Commit

Cela permet de garder un historique clair :

- 1 commit = 1 fonctionnalité ajoutée

- historique lisible sur main

7️⃣ Suppression des branches (optionnel)

Après chaque merge, il est conseillé de supprimer la branche pour garder un repo propre.

🧠 Résumé visuel du workflow Git
```
(main) 
   │
   ├──→ (feat/script_bash) ---- PR #1 ----→ merge ----→ main
   ├──→ (feat/script_pwsh) ---- PR #2 ----→ merge ----→ main
   └──→ (feat/script_python) -- PR #3 ----→ merge ----→ main
```
🎓 Ce que ce projet t’a appris

✔️ Gérer un projet Git complet

✔️ Créer et utiliser des branches fonctionnelles

✔️ Rédiger des commits propres et cohérents

✔️ Faire des Pull Requests et les fusionner

✔️ Écrire des scripts simples dans trois langages

✔️ Comparer les langages via un benchmark théorique + pratique