# 📖 Guia de Estudos & Quiz: Telemetria e Estratégia de F1

Este guia sintetiza os conceitos de **Ciência de Dados e Inteligência Artificial aplicada à Fórmula 1**, consolidando a telemetria em tempo real, as ferramentas preditivas da AWS e o estudo de caso do GP da Malásia (Sepang).

---

## 🎯 Roteiro de Aprendizagem de Motorsport Analytics

```
[1. Coleta de Telemetria (300 Sensores & 1,1M pts/s)] 
                     ⬇️
[2. Modelos Preditivos de Corrida (AWS Track Pulse & Battle Forecast)] 
                     ⬇️
[3. Janela de Pistas Molhadas (Crossover Point & Live Timing S1/S2/S3)] 
                     ⬇️
[4. Modelagem do Acaso (Safety Car, Falhas RCA & Simulação de Monte Carlo)] 
                     ⬇️
[5. Projeção de Título Mundial (Evolução de Antonelli, Russell e Construtores)]
```

---

## 📌 Glossário Técnico Especializado

| Termo | Definição Técnica |
|---|---|
| **Telemetria de Alta Frequência** | Conjunto de dados capturados por cerca de 300 sensores por carro (1,1 milhão de pontos/segundo) cobrindo acelerador, freio, forças G, RPM, marcha e deslizamento. |
| **Track Pulse & Battle Forecast** | Algoritmos de Machine Learning e IA generativa da AWS F1 Insights que cruzam dados ao vivo com 70 anos de histórico para antecipar ultrapassagens e ritmo de prova. |
| **Crossover Point** | Ponto de inflexão em que a pista seca o bastante para justificar pneus slicks ou molha o suficiente para exigir compostos intermediários ou de chuva extrema. |
| **Pit Window & Pit Lane Performance** | Janela temporal calculada por IA que simula a perda de tempo na reta dos boxes e mapeia a reentrada do piloto na pista para evitar tráfego e ar sujo. |
| **Undercut** | Antecipação da parada em 1 ou 2 voltas para calçar pneus novos e ganhar vantagem na volta de saída (*out-lap*) contra o adversário na pista. |
| **Overcut** | Postergação da parada para andar em ar limpo e abrir vantagem enquanto o adversário enfrenta dificuldades para aquecer os pneus novos. |
| **Root Cause Analysis (RCA)** | Algoritmos preditivos de IA que leem dados térmicos e de pressão para detectar anomalias e prever quebras mecânicas antes da falha total. |
| **Simulação de Monte Carlo** | Modelo estocástico que executa milhares de iterações por segundo para calcular probabilidades de Safety Car e desfechos de campeonato. |

---

## 📝 Quiz de Fixação

Teste seus conhecimentos baseando-se nas respostas oficiais do Gemini Notebook:

### Questão 1
Quantos pontos de dados de telemetria por segundo são gerados, em média, pelos aproximadamente 300 sensores instalados em um carro de Fórmula 1 moderno?
* A) Cerca de 10.000 pontos por segundo.
* B) Mais de 1,1 milhão de pontos de dados por segundo.
* C) Apenas 60 pontos por minuto, via satélite comercial.
* D) 500 pontos a cada volta completada.

---

### Questão 2
No Grande Prêmio de Sepang, por que os pilotos que apostaram precocemente em pneus slicks (secos) com o asfalto ainda úmido perderam mais de um pit stop de vantagem em apenas duas voltas?
* A) Porque foram penalizados pelos comissários da FIA por excesso de velocidade.
* B) Porque os pneus slicks não conseguem escoar a água, zerando a aderência antes de atingir o verdadeiro *Crossover Point*.
* C) Porque o motor foi desligado automaticamente pelo sistema de telemetria.
* D) Porque os pneus slicks explodiram devido à baixa temperatura da pista.

---

### Questão 3
Como a entrada do Safety Car durante a prova beneficiou a estratégia de Lewis Hamilton (Ferrari), que havia largado do fundo do grid e feito um primeiro stint de 31 voltas com pneus macios?
* A) O Safety Car permitiu que Hamilton fizesse uma "parada grátis" com perda relativa reduzida e agrupou o grid (*gap to leader*), viabilizando sua subida até o pódio (3º lugar).
* B) O Safety Car obrigou todos os carros à sua frente a abandonarem a corrida.
* C) O Safety Car concedeu 25 pontos extras diretamente ao piloto da Ferrari.
* D) A direção de prova cancelou os tempos de volta de todos os rivais da Mercedes.

---

### Questão 4
Por que a quebra de motor sofrida por George Russell em Sepang teve um impacto matemático quase irreversível nas simulações de título mundial?
* A) Porque a Mercedes foi desclassificada do Mundial de Construtores.
* B) Porque a vantagem do líder Andrea Kimi Antonelli subiu para 84 pontos, o que equivale a mais de três vitórias de folga com poucas etapas restantes.
* C) Porque Russell perdeu sua superlicença da FIA para a temporada seguinte.
* D) Porque o regulamento proíbe que um vice-líder vença corridas após sofrer um abandono.

---

### Questão 5
Qual foi a principal divergência tática admitida pela Ferrari no terceiro stint de Charles Leclerc em relação aos pilotos da frente?
* A) Leclerc colocou pneus de chuva extrema no asfalto completamente seco.
* B) A Ferrari optou pelo composto Duro (15 voltas) — sendo a única entre os quatro primeiros a usá-lo —, admitindo ter ficado no lado errado do planejamento tático.
* C) Leclerc parou quatro vezes a mais que todos os outros competidores.
* D) A Ferrari não trocou os pneus e fez o piloto correr sem rodas na reta final.

---

## 🔑 Gabarito Comentado

* **Questão 1: Alternativa B.**  
  *Explicação:* Conforme destacado na resposta do Gemini LM `[1]`, `[3]`, cada carro possui cerca de 300 sensores gerando mais de 1,1 milhão de pontos de telemetria por segundo transmitidos em tempo real.
* **Questão 2: Alternativa B.**  
  *Explicação:* Colocar slicks antes do *Crossover Point* em asfalto úmido elimina a aderência, provocando tempos de volta catastróficos que anulam qualquer ganho teórico de pit stop `[2]`, `[4]`.
* **Questão 3: Alternativa A.**  
  *Explicação:* A neutralização agrupa o pelotão e reduz o tempo perdido em pit stop, permitindo a Hamilton converter seu longo stint de macios em uma escalada até o 3º lugar no pódio `[9]`, `[10]`.
* **Questão 4: Alternativa B.**  
  *Explicação:* Como uma vitória concede 25 pontos, a distância de 84 pontos para Antonelli exige que Russell vença corridas consecutivas e que o líder zere pontuações repetidamente, tornando o título estatisticamente improvável `[6]`, `[7]`, `[11]`.
* **Questão 5: Alternativa B.**  
  *Explicação:* Enquanto Antonelli, Russell e Hamilton utilizaram combinações de compostos médios e macios, Leclerc foi o único a calçar pneus duros no 3º stint, terminando em 4º lugar `[2]`, `[4]`.
