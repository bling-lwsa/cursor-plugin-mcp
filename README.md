# Plugin Bling para o Cursor

Este plugin conecta o Cursor ao [Bling ERP](https://www.bling.com.br) para consultar e gerenciar pedidos, notas fiscais, estoque, financeiro e contatos.

O plugin aponta para o servidor MCP hospedado pelo Bling em `https://mcp.bling.com.br/mcp`. Não há servidor, código ou executável para instalar neste repositório.

## Como funciona

- No primeiro uso, o Cursor abre a autorização OAuth e você entra com a sua conta Bling.
- A autorização usa Dynamic Client Registration, então você não precisa criar nem informar client id, client secret ou token.
- O `mcp.json` não contém headers, autenticação nem variáveis de ambiente.

## Estrutura

```
.cursor-plugin/plugin.json   manifest do plugin
mcp.json                     aponta para o MCP hospedado do Bling
assets/logo.svg              logo do plugin (placeholder)
README.md
```