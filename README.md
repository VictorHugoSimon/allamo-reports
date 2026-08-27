# Államo Reports Hub

Repositório exclusivo para publicação dos relatórios HTML do PMO, segmentados por empresa e projeto.

## Estrutura

```text
/
├── index.html
├── dual/
│   ├── index.html
│   ├── status-report/YYYY-MM-DD/index.html
│   ├── mit/<codigo>/YYYY-MM-DD/index.html
│   └── plano-acao/YYYY-MM-DD/index.html
├── opr/
│   └── index.html
└── madri/
    └── index.html
```

## Convenção

- Uma empresa nunca compartilha pasta de documentos com outra.
- Um report novo cria uma pasta datada; não sobrescreve histórico.
- O `index.html` da empresa aponta para os relatórios atuais.
- GitHub Pages publica automaticamente após push na `main`.

## Segurança

GitHub Pages em repositório público é público na internet. Não publicar senhas, tokens, dados pessoais sensíveis, FCH detalhado ou informações internas que não possam ser vistas pelo cliente.
