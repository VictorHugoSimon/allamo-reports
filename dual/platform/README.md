# Dual Clima · Plataforma de Governança PMO

Branch de evolução não destrutiva da plataforma atual.

## Arquitetura atual

GitHub → HTML/JS → Vercel → Supabase

## Módulos HTML

- `index.html` — Portal
- `plano-acao/` — Plano de Ação operacional existente
- `pop/` — POP + versões
- `mapa-implantacao/` — Mapa Mestre Stage-Gate
- `requisitos/` — Matriz de Requisitos
- `testes/` — Plano Mestre de Testes
- `riscos/` — Registro de Riscos
- `integracoes/` — Gestão de Integrações
- `documentos/` — Gestão Documental
- `status-report/` — Status Report Executivo do cliente
- `mit053/` — MIT053 / cargas
- `cadastro/` — Cadastro Mestre / saneamento
- `pcp003/` — PCP003 / Código Inteligente
- `intercompany/` — Intercompany
- `rfi/` — RFI
- `perguntas-status/` — Perguntas/Pendências para Status
- `auditoria/` — Auditoria viva da plataforma

## Banco

Projeto Supabase exclusivo `dual-pmo`.

O código público utiliza somente a publishable key. Nenhum secret de servidor é armazenado no HTML/JavaScript.

As novas tabelas utilizam `project_scope = DUAL` e RLS.

## Regra de governança

Reunião / documento / evidência → decisão / requisito / gap / risco → Plano de Ação → execução → teste → evidência → aceite → documentação → Status Report → Go-Live.

## Promoção

Não substituir a produção existente sem preview/stage e smoke tests.
