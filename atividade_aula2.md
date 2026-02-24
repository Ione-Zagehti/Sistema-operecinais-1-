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
Sistema Operacional (SO)
→ Interface entre usuário e hardware
→ Gerencia recursos

Funções principais:

Processos

Memória

Arquivos

Entrada/Saída

Tipos de sistemas:

Batch

Tempo compartilhado

Tempo real

Distribuídos

Embarcados
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
Processo
→ Programa em execução
→ Estados (novo, pronto, executando, bloqueado)

Threads
→ Execução dentro do processo
→ Compartilham memória

Escalonamento:

FCFS

SJF

Round Robin

Problemas:

Condição de corrida

Região crítica
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

Processo
→ Programa em execução
→ Estados (novo, pronto, executando, bloqueado)

Threads
→ Execução dentro do processo
→ Compartilham memória

Escalonamento:

FCFS

SJF

Round Robin

Problemas:

Condição de corrida

Região crítica
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

Arquivos:
→ Organização de dados

Estrutura:

Diretórios

Inodes

Métodos de alocação:

Contígua

Encadeada

Indexada

Segurança:

Permissões

Controle de acesso
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
Funcionamento do hardware de E/S (dispositivos, controladores, DMA e interrupções).

Estrutura em camadas do software de E/S:

Tratadores de interrupção

Drivers de dispositivos

Software independente de dispositivo

Discos: estrutura física, formatação e algoritmos de escalonamento.

Relógios e temporizadores.

Interfaces com o usuário (teclado, mouse, monitor).

Gerenciamento de energia.

👉 Objetivo: organizar e otimizar o uso dos dispositivos físicos.
### Discos:
- Escalonamento (SSTF, SCAN, etc.)
- Tratamento de erros
- Armazenamento estável

### Outros tópicos:
- Relógios
- Interfaces (teclado, mouse, monitor)
- Gerenciamento de energia
- Thin clients
Hardware:
→ Dispositivos
→ Controladores
→ Interrupções

Software:

Drivers

Sistema independente de dispositivo

Discos:

Estrutura física

Escalonamento (SCAN, C-SCAN)
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

👉 Ensina como lidar com bloqueios em sistemas concorrentes.
Condições:

Exclusão mútua

Posse e espera

Não preempção

Espera circular

Soluções:

Ignorar

Detectar

Evitar (Algoritmo do Banqueiro)

Prevenir
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
Temas abordados:

Conceito de máquina virtual.

Hipervisores tipo 1 e tipo 2.

Virtualização de CPU, memória e E/S.

Computação em nuvem (serviços, migração de máquinas virtuais).

Estudo de caso: VMware.

👉 Mostra como um mesmo hardware pode executar vários sistemas operacionais simultaneamente.
---
Virtualização:
→ Máquina virtual
→ Hipervisor (tipo 1 e 2)

Nuvem:
→ IaaS
→ PaaS
→ SaaS

Migração de máquinas virtuais

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

- Conteúdos principais:

Multiprocessadores e multinúcleos.

Sincronização e escalonamento em múltiplas CPUs.

Multicomputadores.

Sistemas distribuídos.

Balanceamento de carga.

👉 Importante para entender computadores modernos com vários núcleos.

Multiprocessadores:
→ Multicore
→ SMP

Problemas:

Sincronização

Balanceamento de carga

Sistemas distribuídos
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
Principais tópicos:

Ameaças e atacantes.

Controle de acesso (ACLs e capacidades).

Modelos de segurança.

Criptografia básica.

Autenticação.

Malware (vírus, worms, spyware, rootkits).

Técnicas de defesa (firewall, antivírus, bit NX, randomização de memória).
Ameaças:
→ Malware
→ Ataques

Proteção:

Criptografia

Autenticação

Controle de acesso

Defesas:

Firewall

Bit NX

Randomização de memória

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

Analisa sistemas reais.

História do UNIX e do Linux.

Estrutura do Linux.

Processos, memória, E/S e sistema de arquivos no Linux.

Segurança no Linux.

Arquitetura do Android.

👉 Mostra como os conceitos teóricos são aplicados na prática.
História do UNIX
Estrutura do Linux
Processos no Linux
Sistema de arquivos
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
Analisa o Windows 8.1.

Estrutura do sistema.

Processos e threads.

Gerenciamento de memória.

Sistema de arquivos NTFS.

Segurança no Windows.

👉 Comparação prática com o Linux.

Estrutura interna
Gerência de memória
Sistema de arquivos NTFS
Segurança
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
Dificuldades do projeto.

Interface e implementação.

Política vs mecanismo.

Desempenho e otimização.

Gerenciamento de equipe.

Tendências (nuvem, multicore, dispositivos móveis).

Política × Mecanismo
Desempenho
Confiabilidade
Tendências (nuvem, mobile, multicore)
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
Leituras adicionais por tema.

Artigos acadêmicos importantes.

Referências atualizadas.

👉 Serve como base para aprofundamento e pesquisa.

Artigos importantes
Pesquisas acadêmicas
Evolução da área
---

# 📌 Visão Geral da Obra

O livro cobre:

- Fundamentos teóricos
- Implementações práticas
- Estudos de caso reais
- Segurança e virtualização modernas
- Projeto e tendências futuras

É uma referência completa para cursos de Sistemas Operacionais em Ciência e Engenharia da Computação.
