# GitHub-Homework

Ez a repository egy GitHub Actions workflow-t tartalmaz, amely Docker image-et épít és pushol Docker Hubra.  
Az image egy egyszerű Nginx szervert tartalmaz, amely egy egyedi üdvözlő oldalt jelenít meg.

## Fájlok
- `Dockerfile`: Az Nginx image konfigurációja
- `index.html`: Az egyedi kezdőlap
- `.github/workflows/docker-build.yml`: GitHub Actions workflow a build és push folyamatokhoz
- `.gitignore`: A szükségtelen fájlok kihagyása a repository-ból
- `README.md`: Ez a fájl, amely elmagyarázza a repository célját

## Használat
1. Forkold ezt a repót.
2. Állítsd be a GitHub Secrets-ben a `DOCKERHUB_USERNAME` és `DOCKERHUB_TOKEN` változókat.
3. Pusholj a `main` branch-re, és ellenőrizd a Docker Hubon az új image-et.
