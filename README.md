# open-law-api-docs

Swagger UI documentation for the [Korean Legislative Service (법제처) Open API](https://open.law.go.kr/LSO/index.html).

## Live

https://open-law-api-docs-wookbros.vercel.app

## Features

- Interactive API documentation with Swagger UI
- Covers all 4 endpoints: case law search/detail, legislation search/detail
- API proxy via Vercel Rewrites (resolves mixed content issue)
- Automatic deployments on push to `main`

## API Endpoints

| Endpoint | Description |
|----------|-------------|
| `lawSearch.do?target=prec` | Search case law list |
| `lawService.do?target=prec` | Get case law detail |
| `lawSearch.do?target=eflaw` | Search legislation list by enforcement date |
| `lawService.do?target=eflaw` | Get legislation detail |

> Base URL: `http://www.law.go.kr/DRF/`

## Local Development

```bash
npx http-server . -p 8080
```

Open `http://localhost:8080` in your browser.

## Deployment

Deployed via [Vercel](https://vercel.com) with automatic deployments on push to `main`.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
