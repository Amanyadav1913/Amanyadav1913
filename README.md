 <p align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&height=280&text=Aman%20Yadav&fontSize=60&fontColor=ffffff&animation=twinkling&color=gradient"/>
</p>

<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=24&duration=2500&pause=900&color=00F7FF&center=true&vCenter=true&width=700&lines=Software+Developer;Frontend+Developer;React+Developer;JavaScript+Developer;DSA+Learner;Open+Source+Learner;Future+Software+Engineer"/>
</p>

## 👨‍💻 About Me

🎓 B.Tech CSE Student

💻 Passionate Frontend Developer

📚 Daily DSA Practice

🌱 Learning React + Backend

🚀 Building Real World Projects

🎯 Dream → Software Engineer

⚡ Fun Fact:
I enjoy solving bugs more than creating them 😄

<p align="center">
<img src="https://skillicons.dev/icons?i=c"/>
<img src="https://skillicons.dev/icons?i=cpp"/>
<img src="https://skillicons.dev/icons?i=js"/>
<img src="https://skillicons.dev/icons?i=html"/>
<img src="https://skillicons.dev/icons?i=css"/>
</p>

<p align="center">
<img src="https://skillicons.dev/icons?i=react"/>
<img src="https://skillicons.dev/icons?i=tailwind"/>
<img src="https://skillicons.dev/icons?i=bootstrap"/>
</p>

<p align="center">
<img src="https://skillicons.dev/icons?i=nodejs"/>
<img src="https://skillicons.dev/icons?i=express"/>
<img src="https://skillicons.dev/icons?i=mongodb"/>
</p>

<p align="center">
<img src="https://skillicons.dev/icons?i=git"/>
<img src="https://skillicons.dev/icons?i=github"/>
<img src="https://skillicons.dev/icons?i=vscode"/>
<img src="https://skillicons.dev/icons?i=figma"/>
<img src="https://skillicons.dev/icons?i=npm"/>
</p>

<p align="center">

<a href="YOUR_LEETCODE_PROFILE">
<img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white"/>
</a>

<a href="YOUR_CODEFORCES_PROFILE">
<img src="https://img.shields.io/badge/Codeforces-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white"/>
</a>

<a href="YOUR_GEEKSFORGEEKS_PROFILE">
<img src="https://img.shields.io/badge/GeeksforGeeks-2F8D46?style=for-the-badge&logo=geeksforgeeks&logoColor=white"/>
</a>

</p>

name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: Amanyadav1913
          outputs: |
            dist/github-contribution-grid-snake-dark.svg

      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
