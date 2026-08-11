# 💫 About Me:
🔭 I’m currently working on<br>👯 I’m looking to collaborate on<br>🤝 I’m looking for help with<br>🌱 I’m currently learning<br>💬 Ask me about<br>⚡ Fun fact


## 🌐 Socials:
[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/https://discord.gg/JFuarzs5Fz) [![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/thisisaayush__)

name: Generate Snake Animation

on:
  # Har 24 ghante me auto-run hoga
  schedule:
    - cron: "0 0 * * *"
  
  # Manually run karne ka option
  workflow_dispatch:
  
  # Push par run hoga
  push:
    branches:
      - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      # Snake Animation SVG generate karega
      - name: Generate github-contribution-grid-snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: aayushzen
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      # Generated SVGs ko 'output' branch me push karega
      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

# 💻 Tech Stack:
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Firebase](https://img.shields.io/badge/firebase-a08021?style=for-the-badge&logo=firebase&logoColor=ffcd34) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.shion.dev/api?username=aayushzen&theme=ambient_gradient&hide_border=false&include_all_commits=true&count_private=false)<br/>
![](https://streak-stats.demolab.com/?user=aayushzen&theme=ambient_gradient&hide_border=false)<br/>
![](https://github-readme-stats.shion.dev/api/top-langs/?username=aayushzen&theme=ambient_gradient&hide_border=false&include_all_commits=true&count_private=false&layout=compact)

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=aayushzen&theme=default&no-frame=false&no-bg=true&margin-w=4)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark)

### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=aayushzen&limit=5&theme=dark&combine_all_yearly_contributions=true)

---
[![](https://komarev.com/ghpvc/?username=aayushzen&icon=9&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
