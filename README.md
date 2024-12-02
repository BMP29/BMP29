[![Readme Quotes](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark&border=true)](https://github.com/piyushsuthar/github-readme-quotes)

![](https://komarev.com/ghpvc/?username=bmp29)

[![Anurag's GitHub stats-Dark](https://github-readme-stats.vercel.app/api?username=bmp29&show_icons=true&theme=dark#gh-dark-mode-only)](https://github.com/bmp29/github-readme-stats#gh-dark-mode-only)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=bmp29&layout=donut-vertical)](https://github.com/bmp29/github-readme-stats)


[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=bmp29)](https://git.io/streak-stats)

name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
