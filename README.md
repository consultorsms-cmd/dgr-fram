# DGR-FRAM Analyze

Plataforma de modelagem sociotécnica baseada no FRAM (Functional Resonance Analysis Method), integrada à Governança e Gestão de Dados e à Engenharia de Resiliência.

## Objetivo

Apoiar a análise da variabilidade funcional em sistemas sociotécnicos complexos, distinguindo variabilidades degradadoras e adaptativas e avaliando, de forma complementar, os mecanismos sistêmicos de resiliência.

## Funcionalidades

- Cadastro e modelagem de funções FRAM
- Cadastro de acoplamentos funcionais
- Avaliação da Variabilidade Degradadora Endógena (VDE)
- Avaliação da Variabilidade Degradadora Exógena (VDX)
- Avaliação da Variabilidade Adaptativa Endógena (VAE)
- Avaliação da Variabilidade Adaptativa Exógena (VAX)
- Avaliação dos Mecanismos de Resiliência (MR) em nível sistêmico
- Parametrização por estimativas mínima, média e máxima
- Simulação probabilística por distribuição Beta-PERT
- Simulação de Monte Carlo
- Cálculo de Média, P90, P95, P99 e Probabilidade de Criticidade
- Análise comparativa dos cenários MR e VAE + VAX
- Matriz Interpretativa Cruzada VD × VA
- Dashboard analítico
- Geração e exportação de relatórios

## Modelo Analítico

A Variabilidade Degradadora (VD) é representada por:

VD = VDE + VDX

Onde:

- VDE = Variabilidade Degradadora Endógena
- VDX = Variabilidade Degradadora Exógena

A Variabilidade Adaptativa (VA) é representada por:

VA = VAE + VAX

Onde:

- VAE = Variabilidade Adaptativa Endógena
- VAX = Variabilidade Adaptativa Exógena

## Simulação de Monte Carlo

O DGR-FRAM Analyze utiliza distribuição Beta-PERT para representar a incerteza associada às estimativas de variabilidade.

São analisados dois cenários comparativos:

### Cenário MR

Aplicação do índice sistêmico e determinístico de Mecanismos de Resiliência (MR) como redutor da Variabilidade Degradadora:

VFRR_MR = VD × (1 − MR)

### Cenário VAE + VAX

Aplicação da capacidade adaptativa como redutor da Variabilidade Degradadora:

VFR = VD × [1 − min(1, VAE + VAX)]

VAE e VAX são amostradas separadamente durante a Simulação de Monte Carlo.

## Indicadores

Os resultados probabilísticos incluem:

- Média
- P90
- P95
- P99
- Probabilidade de Criticidade

O índice MR é tratado como indicador global e sistêmico, não sendo atribuído individualmente às funções FRAM.

## Matriz Interpretativa

A interpretação dos resultados considera conjuntamente:

- Variabilidade Degradadora (VD)
- Variabilidade Adaptativa (VA)

A Matriz Interpretativa Cruzada VD × VA auxilia na caracterização do contexto operacional e na interpretação da relação entre pressões degradadoras e capacidades adaptativas.

## Aplicação

O DGR-FRAM Analyze foi concebido como ferramenta de apoio à análise de sistemas sociotécnicos complexos e infraestruturas críticas, permitindo integrar modelagem funcional, classificação de variabilidades, análise probabilística e mecanismos sistêmicos de resiliência.

## Autor

Antonio Francisco Corno
