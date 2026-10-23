# Rede de Fornecedores · LOC Frotas

Painel: https://gabrielpitter77.github.io/fornecedores/

- `index.html`: a página do painel. Não contém dados.
- `base.enc`: a base de fornecedores, **criptografada** (AES-256-GCM, chave PBKDF2 com 600 mil iterações). Sem usuário e senha, o conteúdo é ilegível.

## Atualizar a base (administrador)

1. Baixe o relatório de fornecedores do sistema.
2. Abra `https://gabrielpitter77.github.io/fornecedores/?admin=1` e faça login.
3. Menu ⚙ → **Carregar base** → escolha a planilha.
4. Confira o resumo e clique em menu ⚙ → **Gerar base.enc para publicar**.
5. Neste repositório: **Add file → Upload files**, arraste o `base.enc` baixado (substitui o antigo) e clique em **Commit changes**.
6. Em até ~10 minutos todos veem a base nova pelo link normal.

## Cuidados

- Nunca suba a planilha (.xlsx), CSV ou JSON aqui: o repositório é público.
- Trocar a senha: menu ⚙ → **Trocar usuário/senha** (modo `?admin=1`), depois suba o `base.enc` novo. A senha antiga deixa de funcionar.
