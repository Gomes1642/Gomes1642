
Olá! Eu sou o Bruno Mattos.


- 💻 Hoje trabalho no Administrativo-financeiro do Grupo Moura.
- 📚 Estudando Java.

<div>
  <a href="https://github.com/Gomes1642">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Gomes1642&show_icons=true&theme=dark&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Gomes1642&layout=compact&langs_count=16&theme=dark"/>
</div>
  
  <div>
    <a href="https://www.linkedin.com/in/bruno-mattos-8914b51b3" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  </div>
  
  ![Snake animation](https://github.com/gomes1642/gomes1642/blob/output/github-contribution-grid-snake.svg)
  name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
