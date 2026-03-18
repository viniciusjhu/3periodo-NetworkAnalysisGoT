# Análise de Redes em "A Song of Ice and Fire" (Game of Thrones)

Este repositório contém o projeto de análise de grafos (Trabalho Prático 03) desenvolvido para a disciplina de Algoritmos e Estruturas de Dados III. O objetivo principal do projeto é aplicar conceitos da Teoria dos Grafos para analisar as interações entre os personagens centrais da aclamada série literária de George R. R. Martin.

## 🎯 Objetivos

- **Modelagem de Dados Literários:** Transformar as menções e interações entre personagens em uma estrutura de dados de grafos.
- **Análise de Conectividade:** Identificar e quantificar os Componentes Conexos do grafo formado pelas relações interpessoais.
- **Estimação de Complexidade da Rede:** Calcular o *Circuit Rank* (Posto de Ciclomático) para entender o nível de ciclos e conexões redundantes ou complexas na rede de personagens.
- **Estruturas de Grafos:** Implementar manipulação de grafos pesados diretos e indiretos usando Matrizes de Adjacência em C.

## 🛠️ Stack Tecnológica

- **Linguagem C:** Linguagem utilizada para o desenvolvimento completo da lógica de leitura, estruturação em memória e cálculos sobre os grafos.
- **Makefile:** Sistema de build otimizado (`-O3`) para facilidade na compilação e gestão do projeto estruturado em múltiplos arquivos (`.c` e `.h`).
- **Git/GitHub:** Controle de versão e versionamento.

## ⚙️ Funcionalidades e Estrutura

- `main.c`: Orquestra todo a execução, iterando pela coleção de 5 diferentes livros da série principal.
- `leitura.c`/`.h`: Executa o parse (leitura e decodificação) dos dados a partir de arquivos externos e contabiliza as arestas.
- `grafo.c`/`.h`: Responsável pela alocação dinâmica, inicialização, inserção e cálculos no grafo, incluindo a sua manipulação em forma indirecionada / bidirecional ("inverter arestas").
- `componentes_conexos.c`/`.h`: Conta os componentes isolados via uma implementação robusta em grafos densos.
- `lista.c`/`.h`: Estrutura de dados complementar base de suporte para algoritmos de passeios no grafo.

A execução do software emite uma matriz formatada que relaciona as menções entre protagonistas (como Arya, Jon, Tyrion, Cersei etc.), computando então o número total de componentes conexos da rede e o seu *Circuit Rank*.

## 👨‍💻 Autores
Trabalho feito em colaboração como requisito acadêmico.
Desenvolvido por:
- Davi Azarias
- Renan Catini
- João Antônio Siqueira
- João Antônio Lassister
- *Vinícius Ribeiro
