# Invest More — Ferramenta de Planejamento de Investimentos

## Sobre o projeto

O **Invest More** é uma ferramenta de planejamento de investimentos desenvolvida do zero no Excel. Seu objetivo é auxiliar na organização de aportes mensais, projeções de patrimônio e distribuição de investimentos em Fundos de Investimento Imobiliário (FIIs), considerando diferentes perfis de investidor.

O projeto reúne fórmulas, funções de busca, validação de dados e referências entre planilhas em uma interface organizada e de fácil utilização.

## Funcionalidades

- Configuração de salário e rendimento da carteira.
- Sugestão de investimento correspondente a 30% do salário.
- Definição de aporte mensal independente do salário.
- Configuração do prazo de investimento e da taxa mensal para projeções.
- Cálculo de patrimônio acumulado.
- Estimativa de dividendos mensais.
- Projeções para cenários de 2, 5, 10, 20 e 30 anos.
- Seleção de perfil: Conservador, Moderado ou Agressivo.
- Distribuição percentual dos investimentos por categoria de FIIs.

## Categorias de FIIs

A ferramenta organiza a distribuição dos investimentos nas seguintes categorias:

- Papel
- Tijolo
- Híbridos
- FOFs
- Desenvolvimento
- Hotelarias

## Distribuição por perfil

| Categoria | Conservador | Moderado | Agressivo |
|---|---:|---:|---:|
| Papel | 30% | 32% | 50% |
| Tijolo | 50% | 35% | 10% |
| Híbridos | 10% | 8% | 5% |
| FOFs | 10% | 5% | 5% |
| Desenvolvimento | 0% | 10% | 10% |
| Hotelarias | 0% | 10% | 20% |
| **Total** | **100%** | **100%** | **100%** |

## Recursos técnicos utilizados

- **VF (Valor Futuro):** utilizada para projetar o patrimônio acumulado a partir dos aportes, prazo e taxa informados.
- **PROCV:** realiza buscas na tabela auxiliar para retornar os percentuais correspondentes ao perfil selecionado.
- **Validação de dados:** permite selecionar os perfis por listas suspensas.
- **Intervalos nomeados:** facilitam a identificação e utilização de células nas fórmulas.
- **Referências entre planilhas:** conectam a interface principal à base auxiliar de parâmetros.

### Intervalos nomeados

| Nome | Referência |
|---|---|
| Aport | APP!D14 |
| Dividendo | APP!D18 |
| Patrimonio | APP!D17 |
| qtd_anos | APP!D15 |
| Rendimento_carteira | APP!D10 |
| taxa_mensal | APP!D16 |

## Estrutura do arquivo

- **APP:** interface principal, entradas de dados, configurações, cálculos, cenários e distribuição dos investimentos.
- **Planilha2:** base auxiliar com parâmetros e percentuais utilizados nas consultas e distribuições por perfil.

## Como utilizar

1. Informe os dados financeiros nos campos de entrada.
2. Defina o aporte mensal e o prazo de investimento.
3. Informe as taxas utilizadas nas projeções.
4. Selecione o perfil de investidor desejado.
5. Consulte os resultados de patrimônio, dividendos estimados e distribuição por categoria.
6. Compare os cenários de diferentes períodos.

## Objetivo do desenvolvimento

O Invest More foi desenvolvido como uma ferramenta prática de organização e planejamento financeiro, aplicando recursos do Excel para transformar dados de entrada em projeções e informações estruturadas para análise.

## Observação

Os resultados apresentados são estimativas matemáticas condicionadas aos valores e às taxas informados. Não representam garantia de rentabilidade nem recomendação individualizada de investimento.

## Tecnologias e recursos

- Microsoft Excel
- Funções financeiras
- Função PROCV
- Validação de dados
- Intervalos nomeados
- Fórmulas e referências entre planilhas
