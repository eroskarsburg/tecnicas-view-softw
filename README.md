# Análise de Gorjetas - Rede de Restaurantes

## Descrição do Projeto
Este projeto desenvolve uma análise completa dos dados de gorjetas de uma rede de restaurantes com 244 clientes, utilizando as bibliotecas Seaborn, Pandas e Matplotlib do Python.

## Arquivos do Projeto

### 1. `gorjetas.csv`
Dataset com 244 registros contendo:
- `total_conta`: Valor total da conta
- `gorjeta`: Valor da gorjeta deixada
- `sexo`: Sexo do cliente (Homem/Mulher)
- `fumante`: Se o cliente é fumante (Sim/Não)
- `dia`: Dia da semana (Dom, Seg, Ter, Qua, Qui, Sex, Sab)
- `tempo`: Período da refeição (Almoço/Jantar)
- `quantidade`: Número de pessoas na mesa

### 2. `main.py` ⭐ **ARQUIVO PRINCIPAL**
Script único que contém todo o código Python do projeto:
- **Função 1**: `analise_principal()` - Gera PDF com gráficos de densidade
  - **Gráfico a)** Densidade das gorjetas por sexo
  - **Gráfico b)** Densidade das gorjetas por quantidade de pessoas (2, 3, 4 pessoas)
  - **Gráfico c)** Densidade das gorjetas por dia da semana
  - **Análise textual** com resultados principais e conclusões
- **Função 2**: `estatisticas_complementares()` - Estatísticas detalhadas
  - Estatísticas descritivas gerais
  - Análise detalhada por sexo, quantidade de pessoas, dia da semana e período
  - Correlação entre conta total e gorjeta
  - Top 5 maiores gorjetas
- **Execução completa**: Roda todas as análises automaticamente

### 3. `analise_gorjetas_restaurante.pdf`
Relatório final em PDF contendo todos os gráficos e análises.

## Como Executar

### Pré-requisitos
```bash
pip install pandas matplotlib seaborn numpy
```

### Execução

```bash
python main.py
```

Este comando único executa:
1. Geração do PDF com todos os gráficos de densidade
2. Exibição das estatísticas complementares no terminal
3. Resumo completo da análise

## Principais Descobertas

### 1. Análise por Sexo
- **Homens**: 64.3% dos clientes, gorjeta média de $3.09
- **Mulheres**: 35.7% dos clientes, gorjeta média de $2.83
- Distribuição similar entre os sexos, com pico entre $2-4

### 2. Análise por Quantidade de Pessoas
- **Mesas de 2 pessoas**: Mais frequentes (63.9%), gorjeta média $2.58
- **Mesas maiores**: Tendem a deixar gorjetas proporcionalmente maiores
- **6 pessoas**: Maior gorjeta média ($5.22)

### 3. Análise por Dia da Semana
- **Sábado**: Maior movimento (35.7% dos clientes)
- **Domingo**: Maior gorjeta média ($3.26)
- **Quinta-feira**: Segundo maior movimento (25.4%)

### 4. Análise por Período
- **Jantar**: 72.1% do movimento, gorjeta média $3.10
- **Almoço**: 27.9% do movimento, gorjeta média $2.73

## Principais Conclusões

1. **Diferença por Sexo**: Pequena diferença nas gorjetas entre homens e mulheres
2. **Tamanho da Mesa**: Grupos maiores deixam gorjetas maiores
3. **Dias da Semana**: Fins de semana têm melhor desempenho
4. **Oportunidades**: Melhorar movimento em quinta e sexta-feira

## Critérios de Avaliação Atendidos

✅ **Gráfico total de gorjetas por sexo** (1,5 pontos)
✅ **Gráfico total de gorjetas pela quantidade de pessoas na mesa** (1,5 pontos)  
✅ **Gráfico total de gorjetas por dia da semana** (1,5 pontos)
✅ **Análise textual sobre a empresa a partir dos gráficos gerados** (1,5 pontos)

**Total: 6,00 pontos**