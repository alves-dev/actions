<!--
template_name=header-default
template_version=v1
-->

<h1 align="center" style="color:#F1F5F9;">
  Actions
</h1>

<p align="center">
  <span style="color:#94A3B8; font-size:16px;">
    Contém a abstração das actions usadas em outros projetos
  </span>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/topics-10B981?style=flat-square&logoColor=white"/> <img src="https://img.shields.io/badge/actions-1E293B?style=flat-square&logoColor=white"/>
</p>

<hr/>


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

<!--
template_name=footer-default
template_version=v1
-->

<p align="center">
  <img src="https://img.shields.io/badge/licença-GPL%203-3B82F6.svg" alt="license"/>
</p>

---

<p align="center">
  <strong style="font-size:16px;">Igor Moreira Alves</strong><br/>
  <span style="color:#94A3B8;">Back-end Software Engineer • Java • Python • Spring Boot • AWS</span>
</p>

<p align="center">
  <a href="https://alves-dev.com" target="_blank">
    <img src="https://img.shields.io/badge/site-alves--dev.com-10B981?style=for-the-badge&logo=google-chrome&logoColor=white"/>
  </a>
  <a href="https://www.linkedin.com/in/alves-dev/" target="_blank">
    <img src="https://img.shields.io/badge/linkedin-Igor%20Moireira-3B82F6?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://github.com/alves-dev" target="_blank">
    <img src="https://img.shields.io/badge/github-alves--dev-1E293B?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</p>

<p align="center">
  <sub style="color:#94A3B8;">
    Atualizado em 2026-01-06 19:13
  </sub>
</p>
