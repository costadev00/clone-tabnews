# clone-tabnews

Projeto para reproduzir o [TabNews](https://tabnews.com.br) como parte do curso **curso.dev**, cobrindo fundamentos e práticas essenciais de engenharia de software.

## Objetivos

- Exercitar os módulos do curso.dev em um projeto completo.
- Criar uma aplicação funcional semelhante ao TabNews.
- Aplicar boas práticas de versionamento, testes e automação.

## Pilares do curso.dev

1. **Fundamentos**: JavaScript, Node.js, React, Next.js e PostgreSQL.
2. **Arquitetura**: padrões de projeto, escalabilidade e manutenção.
3. **DevOps**: Docker, Docker Compose, CI/CD e observabilidade.
4. **Soft Skills**: colaboração, documentação e delivery contínuo.

## Stack principal

- Node.js + Next.js
- PostgreSQL
- Docker & Docker Compose
- ESLint, Prettier e Jest

## Pré-requisitos

- Git
- Docker >= 20
- Docker Compose >= 2
- Node.js >= 18 (opcional para utilitários locais)
- Make (opcional)

## Como rodar o projeto

```bash
docker compose up --build
```

Aplicação: `http://localhost:3000`

Banco: `localhost:5432` (usuario, senha e database definidos em `docker-compose.yml`).

Para desligar:

```bash
docker compose down
```

## Estrutura esperada

- `frontend/` – interface e rotas Next.js.
- `backend/` – APIs, lógica de negócios e integrações.
- `db/` – migrações e seeds.
- `tests/` – testes unitários e de integração.
- `docs/` – anotações e materiais do curso.

## Fluxo de desenvolvimento

1. Criar branches por feature.
2. Atualizar dependências com `docker compose build`.
3. Rodar testes com `docker compose run --rm app npm test`.
4. Abrir PR, revisar e ajustar conforme feedback.

## Próximos passos

- Implementar autenticação e CRUD de posts.
- Construir feed, comentários e sistema de votos.
- Configurar monitoramento e deploy contínuo.
- Documentar aprendizados relevantes do curso.

## Recursos úteis

- [Curso.dev](https://curso.dev)
- [TabNews](https://tabnews.com.br)
- [Documentação Next.js](https://nextjs.org/docs)
- [Docker Docs](https://docs.docker.com)
- [PostgreSQL Docs](https://www.postgresql.org/docs)