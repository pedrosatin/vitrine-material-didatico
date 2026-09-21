# Vitrine de material didático

Página estática única que consolida os artefatos de aula autorais das disciplinas de Engenharia de
Software (UniCesumar), para servir de link único em currículo e perfil profissional, no lugar de
vários repositórios soltos. Só entra artefato usado em aula, com página no ar ou código público, e
todo link é verificado. A página responde 200, o repositório e a imagem são públicos.

## Conteúdo

`index.html` é a página inteira. HTML e CSS num arquivo só, sem JavaScript, sem CDN, sem framework
e sem fonte externa. Tema claro e escuro por `prefers-color-scheme`, em coluna única que se ajusta
até largura de celular.

Não há build. Abrir o arquivo no navegador já mostra o resultado final.

## Artefatos apresentados

| Artefato | Página no ar | Código ou imagem pública |
|---|---|---|
| Runtime de tool calling no navegador | `pedrosatin.github.io/runtime-tool-calling` | `pedrosatin/runtime-tool-calling` |
| Laboratório de prompt injection | `pedrosatin.github.io/laboratorio-prompt-injection` | `pedrosatin/laboratorio-prompt-injection` |
| Extrator de diff de pull request | `pedrosatin.github.io/pr-diff-extractor` | `pedrosatin/pr-diff-extractor` |
| Servidores MCP da disciplina | `pedrosatin.github.io/guitar-study` (domínio do diário) | `psatin/mcp-pokeapi` e `psatin/mcp-diario-violao` no Docker Hub |
| Prova de Programação Web em 2024 | `pedrosatin.github.io/prova-ibge-noticias` | `pedrosatin/prova-ibge-noticias` |

## Como publicar

Repositório privado `pedrosatin/vitrine-material-didatico`, com GitHub Pages público a partir da
branch `main`, pasta `/ (root)`. O endereço é `https://pedrosatin.github.io/vitrine-material-didatico/`.
Basta commitar e dar push. O deploy é automático.

## Manutenção

Ao publicar um artefato novo, copiar um bloco `<section class="card">` existente e manter a mesma
estrutura, com problema pedagógico, o que é, stack e links. A página não afirma nada que não esteja
verificável no repositório correspondente. Sem métrica estimada, sem número de alunos e sem
resultado não medido.
