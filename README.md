# Global Solution GS26_2 — CitizenTech: Mobilidade Urbana Inteligente (MCM)
 
> **Curso:** Ciência da Computação (1º Ano — Turma 1CC)  
> **Disciplina:** Modelagem Matemática e Computacional (MCM)  
> **Integrante:** Gustavo de Souza Correa (RM 570746) e Arthur Tae Gun Yong (RM 570647)

---

## 📂 Arquivos Entregues na Pasta `trabalhosGS2/MCM`

1. **`Relatorio_GS2026_2_MCM.pdf`**  
   Relatório técnico completo em **PDF (4 páginas A4)** pronto para entrega, contendo todas as respostas formais, matrizes, demonstrações matemáticas de Álgebra Linear, código Python e gráficos das **Etapas 1 e 2**:
   - **Etapa 1 (5,0 pontos) — Diagnóstico e Modelagem da Situação Atual:**
     - **a)** Definição formal das variáveis ($x_1 = N, x_2 = S, x_3 = L, x_4 = O \in \mathbb{Z}_+$).
     - **b)** Construção do sistema linear $4 \times 4$ a partir dos quatro indicadores do Relatório I.
     - **c)** Representação matricial $A\mathbf{x} = \mathbf{b}$.
     - **d)** Investigação de existência e unicidade da solução por Álgebra Linear ($\det(A) = 3 \neq 0$, invertibilidade de $A$, independência linear das colunas, escalonamento de Gauss e **Teorema de Rouché-Capelli** com $\text{posto}(A) = \text{posto}([A\mid\mathbf{b}]) = n = 4$).
     - **e)** Implementação computacional em Python (`np.linalg.solve`) encontrando $\mathbf{x} = (12, 20, 16, 24)^T$.
     - **f)** Verificação completa de todos os registros operacionais ($A\mathbf{x} = \mathbf{b}$).
   - **Etapa 2 (5,0 pontos) — Desenvolvimento de uma Política de Redistribuição:**
     - **a)** Estimativa de ônibus necessários por região ($n_i = d_i / 40 \implies [14, 19, 18, 21]$).
     - **b)** Diagnóstico de desequilíbrios regionais (Déficits: Norte $-2$ ônibus / $-80$ vagas, Leste $-2$ ônibus / $-80$ vagas; Superávits: Sul $+1$ ônibus / $+40$ vagas, Oeste $+3$ ônibus / $+120$ vagas; Equilíbrio global de $72$ ônibus).
     - **c)** Proposta e justificativa da política de redistribuição (apresentando tanto a **Política I — Pool Central Proporcional à Demanda** desenvolvida no código do grupo quanto a **Política II — Transferência Operacional Direta Superávit $\to$ Déficit** de deslocamento mínimo).
     - **d)** Representação matemática por meio de Transformação Linear $T: \mathbb{R}^4 \to \mathbb{R}^4$, $\mathbf{y} = T(\mathbf{x}) = T\mathbf{x}$.
     - **e)** Construção das matrizes associadas $T_1$ e $T_2$ e explicação detalhada do significado de cada coeficiente $t_{ij}$.
     - **f)** Demonstração matemática formal da preservação da frota total de $72$ ônibus ($\sum_{i=1}^4 t_{ij} = 1 \implies \mathbf{1}^T T \mathbf{x} = \mathbf{1}^T \mathbf{x} = 72$) e da não negatividade das alocações ($t_{ij} \ge 0 \land x_j \ge 0 \implies y_i \ge 0$).

2. **`Notebook_GS2026_2_MCM.ipynb`**  
   Jupyter Notebook pronto para execução no Jupyter/Google Colab contendo toda a fundamentação em Markdown/LaTeX e os blocos de código das Etapas 1 e 2 já executados.
