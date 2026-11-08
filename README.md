<div align="center">

# 🧭 Turismo Analytics
### Inteligência de Dados para o Turismo Brasileiro

*Chegadas internacionais e meios de hospedagem em uma única visão, comparável no tempo.*

![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-0F7B3F?style=flat)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat&logo=powerbi&logoColor=black)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)

**FATEC São Paulo** · Tecnologia em Análise e Desenvolvimento de Sistemas
Microinformática Aplicada (ILP590) · Prof. Veríssimo · 2º semestre de 2026

</div>

---

## 📌 Sobre o projeto

O turismo brasileiro é acompanhado por bases públicas oficiais que nascem em órgãos diferentes, com formatos, periodicidades e granularidades próprios. Os dados existem — o que falta é uma base consolidada que permita cruzá-los.

**Turismo Analytics** é o Projeto Evolutivo de Dados da disciplina: um fluxo que reúne as bases de chegada de turistas internacionais e de meios de hospedagem, trata e audita cada uma, e as transforma em um modelo analítico único, rastreável da linha bruta até o indicador no dashboard.

> **Pergunta central**
> Como o fluxo de turistas internacionais e a infraestrutura de hospedagem evoluem ao longo do tempo no Brasil, e que padrões sazonais e regionais emergem quando essas dimensões são analisadas em conjunto?

A análise se limita ao que existe nas fontes: eventos, avaliações de destinos e taxa de ocupação não constam dessas bases e não são simulados.

---

## 🗂️ Fontes de dados

| Fonte | O que traz |
|---|---|
| **Ministério do Turismo — Chegada de Turistas Internacionais** | Chegadas por período, país de origem, via de acesso e UF de entrada |
| **Cadastur — Cadastro de Meios de Hospedagem** (um arquivo por trimestre, 1T24 a 2T26) | Estabelecimentos por localidade e tipo, unidades habitacionais, leitos e acessibilidade |

---

## 🔁 Fluxo de trabalho

```
Dado bruto → Excel (auditoria) → Power Query (consolidação) → DAX (modelo e medidas) → Power BI (dashboard)
```

- **Excel** — cada arquivo bruto ganha abas Bruto, Tratado, Cadastros e Auditoria: nenhum valor original é sobrescrito, toda inconsistência é registrada com a linha de origem.
- **Power Query** — união dos trimestres e anos, padronização de nomes e criação do grão trimestral comum às duas fontes.
- **DAX** — tabela calendário, relacionamentos e medidas de demanda, oferta e cruzamento (chegadas, leitos, acessibilidade, variação anual, chegadas por leito).
- **Power BI** — dashboard interativo com evolução trimestral, sazonalidade, concentração de origem e relação demanda × oferta.

---

## 👥 Equipe

| Nome | Papel |
|---|---|
| **Anderson Edilson Presoto** | Engenharia de Dados |
| **Maria Carolina Domingues** | Governança de Dados |
| **Gustavo Oliveira da Silva** | Visualização de Dados e Apresentação dos Resultados |
| **Luis Augusto de Mattos Codonho Ferreira** | DevOps e Integrações · Líder do Projeto |

---

## 📚 Documentação

- **Proposta Técnica** — contexto, objetivos, fontes e planejamento
- **Documentação Técnica** — registro das etapas executadas, tratamentos aplicados e medidas DAX

---

<div align="center">
<sub>Baseado no projeto modelo <b>CaféData Brasil</b> da disciplina · Dados públicos do Ministério do Turismo e do Cadastur</sub>
</div>
