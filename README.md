# Vitrine de material didático

Página estática única que consolida os artefatos de aula autorais das disciplinas de Engenharia de
Software (UniCesumar), para servir de link único em currículo e perfil profissional, no lugar de
vários repositórios soltos. Regra da página: só entra artefato usado em aula, com página no ar ou
código público, e todo link é verificado (página responde 200, repositório e imagem públicos).

## Conteúdo

- `index.html` — a página inteira. HTML e CSS num arquivo só, sem JavaScript, sem CDN, sem
  framework, sem fonte externa. Tema claro e escuro por `prefers-color-scheme`, layout de coluna
  única que se ajusta até largura de celular.

Não há build. Abrir o arquivo no navegador já mostra o resultado final.

## Artefatos apresentados

| Artefato | Página no ar | Código/imagem pública |
|---|---|---|
| Runtime de tool calling no navegador | `pedrosatin.github.io/runtime-tool-calling` | `pedrosatin/runtime-tool-calling` |
| Laboratório de prompt injection | `pedrosatin.github.io/laboratorio-prompt-injection` | `pedrosatin/laboratorio-prompt-injection` |
| Servidores MCP da disciplina | — (imagens Docker) | `psatin/mcp-pokeapi`, `psatin/mcp-diario-violao` no Docker Hub |
| Prova de Programação Web em 2024 | `pedrosatin.github.io/prova-ibge-noticias` | `pedrosatin/prova-ibge-noticias` |
| Programação Web e React em 2024 | — (só código) | `pedrosatin/proffy-web`, `calc-react`, `tasks-react`, `minefield-react`, `calc-angular` (arquivados) |

## Como publicar

Repositório privado `pedrosatin/vitrine-material-didatico`, com GitHub Pages público a partir da
branch `main`, pasta `/ (root)`. O endereço é `https://pedrosatin.github.io/vitrine-material-didatico/`.
Basta commitar e dar push: o deploy é automático.

## Manutenção

Ao publicar um artefato novo, copiar um bloco `<section class="card">` existente e manter a mesma
estrutura: problema pedagógico, o que é, stack, links. A regra da página é não afirmar nada que não
esteja verificável no repositório correspondente — sem métrica estimada, sem número de alunos, sem
resultado não medido.
