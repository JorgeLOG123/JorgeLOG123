# Construyendo mi camino como backend developer

*Estudiante de Programación (UNaB), enfocado en Java y el ecosistema Spring.*

### Construyendo con

Java y Spring Framework (Boot, Data JPA) para aplicaciones backend robustas, con MySQL para la persistencia de datos. Python para automatización y scripts, y Git para versionar cada paso del proceso.

[![My Skills](https://skillicons.dev/icons?i=java,spring,mysql,python,git,github,idea,bash)](https://skillicons.dev)

### Ampliando capacidades con

Spring Security y JWT para sumar autenticación segura a mis APIs, y HTML, CSS, JavaScript y Bootstrap para completar el lado frontend.

[![My Skills](https://skillicons.dev/icons?i=html,css,js,bootstrap)](https://skillicons.dev)

Con ganas de seguir sumando proyectos. Espero que encuentres algo útil por acá.

---

### 🐍 Contribution Snake

![Contribution snake animation](https://raw.githubusercontent.com/JorgeLOG123/JorgeLOG123/output/github-contribution-grid-snake.svg)

**⚙️ Setup: cómo activar la serpiente**

Creá `.github/workflows/snake.yml` en este mismo repo (`JorgeLOG123/JorgeLOG123`) con este contenido:

```yaml
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    steps:
      - uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

Después andá a **Settings → Actions → General → Workflow permissions** en ese repo y activá *Read and write permissions* — sin eso, el Action no puede publicar el SVG y la serpiente no aparece.
