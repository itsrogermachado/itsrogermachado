# CRM Grupos VIP — Estudo de caso técnico

**Tipo:** aplicação de gestão de assinaturas | **Código:** repositório privado | **Stack:** React, TypeScript, Vite, Supabase/PostgreSQL, Edge Functions

## Problema
Para administrar um serviço de assinaturas, o operador precisa identificar vencimentos, acompanhar cobranças, registrar pagamentos e organizar assinantes, especialmente a partir do celular.

## Funcionalidades documentadas no produto
- Cadastro de assinantes e planos, vencimentos e estados de renovação.
- Links públicos de cobrança e criação de pagamentos Pix.
- Integrações com serviços externos de pagamento e mensagens.
- Painel administrativo, histórico e exportação de dados.
- Interface voltada ao uso diário no celular, com versão PWA.

## Fluxo simplificado de arquitetura (conceitual)
1. React renderiza painel e formulários.
2. Supabase Auth identifica o operador, com dados do grupo isolados por regras de acesso.
3. PostgreSQL persiste planos, assinantes, vencimentos e pagamentos.
4. Edge Functions intermedeiam cobranças e comunicação com APIs externas.
5. Webhooks atualizam estados após eventos de pagamento.

Este fluxo é uma simplificação para apresentação, não um diagrama definitivo de todas as dependências.

## Evidências e limites
O repositório contém rotas públicas de checkout, uma configuração Playwright e arquivos de testes. A simples presença desses arquivos **não comprova cobertura automatizada completa nem resultados verdes**.
Não publicar números de clientes, taxa de renovação, pagamentos processados ou disponibilidade sem relatórios verificáveis. A documentação interna do produto registra que antigas estatísticas promocionais eram fictícias.

## Cuidados de apresentação
Nenhum link direto para o código privado. Capturas devem ser feitas em conta demonstrativa, removendo nomes, telefones, valores reais, tokens, QR Codes e URLs de cobrança. Os resultados devem vir de métricas exportadas e auditadas, com consentimento e anonimização.
