- 👋 Hi, I’m @manu-jutt
- 👀 I’m interested in Football
- 🌱 I’m currently learning Java script 
  
- 📫 How to reach me ...
- Whatsapp:03000355543
- 😄 Pronouns: he/him😁
- ⚡ Fun fact: I have 1000 ball knowledge but 17 ball playing😅

<!---
manu-jutt/manu-jutt is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
name: Generate snake animation

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"

  workflow_dispatch:

  push:
    branches:
    - master

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: dist/snake.svg?palette=github-dark


      - name: push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=manu-jutt&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dracula&locale=en&hide_border=false&order=1" height="150" alt="stats graph"  />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=manu-jutt&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false&order=2" height="150" alt="languages graph"  />
  <img src="https://streak-stats.demolab.com?user=manu-jutt&locale=en&mode=daily&theme=dracula&hide_border=false&border_radius=5&order=3" height="150" alt="streak graph"  />
  <img src="https://github-profile-trophy.vercel.app?username=manu-jutt&theme=dracula&column=-1&row=1&margin-w=8&margin-h=8&no-bg=false&no-frame=false&order=4" height="150" alt="trophy graph"  />
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=manu-jutt&radius=16&theme=react&area=true&order=5" height="300" alt="activity-graph graph"  />
</div>

###

<img src="https://raw.githubusercontent.com/manu-jutt/manu-jutt/output/snake.svg" alt="Snake animation" />

###

<div align="left">
  <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/linkedin/default.svg" width="52" height="40" alt="linkedin logo"  />
  <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/twitter/default.svg" width="52" height="40" alt="twitter logo"  />
  <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/discord/default.svg" width="52" height="40" alt="discord logo"  />
  <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/youtube/default.svg" width="52" height="40" alt="youtube logo"  />
</div>

###

<div align="center">
  <img height="200" src="https://i.imgflip.com/65efzo.gif"  />
</div>

###
