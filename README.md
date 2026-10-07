# 📊 FII Simulador de Investimentos em Fundos Imobiliários

Uma ferramenta interativa desenvolvida no Microsoft Excel para simular a formação de patrimônio, estimar dividendos mensais e analisar diferentes cenários de investimento.


O **FII** é uma ferramenta desenvolvida no Microsoft Excel para simular investimentos em Fundos Imobiliários (FIIs), permitindo visualizar a evolução do patrimônio, estimar dividendos mensais e analisar a distribuição dos aportes de acordo com diferentes perfis de investidor.

A ferramenta foi estruturada para responder às principais perguntas de negócio relacionadas ao planejamento de investimentos:

- Quanto investir por mês?
- Por quantos anos investir?
- Qual a taxa de rendimento mensal?
- Quanto de patrimônio será acumulado?
- Quanto poderá receber de dividendos por mês?

> ⚠️ **Aviso:** os percentuais utilizados na ferramenta são exemplos didáticos para fins de simulação e não representam recomendação de investimento.

---

## 🎯 Objetivo

O objetivo do projeto é transformar informações financeiras simples em uma visão clara do potencial de acumulação de patrimônio ao longo do tempo.

A ferramenta permite informar salário, aporte, prazo, rendimento mensal e perfil de investidor. A partir dessas informações, os cálculos são realizados automaticamente.

---




# 🎯 Objetivo do projeto

O objetivo do **FII VISION** é transformar informações financeiras simples em uma ferramenta visual e interativa no Excel.

A partir de algumas informações fornecidas pelo usuário, a ferramenta calcula automaticamente:

- patrimônio acumulado;
- dividendos mensais estimados;
- total aportado;
- projeções para diferentes períodos;
- aporte sugerido com base em 10% do salário;
- distribuição do aporte entre diferentes tipos de FII.

A ferramenta também permite alterar o perfil do investidor e observar automaticamente as mudanças na composição dos aportes.

# 🖥️ Estrutura da ferramenta

A planilha possui duas abas principais:

### 📈 Simulador

É a tela principal da ferramenta.

Nela estão disponíveis:

- salário mensal;
- aporte mensal;
- aporte sugerido de 10% do salário;
- prazo do investimento;
- rendimento mensal;
- perfil do investidor;
- patrimônio acumulado;
- dividendos mensais;
- total aportado;
- projeções de patrimônio;
- distribuição do aporte entre seis tipos de FII;
- gráfico de pizza;
- segunda simulação utilizando 10% do salário.

### ⚙️ Apoio

A aba de apoio concentra as informações utilizadas na estrutura dos cálculos:

- perfis de investidor;
- tipos de FII;
- percentuais de distribuição;
- chave composta;
- listas utilizadas na validação de dados.

---

# 📌 Perguntas de negócio

| Pergunta | Onde aparece na ferramenta |
|---|---|
| Quanto investir por mês? | `Simulador!C10` |
| Qual o salário mensal? | `Simulador!C9` |
| Qual o aporte sugerido? | `Simulador!C11` |
| Por quantos anos investir? | `Simulador!C12` |
| Qual a taxa de rendimento mensal? | `Simulador!C13` |
| Qual o perfil escolhido? | `Simulador!C14` |
| Quanto de patrimônio será acumulado? | `Simulador!F9` |
| Quanto receberá de dividendos por mês? | `Simulador!F10` |
| Quanto foi aportado ao longo do período? | `Simulador!F11` |
| Quanto acumulará em diferentes prazos? | `Simulador!B20:D24` |
| Quanto acumularia utilizando 10% do salário? | `Simulador!F20` |
| Como o aporte será distribuído? | `Simulador!B30:D35` |

---

# 🧮 Cálculo do patrimônio

O cálculo do patrimônio acumulado utiliza a função financeira **VF (Valor Futuro)**.

A função considera:

- taxa de rendimento mensal;
- quantidade de meses;
- valor do aporte mensal;
- valor inicial do investimento.

A lógica utilizada é:

```text
Patrimônio = VF(taxa mensal, prazo em meses, aporte mensal)


