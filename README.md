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
