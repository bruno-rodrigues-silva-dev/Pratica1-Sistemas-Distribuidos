# Prática 1 – Sistemas Distribuídos

**Disciplina:** Plataformas e Sistemas de Alto Desempenho  
**Aluno:** Bruno Rodrigues da Silva  
**Matrícula:** 1220303287  
**Professora:** Ana Paula Faragó  
**Instituição:** Universidade Veiga de Almeida (UVA)  
**Ano:** 2026

## 1. Descrição do projeto

Este projeto apresenta uma simulação de um sistema distribuído desenvolvida em Python e executada no Google Colab.

A implementação utiliza um servidor coordenador e três clientes, que se comunicam por meio de Sockets TCP. O servidor distribui tarefas, recebe os resultados individuais, calcula o resultado global e realiza a sincronização das informações.

Também foi implementado um mecanismo de monitoramento por mensagens PING e PONG, com simulação de ausência de resposta de um dos clientes e identificação por timeout.

## 2. Tecnologias e recursos utilizados

- Python
- Google Colab
- Sockets TCP
- Threading
- JSON
- Mensagens ACK
- Monitoramento PING/PONG
- Timeout

## 3. Resultado da simulação

Os três clientes processaram seus respectivos conjuntos de números:

| Cliente | Resultado |
|---|---:|
| Cliente 1 | 6 |
| Cliente 2 | 15 |
| Cliente 3 | 24 |
| **Resultado global** | **45** |

Durante o monitoramento, o Cliente 3 deixou de enviar a resposta PONG, permitindo que o servidor identificasse a ausência de resposta após o tempo limite estabelecido.

## 4. Acesso ao projeto

**Google Colab:**  
https://colab.research.google.com/drive/1jI-PZLAeFvgMDcziBam53aNYq_AjFT4_#scrollTo=oVlhC5CVeN2N

**Documento da atividade:** disponível neste repositório em formato PDF.

**Código-fonte:** disponibilizado neste repositório em formato Jupyter Notebook (`.ipynb`).

## 5. Objetivo

Aplicar conceitos fundamentais de sistemas distribuídos, incluindo comunicação entre processos, distribuição de tarefas, sincronização de informações, execução concorrente e detecção de falhas.
