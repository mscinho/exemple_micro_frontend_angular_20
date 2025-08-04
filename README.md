# Micro Frontend Angular - Exemplo

Este repositório demonstra uma arquitetura de micro frontends usando Angular 20 e Module Federation. O projeto é composto por três aplicações:

- **shell**: Aplicação principal (container)
- **feature-dashboard**: Micro frontend do painel
- **feature-store**: Micro frontend da loja

## Estrutura de Pastas

```
micro-frontend/
  shell/
  feature-dashboard/
  feature-store/
  docker-compose.yml
  docker-compose.prod.yml
```

## Como rodar em desenvolvimento (Docker)

1. Certifique-se de que o Docker está instalado e rodando.
2. Na raiz do projeto, execute:

```sh
docker-compose up --build
```

- Acesse o shell: http://localhost:4200
- Acesse o dashboard: http://localhost:4201
- Acesse a loja: http://localhost:4202

## Como rodar em produção (Docker)

1. Na raiz do projeto, execute:

```sh
docker-compose -f docker-compose.prod.yml up --build
```

- Shell: http://localhost:8080
- Dashboard: http://localhost:8081
- Loja: http://localhost:8082

## Observações

- Cada micro frontend é um projeto Angular independente.
- O shell carrega os micro frontends remotamente via Module Federation.
- Alterações no código são refletidas automaticamente em desenvolvimento devido ao volume mapeado.

---

Sinta-se à vontade para adaptar este exemplo para suas necessidades!
