# Vitrine de material didático

Página estática única que consolida os artefatos de aula autorais da disciplina de Tecnologias
Emergentes em Engenharia de Software (ESOFT8, UniCesumar), para servir de link único em currículo e
perfil profissional, no lugar de vários repositórios soltos.

## Conteúdo

- `index.html` — a página inteira. HTML e CSS num arquivo só, sem JavaScript, sem CDN, sem
  framework, sem fonte externa. Tema claro e escuro por `prefers-color-scheme`, layout de coluna
  única que se ajusta até largura de celular.

Não há build. Abrir o arquivo no navegador já mostra o resultado final.

## Artefatos apresentados

| Artefato | Repositório |
|---|---|
| Runtime de tool calling no navegador | `pedrosatin/runtime-tool-calling` |
| Laboratório de segurança de agentes | `pedrosatin/laboratorio-seguranca-agentes` |
| Servidores MCP da disciplina | `pedrosatin/mcp-servidores-aula` (imagens `psatin/*` no Docker Hub) |
| Servidor MCP de revisão da B1 | `pedrosatin/mcp-revisao-b1` |
| Acervo de slides por turma | `TI-UNICESUMAR/2026-tecnologias-emergentes-esoft8s-a` e `-b` |

## Como publicar

Esta pasta ainda não é um repositório Git. Qualquer um dos dois caminhos abaixo serve.

### GitHub Pages

1. Criar um repositório público, por exemplo `pedrosatin/vitrine`.
2. Na pasta desta vitrine:

   ```
   git init
   git add index.html README.md
   git commit -m "Vitrine de material didatico"
   git branch -M main
   git remote add origin https://github.com/pedrosatin/vitrine.git
   git push -u origin main
   ```

3. No repositório, em `Settings > Pages`, escolher `Deploy from a branch`, branch `main`, pasta
   `/ (root)`.
4. O endereço sai como `https://pedrosatin.github.io/vitrine/`.

Para servir na raiz do domínio de usuário (`https://pedrosatin.github.io/`), o repositório precisa
se chamar `pedrosatin.github.io`.

### Cloudflare Pages

1. Fazer o push para um repositório Git, como acima.
2. No painel da Cloudflare: `Workers & Pages > Create > Pages > Connect to Git`, escolher o
   repositório.
3. Build command vazio e output directory `/` — é um site estático sem build.
4. O endereço sai como `https://<projeto>.pages.dev`, e um domínio próprio pode ser ligado em
   `Custom domains`.

Alternativa sem Git, pelo Wrangler, a partir desta pasta:

```
npx wrangler pages deploy . --project-name vitrine
```

## Manutenção

Ao publicar um artefato novo, copiar um bloco `<section class="card">` existente e manter a mesma
estrutura: problema pedagógico, o que é, stack, links. A regra da página é não afirmar nada que não
esteja verificável no repositório correspondente — sem métrica estimada, sem número de alunos, sem
resultado não medido.
