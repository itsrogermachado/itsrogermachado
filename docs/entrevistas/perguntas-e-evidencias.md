# Preparação para entrevista — Full-Stack e transição para IA

## Apresentação de 45 segundos
“Sou desenvolvedor full-stack e estudante de Engenharia de Software. Trabalho principalmente com React, TypeScript, Supabase e PostgreSQL. Tenho experiência desenvolvendo e mantendo produtos web, com autenticação, regras de acesso e integrações. Um dos meus diferenciais é conseguir conectar interface, dados e regras de negócio. Hoje estou aprofundando minha formação em aplicações com LLMs e busco uma equipe onde possa aplicar essa base e evoluir com boas práticas de engenharia.”

## Perguntas que você precisa conseguir defender
1. Como separa autorização da interface e RLS no PostgreSQL? Descreva um teste em que um usuário tenta acessar dados de outro.
2. Como lida com notificação de pagamento repetida? Diferencie recebimento do webhook e confirmação junto ao provedor.
3. Como faz migrations sem indisponibilizar o produto? Explique backup, rollback, janela e compatibilidade de versões.
4. Qual a diferença entre teste unitário, integração e E2E? Cite um fluxo realmente testado e mostre a execução.
5. O que você fez pessoalmente em cada projeto e em que momentos utilizou IA? Quais decisões revisou e validou?
6. Como proteger secrets, endpoints, logs, dados pessoais e chaves de terceiros?
7. Por que escolheu Supabase em vez de backend próprio? Fale de trade-offs e limites.
8. Onde pode haver race condition em checkout e assinaturas? Como investigar?
9. Como a PWA se atualiza? O que acontece quando cliente e servidor estão em versões diferentes?
10. O que são RAG, embeddings, tool calling e avaliações? Responda apenas conforme realmente aprender e implementar.

## Matriz de provas — preencher com dados verificáveis
| Alegação | Prova aceitável | Estado |
|---|---|---|
| Sistema público disponível | URL da landing e registro de acesso | Página inicial verificada; não demonstra fluxos autenticados |
| Codebase React/TypeScript | package.json, arquivos do repositório | Verificado |
| Edge Functions e webhooks | Código e rotas existentes | Verificado; não equivale a teste em produção |
| Testes automatizados | Execução reproduzível no CI com logs | Parcial: Barber Flow possui workflow; status do último run não auditado |
| RLS e migrações | Contagem e revisão das migrações por commit | Ainda não auditado integralmente |
| Métricas de clientes e disponibilidade | Dashboard exportado e período definido | Não apresentado |
| Habilidade profissional em LLMs | Projeto IA com avaliações e código | Ainda a desenvolver |

## Perguntas para fazer ao recrutador
- Como a equipe testa mudanças críticas em produção?
- Quem revisa arquitetura e segurança?
- Onde IA entra no produto e como vocês medem qualidade e custo?
- O que define sucesso nos primeiros 90 dias?
