# Nova Era MTDS — Estudo de caso técnico

**Tipo:** produto web em operação | **Papel:** desenvolvimento e manutenção full-stack | **Período:** desde jan/2026

**Demonstração pública:** https://novaeramtds.com

## Problema e solução
Aplicação para registrar operações, despesas, resultados e metas, consolidando indicadores em painéis e oferecendo experiência instalável (PWA). O escopo também inclui login, perfis e ferramentas administrativas.

## Arquitetura observável no repositório privado
- Interface React + TypeScript + Vite + Tailwind; projeto configurado como PWA.
- Supabase Auth e PostgreSQL; migrações versionadas e políticas de acesso por usuário (RLS).
- Edge Functions em TypeScript/Deno para integrações de pagamento, webhooks, notificações e serviços agendados.
- Webhook SyncPay contém lógica de consulta à API do provedor antes de confirmar pagamentos e tratamento para avisos repetidos; isso é uma decisão de projeto observada no código, **não uma certificação de segurança ou prova de operação sem falhas**.
- Página pública e identidade visual verificáveis no endereço acima. As telas autenticadas não são expostas nesta documentação.

## Responsabilidades e decisões técnicas para apresentar em entrevista
1. Modelagem e isolamento de dados por meio de RLS e migrações.
2. Fluxo completo: interface → autenticação → consulta/atualização de dados → Edge Functions.
3. Desafios de sincronização frontend/backend e cache em PWA.
4. Tratamento de notificações de pagamento e idempotência.
5. Evolução de um sistema existente com usuários, sem interromper a operação.

## O que ainda precisa de comprovação
- Contagens de tabelas, políticas e commits mencionadas em versões antigas do currículo são **declarações históricas**; recontar no commit escolhido antes de divulgar números definitivos.
- Não foram coletadas métricas auditáveis de MAU, uptime, latência, receitas ou volume de pagamentos.
- Existem planos de correção de segurança e documentação de riscos; a implementação de cada melhoria deve ser validada contra o estado atual.
- Capturas de telas internas devem ser produzidas com dados demonstrativos e revisão de privacidade.

## Demonstração em entrevista
Usar a landing pública, um usuário de teste sem dados reais e uma apresentação de arquitetura simplificada. Não divulgar chaves, dados de clientes, endpoints privados ou capturas de produção com informações identificáveis.
