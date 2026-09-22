# Plan de Formation — IA Générative & Copilot Microsoft 365

Page web du plan de formation professionnelle **NT Digital Conseil**
(réf. NTDC-IA-COPILOT-2026, v2.0) : 2 jours / 14h, acculturation IA générative,
prompt engineering (TCREI, OPRO) et maîtrise de Copilot Microsoft 365.

## Contenu

- `index.html` — page complète autonome (HTML + CSS inline, polices Google Fonts).

## Publier la page (GitHub Pages)

`index.html` est à la racine, la page est donc directement publiable :

1. **Settings → Pages** du dépôt
2. **Source** : `Deploy from a branch`
3. **Branch** : sélectionner la branche puis `/ (root)` → **Save**

L'URL par défaut est : `https://soleilbms.github.io/testhml/`

## Domaine personnalisé

Le fichier `CNAME` déclare le domaine **copilot-facile.fr**. Pour qu'il
fonctionne, le domaine doit être acheté et les enregistrements DNS suivants
créés chez le registrar :

| Type    | Nom   | Valeur              |
|---------|-------|---------------------|
| `A`     | `@`   | `185.199.108.153`   |
| `A`     | `@`   | `185.199.109.153`   |
| `A`     | `@`   | `185.199.110.153`   |
| `A`     | `@`   | `185.199.111.153`   |
| `CNAME` | `www` | `soleilbms.github.io.` |

Puis, dans **Settings → Pages**, cocher **Enforce HTTPS** une fois le
certificat émis (quelques minutes à 24h après la propagation DNS).

Pour changer de domaine, modifier `CNAME` (une seule ligne, sans `https://`)
et ajuster les DNS en conséquence.

## Aperçu local

Ouvrir `index.html` dans un navigateur, ou :

```bash
python3 -m http.server 8000
# puis http://localhost:8000
```
