## Problema de Máxima Cobertura com BRKGA

Este projeto implementa uma abordagem heurística baseada no **BRKGA (Biased Random-Key Genetic Algorithm)** para resolver uma variante do **Problema de Máxima Cobertura (MCP)**, inspirado no Problema de Cobertura de Conjuntos (Set Covering Problem – SCP).

A solução foi desenvolvida em **Python**, utilizando a biblioteca [brkga\_mp\_ipr](https://github.com/ceandrade/brkga_mp_ipr), e validada com instâncias do artigo de **Prata (2012)**.

Link para a pasta contendo o artigo oficial, testes realizados, código e instâncias utilizadas no traballho: https://drive.google.com/drive/folders/1l4fLf02aWAH6EsXGMY28ra6rTHw-FVSB?usp=sharing
---

## 📌 Objetivo

Selecionar um subconjunto limitado de colunas de uma matriz binária de forma a **maximizar a cobertura de linhas**.
Enquanto a Programação Linear Inteira (PLI) encontra soluções exatas, este projeto explora o **BRKGA** como alternativa para obter boas soluções em menos tempo, especialmente em instâncias maiores.

---

## ⚙️ Tecnologias utilizadas

* **Python**
* **Google Colab** (ambiente de desenvolvimento)
* **Bibliotecas**:

  * `brkga_mp_ipr` (implementação oficial do BRKGA)
  * `numpy` (manipulação de matrizes)
  * `os`, `importlib.util` (carregamento de instâncias `.py`)
  * `time` (medição de execução)

---

## 🚀 Como executar

1. Clone este repositório:

   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   ```
2. Instale as dependências:

   ```bash
   pip install numpy
   pip install brkga_mp_ipr
   ```
3. Adicione as instâncias do problema (arquivos `.py`) na pasta indicada.
4. Execute o algoritmo principal:

   ```bash
   python main.py
   ```
5. O programa irá:

   * Ler automaticamente as instâncias.
   * Aplicar o BRKGA.
   * Reportar: subconjuntos escolhidos, linhas cobertas/não cobertas, tempo de execução e valor da função objetivo.

---

## 📊 Resultados

* O **BRKGA** apresentou **tempos de execução entre 15 e 20 segundos**, muito menores do que a solução via **Programação Linear Inteira (PLI)**.
* Em termos de qualidade, o BRKGA apresentou **pequena perda de cobertura**, mas manteve consistência entre diferentes execuções.
* É mais adequado para **instâncias maiores** e cenários onde **tempo de execução é restritivo**.

---

## 🖥️ Ambiente de testes

* **Máquina 1**: AMD Ryzen 5 PRO 2400GE, 8GB RAM, Windows 10 Pro, SSD 240GB
* **Máquina 2**: AMD Ryzen 5 5500, 16GB RAM, Windows 11 Pro, SSD 480GB

---

## 📚 Referências

* PRATA, Bruno de Athayde. *Um algoritmo enxame de partículas para uma variante do problema de máxima cobertura.* GEPROS, v. 7, n. 2, p. 139–148, 2012.
* [BRKGA-MP-IPR GitHub Repository](https://github.com/ceandrade/brkga_mp_ipr)

---

## 👥 Autores

* **Gustavo Henrique Sargi Michelim** – Universidade Estadual de Maringá (UEM)
* **Henrique Rosa de Araújo** – Universidade Estadual de Maringá (UEM)

---

Quer que eu também monte um **exemplo de seção de resultados com gráficos (tempo x qualidade)** no README para ficar mais ilustrativo no GitHub?
