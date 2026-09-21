# Teaching material showcase

A single static page that gathers the original class artifacts from Software Engineering
courses (UniCesumar), to serve as one link on a resume or professional profile instead of
several loose repositories. Only artifacts actually used in class are listed, each with a live
page or public code, and every link is checked. The page responds 200, and the repository and
image are public.

## Contents

`index.html` is the whole page: HTML and CSS in a single file, no JavaScript, no CDN, no
framework, and no external font. Light and dark themes follow `prefers-color-scheme`, in a
single column that adapts down to phone width.

There is no build step. Opening the file in a browser already shows the final result.

## Artifacts featured

| Artifact | Live page | Public code or image |
|---|---|---|
| Browser-based tool calling runtime | `pedrosatin.github.io/runtime-tool-calling` | `pedrosatin/runtime-tool-calling` |
| Prompt injection lab | `pedrosatin.github.io/laboratorio-prompt-injection` | `pedrosatin/laboratorio-prompt-injection` |
| Pull request diff extractor | `pedrosatin.github.io/pr-diff-extractor` | `pedrosatin/pr-diff-extractor` |
| Course MCP servers | `pedrosatin.github.io/guitar-study` (diary's domain) | `psatin/mcp-pokeapi` and `psatin/mcp-diario-violao` on Docker Hub |
| 2024 Web Programming exam | `pedrosatin.github.io/prova-ibge-noticias` | `pedrosatin/prova-ibge-noticias` |

## How it is published

Public repository `pedrosatin/vitrine-material-didatico`, with GitHub Pages served from the
`main` branch, `/ (root)` folder, via the workflow in `.github/workflows/pages.yml`. The address
is `https://pedrosatin.github.io/vitrine-material-didatico/`. Committing and pushing to `main`
is enough; deployment is automatic.

## Maintenance

When publishing a new artifact, copy an existing `<section class="card">` block and keep the
same structure: teaching problem, what it is, stack, and links. The page states nothing that
isn't verifiable in the corresponding repository. No estimated metrics, no student counts, and
no unmeasured results.

## License

MIT. See [LICENSE](LICENSE).
