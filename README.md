# elkuku.dev

Front page for [elkuku.dev](https://elkuku.dev): a single static page in plain HTML and CSS, with no build step or JavaScript. It follows the system light/dark setting and works on phones.

It links to the sites hosted on the same Plesk server:

- [4e-ecuador.elkuku.dev](https://4e-ecuador.elkuku.dev/)
- [agent-tools.elkuku.dev](https://agent-tools.elkuku.dev/)
- [atacames.elkuku.dev](https://atacames.elkuku.dev/)
- [kgpsdiary.elkuku.dev](https://kgpsdiary.elkuku.dev/)
- [maxfielder.elkuku.dev](https://maxfielder.elkuku.dev/)
- [minicc.elkuku.dev](https://minicc.elkuku.dev/)

## Files

- `index.html`: the page, with styles inline
- `img/`: avatar and icons
- `favicon.ico`

## Local preview

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765.

## Deployment

The site is deployed through Plesk's Git integration. Plesk hosts the repository and deploys the `master` branch to `httpdocs` automatically on every push.

| Remote   | Where                         | Purpose                     |
|----------|-------------------------------|-----------------------------|
| `origin` | Plesk repo on the server      | Pushing here deploys live   |
| `github` | github.com/elkuku/elkuku.dev  | Public mirror               |

```bash
git push origin master   # deploy
git push github master   # update GitHub
```
