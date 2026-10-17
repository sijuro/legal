# Legal

Páginas legales públicas (Terms of Service y Privacy Policy) para la app de
TikTok **tk-clip**, publicadas con GitHub Pages.

- Terms of Service: `tos.html`
- Privacy Policy: `privacy.html`

## Publicar

1. Crea un repositorio **público** llamado `legal` en tu cuenta:
   <https://github.com/new> → owner `sijuro`, nombre `legal`, visibilidad **Public**.
2. Sube estos ficheros:
   ```bash
   cd /home/simon/git/legal
   git remote add origin git@github.com:sijuro/legal.git
   git push -u origin main
   ```
3. Activa Pages: repo → **Settings → Pages** → *Build and deployment* →
   Source **Deploy from a branch** → Branch **main** / **/(root)** → Save.
4. En un minuto estarán disponibles:
   - <https://sijuro.github.io/legal/tos.html>
   - <https://sijuro.github.io/legal/privacy.html>
   - <https://sijuro.github.io/legal/>

## Verificar las URLs en TikTok

En la app de TikTok for Developers → **URL properties → Verify properties**:

- Usa verificación por **URL prefix** con `https://sijuro.github.io/legal/`.
- TikTok te dará un fichero de firma: descárgalo y déjalo en la **raíz de este
  repo** (queda servido en `https://sijuro.github.io/legal/<fichero>`), haz
  commit y push, y pulsa **Verify**.

Rellena así los campos de la app:

| Campo                 | Valor                                          |
| --------------------- | ---------------------------------------------- |
| Terms of Service URL  | `https://sijuro.github.io/legal/tos.html`      |
| Privacy Policy URL    | `https://sijuro.github.io/legal/privacy.html`  |
| Web / Desktop URL     | `https://sijuro.github.io/legal/`              |

> Estos textos son una plantilla razonable para una herramienta personal, no
> asesoramiento legal. Revísalos antes de la auditoría de TikTok.
