Segue versão **100% copiável** para colocar direto no `README.md`:

---

# 📊 Dashboard de Consumo de Energia – Power BI

## 📌 Sobre o Projeto

Dashboard desenvolvido em **Power BI** para análise do consumo de energia elétrica ao longo de 12 meses.

O objetivo é visualizar tendências, identificar padrões de consumo, analisar picos de demanda e apoiar decisões baseadas em dados.

---

## 📂 Fonte de Dados

O projeto utiliza um arquivo CSV contendo:

* `DataHora`
* `CodigoMedidor`
* `Empresa`
* `TipoEnergia`
* `ConsumoAtivo_kWh`
* `ConsumoReativo_kVArh`
* `Demanda_kW`
* `Demanda_Max_Hora`
* `GeracaoAtiva_kWh`
* `GeracaoReativa_kVArh`

---

## 📐 Modelagem

A modelagem foi realizada diretamente no Power BI, com tratamento de:

* Tipagem correta de datas
* Agregações por período (Ano/Mês)
* Criação de medidas em DAX

### Medida Principal

```DAX
Consumo Total (kWh) =
SUM ( detalhes_12meses_caeira[ConsumoAtivo_kWh] )
```

---

## 📊 Visualizações

* 📈 Gráfico de linha com evolução temporal do consumo
* 📅 Análise mensal consolidada
* 📊 Indicadores agregados
* ⚡ Estrutura preparada para análise de demanda e geração

---

## 🎨 Customizações Aplicadas

* Eixo temporal configurado como contínuo
* Unidades de exibição ajustadas (milhares/milhões)
* Layout limpo e minimalista
* Redução de poluição visual (grid simplificado)

---

## 🚀 Como Executar

1. Baixe o arquivo `.pbix`
2. Abra no **Power BI Desktop**
3. Atualize a fonte de dados, se necessário
4. Explore os relatórios ou publique no Power BI Service

---

## 🛠 Tecnologias Utilizadas

* Power BI Desktop
* DAX (Data Analysis Expressions)
* Modelagem de dados
* Visualização analítica

---

## 📎 Arquivo do Projeto

```
Consumo de Energia.pbix
```

---

## 🔮 Melhorias Futuras

* Média móvel de consumo
* Identificação automática de pico de demanda
* Comparação entre empresas
* KPIs estratégicos
* Dashboard executivo

---

## 📄 Licença

Projeto desenvolvido para fins de estudo. Livre para adaptação.
