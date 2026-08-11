# Punção & Colapso Progressivo — INEC

Aplicativo web (arquivo único, sem dependências, offline) para **verificação de punção em lajes sobre pilares e cálculo da armadura de colapso progressivo** conforme a **NBR 6118**, portado fielmente da planilha de cálculo do curso (Cálculo de Punção ALM).

Material didático da **Pós-Graduação INEC** — Instituto Nacional de Engenharia Civil.

## Uso

Abra `index.html` no navegador. Nada a instalar. Também roda publicado via **GitHub Pages**.

## O que faz

- Verificação nos contornos **C** (biela), **C′** (2d), **C′ com armadura** e **C″** (fora da região armada).
- Armadura de punção **A_sw** necessária por camada.
- **Colapso progressivo**: armadura de flexão inferior e contagem de barras por bitola.
- **Diagrama do pilar** com eixos centroidais x, y (mesma figura da planilha), reativo às dimensões.
- **Auto-revisão** em três frentes: conferência célula a célula contra a planilha-fonte, simulações de exemplos práticos (pilar interno, de borda e de canto) e travas de sanidade que apontam entradas fora de faixa/domínio.
- Exportação do memorial via impressão/PDF.

## Validação

Motor de cálculo conferido **célula a célula** contra os valores em cache da planilha-fonte:

- Caso interno padrão: **31/31** grandezas conferem (erro < 1×10⁻⁹).
- Cenários de borda e de canto: **100%** contra o motor validado.

## Convenções (preservadas da planilha)

Fk em tf, Mk em tf·m, τ em kgf/cm², fck em MPa; `Pi = 3,14159265358979`; áreas nominais de barra tabeladas (ex.: Ø16 = 2,0 cm²). As expressões de τRd valem até ~C50.

## Responsabilidade técnica

Ferramenta de **apoio** ao projeto. Os cálculos e verificações **não substituem a análise do projetista** — os indicadores "OK/BUMM!!!/NECESSITA" reproduzem as verificações da planilha e servem à conferência. A interpretação, o valor adotado e a validação final são do **engenheiro responsável, que responde pela ART**. Dados fictícios/didáticos; nenhum projeto real de cliente.

---

© INEC — uso didático.
