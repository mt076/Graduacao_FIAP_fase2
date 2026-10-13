# 🚀 MGPEB - Missão Aurora Siger (Fase 2)

<img width="3584" height="1184" alt="Gemini_Generated_Image_cz84nucz84nucz84" src="https://github.com/user-attachments/assets/5778249c-ca35-405b-9a7e-72bed090b5df" />

![FIAP](https://img.shields.io/badge/FIAP-Ci%C3%AAncia_da_Computa%C3%A7%C3%A3o-ED145B?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)

## 📌 Sobre o Projeto
Este repositório contém o **Módulo de Gerenciamento de Pouso e Estabilização de Base (MGPEB)**, desenvolvido como Atividade Integradora para o curso de Ciência da Computação (FIAP). O objetivo do sistema é orquestrar, de forma autônoma e segura, a descida de módulos logísticos e tripulados na colônia marciana Aurora Siger.

Diferente do processamento *hardcoded* e limitado da era Apollo 11 (cujo AGC possuía apenas 4KB de RAM), este projeto utiliza a linguagem Python para alocação dinâmica de memória, permitindo processar a telemetria espacial em tempo real, respeitando rigorosos protocolos lógicos e legislações interplanetárias (ESG).

## ⚙️ Arquitetura e Estruturas de Dados
O motor de decisão foi construído sem o uso de frameworks complexos, focando no domínio de fundamentos de Ciência da Computação:

*   **Filas (Queues - FIFO):** Processamento da ordem de autorização dos módulos em órbita aguardando janela de pouso.
*   **Pilhas (Stacks - LIFO):** Implementação da "Câmara de Ar" para o sistema de Aborto de Emergência. Módulos ameaçados por anomalias (ex: clima) são revertidos seguindo a lógica do último a entrar, primeiro a sair.
*   **Listas e Dicionários:** Mapeamento dinâmico e organização de dicionários complexos com as características de cada módulo (Massa, Tripulação, Combustível, Bateria, Status).

## 🧮 Algoritmos e Lógica Computacional
*   **Busca Linear $O(n)$:** Algoritmo implementado para auditar o status atualizado de qualquer módulo orbitando ou já estabilizado em solo.
*   **Bubble Sort $O(n^2)$:** Ordenação de criticidade aplicada aos módulos pousados para priorização de reabastecimento imediato.
*   **Álgebra Booleana:** A árvore de decisões do motor em Python foi otimizada via absorção lógica, resultando no circuito determinístico de autorização de pouso ($Z$):
    $$Z = B \cdot (\neg T + C)$$
    *(O Pouso só ocorre se houver Bateria Segura **E** [o módulo for não-tripulado **OU** possuir combustível acima de 50%])*

## 📈 Modelagem Matemática
A análise de telemetria conta com uma modelagem da regressão linear para previsão do consumo do propelente durante a queima atmosférica de descida:
*   **Equação:** $C(t) = a \cdot t + b$
*   *Onde:* $a$ = taxa de queima/min; $b$ = volume inicial; $t$ = tempo.
*   O cálculo alimenta a interface gráfica plotada através das bibliotecas **Matplotlib** e **Seaborn**.

## 🌍 Diretrizes ESG e Governança
O projeto foi desenvolvido em conformidade com:
1.  **Ambiental:** Protocolos de Proteção Planetária (COSPAR) e o Art. IX do Tratado do Espaço Exterior (ONU, 1967), prevenindo colisão e contaminação de Regiões Especiais de Marte.
2.  **Social:** Preservação incondicional da vida, bloqueando descidas tripuladas com níveis sub-ótimos de redundância (combustível e bateria).
3.  **Governança:** Motor de decisão 100% aberto, rastreável (logs de terminal) e sem viés de IA "caixa-preta".

## 🛠️ Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/mt076/Graduacao_FIAP.git
```
2. Instale as dependências utilizadas para visualização e análise de dados (caso não tenha):
```bash
pip install pandas numpy matplotlib seaborn
```
3. Execute o Jupyter Notebook `modelagem_cenario.ipynb` em sua IDE (VS Code, JupyterLab) ou rode os blocos sequencialmente para observar:
    * A geração da telemetria fictícia (arquivos `.csv`).
    * O processamento das estruturas lineares (Filas e Pilhas).
    * O algoritmo de Ordenação e Busca.
    * A plotagem da Modelagem Matemática.
