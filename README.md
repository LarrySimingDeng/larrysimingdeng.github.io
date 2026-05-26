# larrysimingdeng.github.io

This is the source repository for the personal academic website of **Siming Deng (Larry Deng)** — graduate student at the [Department of Electrical and Systems Engineering](https://www.ese.upenn.edu/) at [Penn Engineering](https://www.seas.upenn.edu/), University of Pennsylvania.

🔗 **Live site:** [https://larrysimingdeng.github.io](https://larrysimingdeng.github.io)

## About

The site showcases my academic profile, research, and professional journey, including:

- **About Me** — background, work experience timeline, and current research focus
- **Publications** — peer-reviewed papers in *Communications in Statistics*, *Statistical Analysis and Data Mining*, and related venues
- **Beyond Research** — hobbies and life outside the lab
- **News & Updates** — milestones, paper acceptances, and offers

### Research Interests
- Machine Learning
- Nonparametric Statistics
- Distortion Measurement Error Models
- Large Sample Theory

## Tech Stack

- **[Jekyll](https://jekyllrb.com/)** — static site generator
- **[GitHub Pages](https://pages.github.com/)** — hosting
- **[Minimal Mistakes](https://mademistakes.com/)** — base theme
- Custom HTML/CSS/JS for the interactive timeline, publication cards, and news grid

## Running Locally

Requirements: Ruby (see `.ruby-version`) and Bundler.

```bash
# Install dependencies
bundle install

# Serve the site locally
bundle exec jekyll serve

# Open http://localhost:4000 in your browser
```

Before serving locally, you may want to comment out the `url:` field in `_config.yml` so that base URLs resolve correctly.

## Project Structure

```
.
├── _config.yml          # Site configuration (title, owner, nav links)
├── _includes/           # Reusable HTML partials
├── _layouts/            # Page layout templates
├── assets/              # CSS, JS, fonts
├── images/              # Logos, paper thumbnails, photos
├── blogs/               # Blog posts
├── mypaper/             # Paper-related assets
├── index.md             # Home / About Me
├── publications.md      # Publications page
├── hobbies.md           # Beyond Research page
├── awards.md            # Awards page
└── README.md
```

## Contact

If you are interested in my work or would like to collaborate, feel free to reach out:

- 📧 Email: `siming_deng_stat [at] 163.com`
- 🎓 [Google Scholar](https://scholar.google.com/citations?hl=en&user=aKyLtgsAAAAJ)
- 🔬 [ResearchGate](https://www.researchgate.net/profile/Siming-Deng-3)
- 💼 [LinkedIn](https://www.linkedin.com/in/larry-deng-317b92360)
- 🐙 [GitHub](https://github.com/LarrySimingDeng)

## Acknowledgements

This site is built on top of the wonderful work of:

- [GuangLun2000 / Hanlin Cai](https://github.com/GuangLun2000/GuangLun2000.github.io) — for the original template this site is forked from
- [Jason Ansel](https://github.com/jansel/jansel.github.io) — for the underlying website framework
- [Minimal Mistakes](https://mademistakes.com/) — for the Jekyll theme

## License

Released under the [MIT License](LICENSE). Content (text, images, publication thumbnails) © Siming Deng. If you reuse the site structure for your own personal page, please keep attribution to the upstream projects above.
