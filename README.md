# 💸 Monitoramento de Custos no Azure Data Factory

Este repositório documenta o processo de monitoramento de custos no **Azure Data Factory**, com descrições, prints da interface, insights e sugestões de melhorias para controle de gastos.

---

## 📌 Objetivo

Demonstrar como acompanhar e controlar os custos gerados por pipelines, triggers e atividades no Data Factory, além de compartilhar boas práticas e aprendizados do processo.

---

## 🔍 Etapas do Monitoramento

### 1. Acessando o Cost Management

- Acesse o portal do Azure.
- Vá até o recurso do Azure Data Factory desejado.
- No menu lateral, selecione **Cost Management** > **Cost Analysis**.

📷 *Exemplo de visualização:*

![Cost Analysis](images/cost-analysis.png)

---

### 2. Aplicando filtros por período e recurso

- Visualize os custos por dia, semana ou mês.
- Use filtros para detalhar os recursos consumidos por atividade/pipeline.

📷 *Print com filtros aplicados:*

![Filtros de Custo](images/filtros-custos.png)

---

### 3. Criando orçamentos e alertas

- No painel do **Cost Management**, acesse **Budgets**.
- Crie um novo orçamento com um limite mensal.
- Configure alertas por e-mail para 80%, 90% e 100% do orçamento.

📷 *Print de criação de alerta:*

![Alertas de Orçamento](images/alertas-custos.png)

---

## 💡 Insights Obtidos

- 🔁 **Triggers com alta frequência** (ex: a cada 5 minutos) geram custos consideráveis.
- 🌐 **Transferência entre regiões** (cross-region) tem custo elevado.
- 🧪 **Data Flows** são poderosos, mas podem custar mais que atividades básicas.
- 📊 Análise diária permite identificar gargalos de custo rapidamente.
- ⏲️ Rodar pipelines em horários estratégicos pode reduzir custos (especialmente com escalabilidade automática ou uso sob demanda).
- 🏷️ O uso de **tags** facilita muito o rastreio por centro de custo ou projeto.

---

## 🚀 Possibilidades Futuras

- Exportar dados de custo com API do Azure para visualização no Power BI.
- Automatizar alertas com lógica personalizada.
- Criar dashboards de custo por pipeline.
- Associar custos por projeto, cliente ou responsável através de **tags**.

---

## 🗂️ Estrutura de Diretórios

```
datafactory-cost-monitoring/
├── README.md
└── images/
    ├── cost-analysis.png
    ├── filtros-custos.png
    └── alertas-custos.png
```

---

## 📚 Referências

- [Azure Data Factory - Visão Geral](https://learn.microsoft.com/pt-br/azure/data-factory/introduction)
- [Cost Management + Billing - Microsoft Learn](https://learn.microsoft.com/pt-br/azure/cost-management-billing/)
- [Tutorial: Criar alertas de orçamento](https://learn.microsoft.com/pt-br/azure/cost-management-billing/costs/tutorial-acm-create-budgets)

---
