# Qualitativos e quantitativos de obras (SINAPI)

Gera orçamentos de obras residenciais e comerciais com a base oficial SINAPI, em planilha e relatório.


## Problema

Orçar obras com a tabela SINAPI exige cruzar milhares de composições. A tabela é regional por estado, então obras fora da capital precisam de ajuste local documentado.

## Como funciona

- Normaliza a planilha da Caixa e encontra os códigos SINAPI a partir da descrição de cada serviço.
- Motor de cálculo em Python: toda conta é feita em código, a IA nunca estima valores.
- Composição de BDI e camada de ajuste municipal, com justificativa escrita para cada fator.
- Estimativas paramétricas entregues em faixa (±15 a 25%), nunca em valor único.
- Itens sem preço vão para uma aba de pendências em vez de virar zero, e unidades divergentes ficam destacadas.

## Ferramentas

Claude Skill, Claude Cowork, Python (pandas, openpyxl, python-docx).

## Resultados

- Orçamento paramétrico e analítico em .xlsx e .docx.
- Testado de ponta a ponta com dados que continham erros propositais, para confirmar que o sistema os detecta.
