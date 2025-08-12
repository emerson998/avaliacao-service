# Avaliação Service API

Este projeto implementa uma API REST para gerenciamento de avaliações de produtos utilizando Spring Boot. O foco deste componente é expor um endpoint que retorna as avaliações associadas a um produto específico.

## Visão Geral

O controlador `AvaliacaoController` disponibiliza um endpoint para buscar avaliações por `produtoId`. As avaliações são filtradas a partir de um repositório em memória (ou persistente) e retornadas em formato JSON.

## Endpoints

### GET /avaliacoes

Retorna uma lista de avaliações relacionadas a um produto.

**Parâmetros:**

| Parâmetro  | Tipo   | Descrição               | Obrigatório |
|------------|--------|-------------------------|-------------|
| produtoId  | Long   | ID do produto a ser buscado | Sim         |
