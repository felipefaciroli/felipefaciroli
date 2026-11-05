<h1 align="center">Hi, I'm Felipe Faciroli 👋</h1>
<h3 align="center">React & NestJS developer, and a gamer in my spare time</h3>

<p align="center">
  <img alt="Pixel art by Pixel Jeff (behance.net/pixeljeff)" src="https://mir-s3-cdn-cf.behance.net/project_modules/1400_opt_1/9afe0493484903.5e66500f8dea4.gif" />
</p>

## 🛠️ Stack <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="28">

<p align="left">
  <img src="https://skillicons.dev/icons?i=react,ts,nestjs,express,nodejs,mongodb" alt="React, TypeScript, NestJS, Express, Node.js, MongoDB" />
</p>

## 📊 GitHub Stats

<p align="center">
  <img src="./profile-summary-card-output/radical/0-profile-details.svg" alt="Profile details" width="100%" />
</p>

<p align="center">
  <img src="./profile-summary-card-output/radical/3-stats.svg" alt="GitHub stats" height="180" />
  <img src="./profile-summary-card-output/radical/2-most-commit-language.svg" alt="Most commit languages" height="180" />
</p>

<p align="center">
  <img src="./profile-summary-card-output/radical/1-repos-per-language.svg" alt="Repos per language" height="180" />
  <img src="./profile-summary-card-output/radical/4-productive-time.svg" alt="Productive time" height="180" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=felipefaciroli&theme=radical&hide_border=true" alt="GitHub streak" />
</p>

## ☕ Social

<p align="left">
  <a href="mailto:felipef.dev@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" /></a>
  <a href="https://www.instagram.com/felipe.faciroli/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" /></a>
  <a href="https://felipefaciroli.com.br"><img src="https://img.shields.io/badge/Website-000000?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
</p>

2. Action que gera os indicadores

No repositório felipefaciroli/felipefaciroli, crie o arquivo .github/workflows/profile-cards.yml:

name: Profile summary cards

on:
  schedule:
    - cron: "0 3 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: vn7n24fzkq/github-profile-summary-cards@release
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          USERNAME: ${{ github.repository_owner }}
