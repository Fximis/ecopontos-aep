# 🌱 EcoPontos

**Plataforma Web de Gamificação para Gestão de Resíduos**

> Trabalho acadêmico — AEP 2026.2 · ADS 3º Semestre · Universidade Cesumar (UNICESUMAR)

---

## Sobre o Projeto

O **EcoPontos** é uma aplicação web que incentiva a reciclagem por meio de gamificação. Usuários registram entregas de materiais recicláveis em pontos de coleta, acumulam pontos e trocam por benefícios reais — como passes de ônibus, descontos em tributos municipais e cupons de parceiros.

A proposta está alinhada com a **ODS 12 da ONU** (Consumo e Produção Responsáveis).

---

## Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| Autenticação | Cadastro e login de usuários com sessão por aba |
| Registro de Entrega | Registra materiais recicláveis com cálculo automático de pontos |
| Histórico de Entregas | Exibe entregas mais recentes (estrutura de pilha) |
| Resgate de Benefícios | Troca pontos por benefícios com validação de saldo |
| Benefícios Resgatados | Histórico de resgates do usuário |
| Desfazer Entrega | Remove a última entrega registrada |

---

## Materiais e Pontuação

| Material | Pontos por kg |
|---|---|
| Papel | 10 pts |
| Plástico | 15 pts |
| Vidro | 20 pts |
| Metal | 25 pts |

---

## Benefícios Disponíveis

| Benefício | Custo |
|---|---|
| 🚌 Passe de ônibus | 75 pts |
| 🎟️ Cupom parceiro | 100 pts |
| 🏪 Desconto em loja | 250 pts |
| 💡 Desconto em conta de serviços | 350 pts |
| 🏛️ Benefício municipal | 500 pts |
| 🚲 Aluguel de bicicleta (1 mês) | 750 pts |

---

## Stack Técnica

- **HTML5 + CSS3 + JavaScript (ES6+)** — aplicação single-page sem dependências externas
- **Design:** Glass-morphism com tema escuro e acentos neon (verde `#39ff14` e ciano `#00e5ff`)
- **Fontes:** Sora · JetBrains Mono
- **Persistência:** in-memory (dados por sessão, sem banco de dados)

---

## Modelagem (POO)

```
Usuario        → nome, senha, pontos, historico (Pilha<Entrega>), beneficiosResgatados (Pilha)
Entrega        → material, quantidade, pontos, data
Benefício      → nome, custoEmPontos
Pilha<T>       → push / pop / peek / isEmpty  (estrutura de dados implementada do zero)
GerenciadorUsuarios → autenticação e controle de sessão
```

---

## Equipe

| Nome | GitHub |
|------|--------|
| Carlos Henrique Saran Pappa | [he-nz](https://github.com/he-nz) |
| Fellipe Miquelão Schmidt | [Fximis](https://github.com/Fximis) |
| Lucas Thomaz Brandel Zequini | [lucastbzequini](https://github.com/lucastbzequini)  |

---

**Universidade Cesumar — UNICESUMAR · ADS · 3º Semestre · 2026.2**
