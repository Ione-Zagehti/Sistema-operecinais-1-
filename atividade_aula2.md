
# Resumo – Capítulos 1 a 13  
**Sistemas Operacionais Modernos – Andrew S. Tanenbaum & Herbert Bos**

---

## 📘 Capítulo 1 – Introdução

Apresenta o conceito de sistema operacional (SO) sob duas perspectivas:

- **Máquina estendida**: abstrai o hardware complexo e fornece interfaces simples.
- **Gerenciador de recursos**: administra CPU, memória, discos e dispositivos de E/S.

### Principais tópicos:
- Evolução histórica dos sistemas operacionais
- Revisão de hardware (CPU, memória, discos, barramentos)
- Tipos de SO (servidores, embarcados, tempo real, multiprocessadores)
- Conceitos fundamentais:
  - Processos
  - Espaço de endereçamento
  - Arquivos
  - Proteção
  - Shell
- Chamadas de sistema
- Estruturas de SO:
  - Monolítico
  - Em camadas
  - Micronúcleo
  - Máquinas virtuais
  - Exonúcleo

---

## 📘 Capítulo 2 – Processos e Threads

Foco na execução concorrente.

### Processos:
- Modelo de processo
- Estados (novo, pronto, executando, bloqueado)
- Criação e término
- Hierarquia de processos

### Threads:
- Conceito e vantagens
- Threads em nível usuário e nível núcleo
- Implementações híbridas

### Comunicação e sincronização:
- Condições de corrida
- Região crítica
- Exclusão mútua
- Semáforos
- Mutex
- Monitores
- Troca de mensagens
- Barreiras

### Escalonamento:
- Sistemas em lote
- Interativos
- Tempo real

### Problemas clássicos:
- Jantar dos filósofos
- Leitores e escritores

---

## 📘 Capítulo 3 – Gerenciamento de Memória

Estuda como a memória principal é organizada e protegida.

### Conceitos:
- Espaço de endereçamento
- Swapping
- Memória virtual

### Paginação:
- Tabelas de páginas
- TLB
- Paginação multinível

### Substituição de páginas:
- Ótimo
- FIFO
- NRU
- LRU
- Relógio
- WSClock

### Segmentação:
- Segmentação pura
- Segmentação com paginação

### Questões de projeto:
- Alocação local vs global
- Tamanho da página
- Páginas compartilhadas
- Arquivos mapeados

---

## 📘 Capítulo 4 – Sistemas de Arquivos

Define como os dados são organizados em armazenamento secundário.

### Arquivos:
- Estrutura
- Tipos
- Atributos
- Operações

### Diretórios:
- Hierárquicos
- Caminhos absolutos e relativos

### Implementação:
- Blocos
- i-nodes
- Sistemas journaling
- Sistemas virtuais de arquivos

### Gerenciamento:
- Espaço em disco
- Consistência
- Backups
- Desempenho

### Exemplos:
- MS-DOS
- UNIX

---

## 📘 Capítulo 5 – Entrada/Saída (E/S)

Explica como o SO interage com dispositivos.

### Hardware:
- Controladores
- E/S mapeada em memória
- DMA
- Interrupções

### Software:
- Drivers
- Camadas de E/S
- Software independente de dispositivo

### Discos:
- Escalonamento (SSTF, SCAN, etc.)
- Tratamento de erros
- Armazenamento estável

### Outros tópicos:
- Relógios
- Interfaces (teclado, mouse, monitor)
- Gerenciamento de energia
- Thin clients

---

## 📘 Capítulo 6 – Impasses (Deadlocks)

Analisa bloqueios permanentes entre processos.

### Condições para deadlock:
1. Exclusão mútua
2. Posse e espera
3. Não preempção
4. Espera circular

### Estratégias:
- Ignorar (algoritmo do avestruz)
- Detecção e recuperação
- Evitação (Algoritmo do Banqueiro)
- Prevenção

### Outros problemas:
- Livelock
- Inanição

---

## 📘 Capítulo 7 – Virtualização e Nuvem

Capítulo novo na 4ª edição.

### Virtualização:
- Hipervisores tipo 1 e tipo 2
- Virtualização de CPU, memória e E/S
- Custos da virtualização

### Nuvem:
- Computação como serviço
- Migração de máquinas virtuais
- Checkpointing

### Estudo de caso:
- VMware

---

## 📘 Capítulo 8 – Sistemas com Múltiplos Processadores

Foco em paralelismo e sistemas distribuídos.

### Multiprocessadores:
- SMP
- Consistência de cache
- Escalonamento multiprocessado

### Multicomputadores:
- Comunicação
- RPC
- Memória distribuída

### Sistemas distribuídos:
- Middleware
- Protocolos de rede
- Balanceamento de carga

---

## 📘 Capítulo 9 – Segurança

Aborda proteção contra ameaças.

### Conceitos:
- Ameaças e atacantes
- Base computacional confiável

### Controle de acesso:
- Domínios
- ACLs
- Capacidades

### Criptografia:
- Chave secreta
- Chave pública
- Assinaturas digitais

### Vulnerabilidades:
- Buffer overflow
- Ponteiros nulos
- Injeção de comando

### Malware:
- Cavalo de Troia
- Vírus
- Worms
- Spyware
- Rootkits

### Defesas:
- Firewalls
- Antivírus
- Encapsulamento
- Detecção de intrusão

---

## 📘 Capítulo 10 – Estudo de Caso 1: UNIX, Linux e Android

### História:
- UNIX
- MINIX
- Linux

### Linux:
- Processos
- Escalonamento
- Memória
- E/S
- Sistema de arquivos
- Segurança

### Android:
- Arquitetura
- Dalvik
- Binder IPC
- Modelo de aplicações
- Segurança e sandbox

---

## 📘 Capítulo 11 – Estudo de Caso 2: Windows 8

### Estrutura:
- Kernel NT
- Subsistemas
- DLLs

### Processos e threads
### Gerenciamento de memória
### Caching
### E/S
### Sistema de arquivos NTFS
### Segurança
### Gerenciamento de energia

---

## 📘 Capítulo 12 – Projeto de Sistemas Operacionais

Discute decisões de engenharia.

### Projeto:
- Interface
- Separação política vs mecanismo
- Ortogonalidade
- Binding time

### DesempenhoN:
- Localidade
- Uso de cache
- Otimização do caso comum

### Gerenciamento de projeto:
- Estrutura de equipe
- Experiência
- Complexidade

### Tendências:
- Nuvem
- Multinúcleo
- Sistemas embarcados
- Grandes espaços de endereçamento

---

## 📘 Capítulo 13 – Sugestões de Leitura e Referências

Inclui:
- Leituras clássicas e introdutórias
- Referências por área:
  - Processos
  - Memória
  - Arquivos
  - Segurança
  - Virtualização
  - Windows
  - Linux
- Referências atualizadas da 4ª edição

---

# 📌 Visão Geral da Obra

O livro cobre:

- Fundamentos teóricos
- Implementações práticas
- Estudos de caso reais
- Segurança e virtualização modernas
- Projeto e tendências futuras

É uma referência completa para cursos de Sistemas Operacionais em Ciência e Engenharia da Computação.
