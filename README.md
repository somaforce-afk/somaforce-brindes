# Somaforce — controle de brindes

Interface estática para GitHub Pages. O banco de dados e a API permanecem no Supabase.

## Publicação

1. Crie um repositório público chamado `somaforce-brindes`.
2. Envie `index.html` e `.nojekyll` para a raiz da branch `main`.
3. Em **Settings → Pages**, selecione **Deploy from a branch**, **main** e **/(root)**.
4. Aguarde o Pages informar o endereço `https://<usuario>.github.io/somaforce-brindes/`.

A senha de acesso é verificada pela API no Supabase. Ela não deve ser incluída neste repositório.
O acesso fica válido por até 12 horas na aba atual; fechar a aba encerra a sessão local.

## Arquitetura

- Frontend: HTML, CSS e JavaScript em `index.html`.
- API: função `somaforce-brindes` do projeto Supabase existente.
- Dados: tabelas protegidas por RLS no Supabase.

O projeto GitHub Pages é público; o código da interface pode ser visto por qualquer pessoa.
