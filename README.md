# Portfolio

Hugo + [Blowfish](https://blowfish.page/) portfolio site.

## Run

```bash
# Docker
docker compose up

# Or Hugo directly
hugo server -D
```

Then open http://localhost:1313/

## Edit

- Personal info: `config/_default/languages.en.toml`
- About page: `content/about.md`
- Resume: `content/resume.md`
- Projects: `content/projects/*.md`
- Nav menu: `config/_default/menus.en.toml`
- Theme settings: `config/_default/params.toml`

## Deploy

Push to GitHub with Actions workflow, or build with `hugo --minify` and deploy the `public/` folder anywhere.

## Credits

- [Hugo](https://gohugo.io/)
- [Blowfish](https://github.com/nunocoracao/blowfish) by Nuno Coração
