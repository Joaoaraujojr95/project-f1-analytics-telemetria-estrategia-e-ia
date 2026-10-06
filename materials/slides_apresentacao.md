# 📊 Roteiro de Slides: Ciência de Dados a 350 km/h

Apresentação executiva e técnica elaborada a partir das fontes do Segundo Cérebro no NotebookLM e do estudo de caso do GP da Malásia (Sepang).

---

### Slide 1: Título e Abertura
* **Título:** Ciência de Dados a 350 km/h: Como a IA Decide Corridas e Projeta Campeões
* **Subtítulo:** Telemetria em Tempo Real, Janelas Climáticas, Estratégia de Box e Modelagem Estocástica no Motorsport
* **Apresentador:** Especialista em Telemetria & Estratégia de F1
* **Mensagem-chave:** Na Fórmula 1 moderna, o piloto aperta os pedais, mas é a convergência de dados e algoritmos que vence a corrida.

---

### Slide 2: A Mina de Ouro da Telemetria (300 Sensores & Nuvem)
* **Infraestrutura:** Cada carro possui cerca de 300 sensores gerando mais de 1,1 milhão de pontos de dados por segundo.
* **Variáveis Transmitidas:**
  * Velocidade, abertura de acelerador e pressão de freio;
  * RPM, marcha e forças G longitudinais/laterais;
  * Dados térmicos e de deslizamento de pneus (*micro-slip*).
* **AWS F1 Insights:** Integração contínua da telemetria ao vivo com mais de 70 anos de histórico de corridas.

---

### Slide 3: Cálculo de Probabilidade de Vitória Volta a Volta
* **Além da Posição Física:** Estar em 1º lugar não garante a vitória.
* **Os Quatro Pilares Preditivos:**
  1. *Ritmo e Tempos de Setor:* S1, S2, S3 e *gap to leader*;
  2. *Degradação dos Pneus:* Estimativa da energia de desgaste e vida útil do composto;
  3. *Pit Window e Tráfego:* Simulação da perda no pit lane e janela de reentrada limpa;
  4. *Battle Forecast:* Previsão matemática de quando o perseguidor entrará em zona de ataque.

---

### Slide 4: O Caos Climático e o "Crossover Point" (Estudo de Caso: Sepang)
* **A Linha Tênue da Chuva:** A transição entre pista seca e molhada é o maior gerador de volatilidade.
* **O Risco da Janela de Transição:**
  * Slicks em pista úmida: perda de aderência instantânea e prejuízo de mais de um pit stop em duas voltas.
  * Intermediários em piso seco: superaquecimento e destruição acelerada da borracha.
* **Detecção por Dados:** Quando os setores S1, S2 e S3 do primeiro rival com o composto oposto superam o ritmo atual, a IA aponta a abertura imediata da janela de box.

---

### Slide 5: Xadrez Estratégico: Mercedes vs. Ferrari
* **Análise Comparativa de Stints no GP:**

| Piloto | Equipe | Estratégia de Compostos | Desfecho |
|---|---|---|---|
| **Kimi Antonelli** | Mercedes | Intermediário (9v) $\rightarrow$ Médio (24v) $\rightarrow$ Macio (11v) $\rightarrow$ Macio (11v) | **P2** (Consistência e controle) |
| **George Russell** | Mercedes | Intermediário (9v) $\rightarrow$ Macio (23v) $\rightarrow$ Macio (12v) $\rightarrow$ Macio (6v) | **DNF** (Quebra de motor perto do fim) |
| **Lewis Hamilton** | Ferrari | Macio (31v) $\rightarrow$ Médio (12v) $\rightarrow$ Macio (12v) | **P3** (Pódio após largar do fundo com Safety Car) |
| **Charles Leclerc** | Ferrari | Intermediário (6v) $\rightarrow$ Macio (19v) $\rightarrow$ Duro (15v) $\rightarrow$ Macio (12v) | **P4** (Erro tático assumido pelo uso do pneu duro) |

---

### Slide 6: O Fator Acaso e a "Parada Grátis"
* **Eventos Estocásticos:**
  * Toques em pista (Bortoleto vs. Sainz) e quebras de motor (Russell);
  * Panes de software na unidade de potência na volta de formação.
* **A Matemática do Safety Car:**
  * Neutraliza o ritmo e agrupa o grid (*gap to leader*);
  * A perda de tempo no pit lane cai drasticamente (carros na pista sob delta obrigatório);
  * Hamilton utilizou o Safety Car para recuperar mais de 1 pit stop de desvantagem e saltar ao pódio.

---

### Slide 7: Projeções do Campeonato Mundial: Antonelli Rumo ao Título
* **Mundial de Pilotos (Pós-Sepang):**
  * **1º Andrea Kimi Antonelli (Mercedes):** **320 pontos** (Vantagem massiva de **84 pontos** — mais de 3 vitórias de margem);
  * **2º George Russell (Mercedes):** **236 pontos** (Título matematicamente "muito difícil e improvável" após DNF);
  * **Pelotão Perseguidor:** Hamilton (**214 pts**), Leclerc (**191 pts**), Verstappen (**188 pts**), Norris (**188 pts**).
* **Mundial de Construtores:**
  * **Mercedes:** 556 pontos (Dominância isolada);
  * **Ferrari:** 405 pontos;
  * **McLaren:** 316 pontos;
  * **Red Bull:** 298 pontos.

---

### Slide 8: Conclusão
* **A Síntese:** A Fórmula 1 é o laboratório supremo de Big Data em tempo real.
* **As Três Lições:**
  1. A telemetria contínua normaliza fatores invisíveis aos olhos do espectador;
  2. O clima premia quem decide pelo *crossover point* baseado em setores, e não na intuição;
  3. O acaso é mitigado por Simulações de Monte Carlo que orientam as equipes sob bandeiras amarelas.
