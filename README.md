# Project Starter Template

Plantilla base para iniciar repositorios consistentes en GitHub.

## Que incluye
- Estandares de Git y edicion (`.gitattributes`, `.editorconfig`, `.gitignore`).
- Plantillas de colaboracion (PR e issues).
- Workflow CI multi-stack en GitHub Actions.
- Guia de contribucion y convencion de commits.

## CI incluido
El workflow `.github/workflows/ci.yml` detecta automaticamente el stack por archivos:
- Java/Maven: si existe `pom.xml`
- Node.js: si existe `package.json`
- Python: si existe `pyproject.toml` o `requirements.txt`
- Docker: si existe `Dockerfile`

## Como usar esta plantilla
1. En GitHub, presiona **Use this template**.
2. Crea el nuevo repo.
3. Ajusta el `README.md` y variables del proyecto.
4. Haz tu primer push y revisa Actions.

## Convencion de commits
Usa Conventional Commits:
- `feat: ...`
- `fix: ...`
- `refactor: ...`
- `test: ...`
- `ci: ...`
- `docs: ...`
- `chore: ...`

Ejemplo:
`feat(auth): add jwt refresh endpoint`

## Notas
- La parte "global" (estandares, PR/issues, convenciones) aplica a cualquier proyecto.
- La parte "build/test" siempre depende del stack; por eso el workflow viene con jobs condicionales por tecnologia.
