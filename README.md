# Relatório de Experimentos - Programação em Tempo Real

Este repositório contém os relatórios e evidências da execução de 10 experimentos práticos focados nos conceitos fundamentais de **Sistemas de Tempo Real (STR)**. Os testes foram realizados simulando cenários de escalonamento, sincronização, compartilhamento de recursos e tratamento de falhas.

---

## 👤 Autor e Instituição
* **Aluno:** Leonardo Gabriel Santos Santana
* **Instituição:** Afya – Montes Claros
* **Curso/Disciplina:** Programação em Tempo Real

---

## 📁 Estrutura de Arquivos no Repositório
* `PRINT DOS RESULTADOS.pdf`: Documento consolidado contendo as capturas de tela das execuções dos scripts.
* `PROGRAMAÇÃO EM TEMPO REAL_experimentos.pdf`: Relatório final estruturado em formato PDF com os objetivos, procedimentos e conclusões.
* `PROGRAMAÇÃO EM TEMPO REAL_experimentos.docx`: Versão editável em Word do relatório final de experimentos.

---

## 🔬 Resumo dos 10 Experimentos Executados

### 1. Produtor-Consumidor e Fila (`04_queue_producer_consumer.py`)
* **Objetivo:** Analisar o comportamento de uma fila compartilhada entre processos produtores e consumidores para desacoplar a produção de dados e reduzir perdas.

### 2. Bloqueio por Mutex (`05_mutex_blocking_latency.py`)
* **Objetivo:** Avaliar o impacto da exclusão mútua (Mutex) na latência de acesso a recursos compartilhados quando há concorrência de tarefas.

### 3. Inversão de Prioridade (`06_priority_inversion_simulated.py`)
* **Objetivo:** Demonstrar visualmente o fenômeno em que uma tarefa de alta prioridade fica bloqueada aguardando um recurso retido por uma tarefa de baixa prioridade.

### 4. Escalonamento Rate Monotonic - RM (`07_rate_monotonic_sim.py`)
* **Objetivo:** Estudar o comportamento determinístico e previsível do algoritmo clássico de prioridade estática (RM), onde tarefas de menor período ganham maior prioridade.

### 5. Escalonamento Earliest Deadline First - EDF (`08_edf_sim.py`)
* **Objetivo:** Analisar a dinâmica do algoritmo de prioridade dinâmica EDF, priorizando tarefas mais próximas de estourar o prazo (*deadline*).

### 6. Simulação de Watchdog (`09_watchdog_simulated.py`)
* **Objetivo:** Avaliar o uso de temporizadores de monitoramento (*watchdog*) na detecção automática de travamentos e execução do reset do sistema.

### 7. Malha de Controle Periódica (`10_control_loop_fixed_period.py`)
* **Objetivo:** Investigar uma malha de controle de período fixo e validar como o erro e a estabilidade dependem diretamente do rigor temporal da periodicidade.

### 8. Interpretação de Diagrama de Gantt
* **Objetivo:** Mapear e interpretar a linha do tempo da CPU, visualizando liberações, execuções e prazos para facilitar a análise temporal do sistema.

### 9. Efeito de Offsets e Fase Inicial (`offsets_sim.py`)
* **Objetivo:** Observar como a inserção de deslocamentos iniciais (*offsets*) redistribui a carga de tarefas ao longo do tempo sem alterar a utilização total do processador.

### 10. Conjuntos Harmônicos vs. Não Harmônicos (`harmonic_vs_nonharmonic.py`)
* **Objetivo:** Comparar o comportamento de escalonamento entre conjuntos de tarefas periódicas múltiplas entre si (harmônicos) e conjuntos com períodos arbitrários, validando a previsibilidade dos harmônicos.

---

## 🎯 Conclusão Geral
A execução prática dos cenários simulados comprovou que em Sistemas de Tempo Real o cumprimento rigoroso dos requisitos de tempo e o planejamento do escalonamento são fundamentais para assegurar a **previsibilidade**, a **confiabilidade** e a **segurança** das aplicações.
