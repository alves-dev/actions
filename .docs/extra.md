[AI Code Review](./.github/workflows/analyze-agent.yml): Faz analise do commit utilizando a StackSpot AI

[Build Docker Image](./.github/workflows/build-docker.yml): Realiza o build da imagem docker e publica no GitHUb

[Readme Generate](./.github/workflows/readme-generate.yml): Aciona script na minha infra para gerar o README.md automaticamente

[Sonar Scan](./.github/workflows/sonar.yml): Faz o scan e comenta no PR caso haja um aberto


Como usar o [update-repo-metadata.yml](../.github/workflows/update-repo-metadata.yml)
```
name: Update Repo Info

on:
  push:
    paths:
      - '.repo.yml'

jobs:
  update-metadata:
    uses: alves-dev/actions/.github/workflows/update-repo-metadata.yml@latest
    secrets:
      token: ${{ secrets.PERSONAL_GITHUB_TOKEN }}
```