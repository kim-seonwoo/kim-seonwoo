name: GitHub City
uses: lowlighter/metrics@latest
with:
  filename: metrics.plugin.skyline.city.svg
  token: NOT_NEEDED
  base: ""
  plugin_skyline: yes
  plugin_skyline_year: 2020
  plugin_skyline_frames: 6
  plugin_skyline_quality: 1
  plugin_skyline_settings: |
    {
      "url": "https://honzaap.github.io/GithubCity?name=${login}&year=${year}",
      "ready": "[...document.querySelectorAll('.display-info span')].map(span => span.innerText).includes('${login}')",
      "wait": 4,
      "hide": ".github-corner, .footer-link, .buttons-options, .mobile-rotate, .display-info span:first-child"
    }
