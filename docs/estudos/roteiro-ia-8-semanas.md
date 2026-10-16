# Roteiro de estudos: Full-Stack → Aplicações com IA (8 semanas)

**Status:** plano de aprendizagem; não representa experiência profissional já adquirida.
**Pré-requisitos:** JavaScript/TypeScript, HTTP, APIs, React, Git e noções de SQL.

## Semana 1 — Fundamentos de LLMs
Tokens, janelas de contexto, embeddings, inferência, temperatura, custos, limites e diferenças entre modelos. Exercício: integrar um modelo a uma API Node com segredo somente no servidor.

## Semana 2 — Prompting confiável
Instruções, contexto, exemplos, saída estruturada JSON/Zod, tratamento de erros e versionamento de prompts. Exercício: classificador de solicitações com testes e validação de schema.

## Semana 3 — RAG
Chunking, embeddings, indexação, recuperação semântica e citações. Exercício: FAQ sobre documentos próprios usando pgvector/PostgreSQL ou um mecanismo de busca gerenciado.

## Semana 4 — Avaliação de respostas
Criar conjunto de perguntas com gabarito, medir correção, grounding, taxa de abstenção, latência e custo. Exercício: conjunto de 30 casos fixos e relatório comparativo.

## Semana 5 — Ferramentas e agentes
Function/tool calling, permissões, limites de ação, checkpoints e confirmação antes de operações de escrita. Exercício: assistente que consulta pedidos de uma base fictícia em modo somente leitura.

## Semana 6 — Segurança e produção
Prompt injection, vazamento de dados, autenticação, isolamento multiusuário, rate limiting, observabilidade e controle de gastos. Exercício: executar testes adversariais e adicionar métricas.

## Semana 7 — Projeto de portfólio
Construir um **Assistente de Suporte com IA**: Next.js + TypeScript + API server-side + PostgreSQL/pgvector + interface de chat, respostas com fontes e login.

## Semana 8 — Entrega e evidências
Publicar demo com documentos sintéticos, README técnico, vídeo curto, gráfico de custo/latência, conjunto de avaliações e limitações honestas. Preparar apresentação de 5 minutos.

### Critérios mínimos de qualidade
- Chaves de API apenas no servidor e jamais em commits.
- Não prometer 100% de precisão; oferecer citação e abstenção quando não houver base.
- Documentar custo por consulta, limites e trade-offs.
- Construir testes reproduzíveis antes de anunciar o projeto como produção.

### Fontes para estudo
- OpenAI API: https://platform.openai.com/docs
- Documentação PostgreSQL/pgvector: https://github.com/pgvector/pgvector
- Vercel AI SDK: https://ai-sdk.dev/docs
- OWASP LLM Top 10: https://genai.owasp.org/llm-top-10/
