# Plano Estratégico The Navigator Company 2026–2028

**Microsite Estático de Alta Fidelidade | 10º MBA Executivo ISAG**

---

## ⚠️ Disclaimer Académico

Este projeto é de natureza **estritamente académica**, desenvolvido no âmbito do **MBA Executivo do ISAG (2025/2026)**. As análises, projeções e recomendações estratégicas apresentadas não constituem informações oficiais da **The Navigator Company** e foram elaboradas unicamente para fins pedagógicos.

### Contexto de Entrega
- **Módulo:** Direção Estratégica de Pessoas
- **Docente:** Professor Protásio Leão
- **Objetivo:** Alinhamento da estratégia corporativa com a gestão de talentos e transformação digital.

---

## 📋 Arquitetura do Projeto

O ecossistema é composto por três interfaces principais integradas, focadas em fornecer uma visão 360º da estratégia:

### 1. Painel Corporativo Principal (`index.html`)
O hub central do plano estratégico, contendo:
- **Sumário Executivo:** Desafio de gerir o declínio estrutural do papel UWF e acelerar a bioeconomia.
- **Identidade:** Visão, Missão e Valores focados em sustentabilidade.
- **Análises de Macroambiente:**
    - **PESTEL:** Avaliação de fatores Políticos, Económicos, Sociais, Tecnológicos, Ecológicos e Legais.
    - **5 Forças de Porter:** Análise da competitividade setorial.
    - **FCS (Fatores Críticos de Sucesso):** Fibra sustentável, Inovação (RAIZ), Logística.
    - **VRIO:** Identificação de recursos de vantagem competitiva sustentável.
- **Matriz SWOT & TOWS:** Planeamento tático de curto e médio prazo.
- **Plano de Ações:** 7 iniciativas prioritárias (Packaging, Tissue, Digitalização, etc.).

### 2. Estratégia de RH & Diagnóstico (`rh_estrategia.html`)
Módulo avançado para a gestão de Capital Humano:
- **Diagnóstico Estratégico (2020-2024):** Visualização interativa de KPIs históricos via **Chart.js**:
    - Headcount (Evolução de colaboradores).
    - Pirâmide Etária (% < 30 anos).
    - Diversidade (% Mulheres).
    - Turnover (%) e Horas de Formação.
    - Segurança no Trabalho (LTI).
- **HR Scorecard (2026-2028):** Dashboard de metas estratégicas:
    - **Perspetiva Financeira:** Custo de Pessoal sobre Receita (Meta < 13%).
    - **Perspetiva Processos:** Digitalização de processos de RH.
    - **Perspetiva Pessoas:** Digital Readiness (%) e Retenção de Talentos.
    - **Perspetiva Aprendizagem:** Liderança feminina e KPIs de clima.
- **Centro de Dados:**
    - **CSV Viewer Premium:** Visualização dinâmica de indicadores via parsing de `hr_indicators_export.csv`.
    - **Central de Downloads:** Acesso imediato ao PDF do Plano Estratégico e base de dados bruta.

### 3. Balanced Scorecard Corporativo (`bsc.html`)
Painel de monitorização executiva com:
- **4 Perspetivas Corporativas:** Financeira, Clientes, Processos e Aprendizagem.
- **Modos de Visualização:** Alternância entre Vista de Cartões (Grid) e Vista de Tabela Completa.
- **Exportação:** Funcionalidade de download de dados do BSC em formato CSV.

---

## 🎨 Design & Identidade Visual

### Paleta Institucional (CSS Variables)
Customização total baseada na marca Navigator:
- `--nav-dk1: #1C3D2E` (Verde Floresta - Primária)
- `--nav-lt2: #C7E7A1` (Verde Folha - Backgrounds)
- `--nav-accent4: #7AA64A` (Verde Navigator - Destaques)

### Assets Técnicos
- **Tipografia:** Source Sans Pro (moderna e legível).
- **Framework Visual:** Template "Dimension" by HTML5 UP, extensivamente modificado para um look premium e corporativo.
- **Responsividade:** Layout validado para Desktop, Tablet e Mobile.

---

## 📁 Estrutura de Diretórios

```
C:\dev\navigator\
├── index.html                  # Dashboard Estratégico Global
├── rh_estrategia.html          # Módulo de Direção Estratégica de Pessoas
├── bsc.html                    # Balanced Scorecard Interativo
├── documentos/                 # PDFs Formais e Ficheiros de Dados (CSV)
├── images/                     # Biblioteca de Imagens de Alta Resolução
└── assets/
    ├── css/                    # theme.css (Custom), main.css, fontawesome
    └── js/                     # rh_data.js (Base de Dados), main.js, Charts
```

---

## 🛠️ Tecnologias & Performance

- **Frontend:** HTML5 Semântico, CSS3 (Grid/Flexbox/Variables).
- **Interatividade:** JavaScript Vanilla (ES6) – Sem dependências pesadas de frameworks.
- **Visualização de Dados:** Chart.js Integration.
- **Parsing de Dados:** CSV Fetch & Dynamic Render.
- **Acessibilidade:** WCAG 2.1 AA (Amostras de contraste validadas).

---

## � Autores (MBA ISAG)

- **Bruno Silva**
- **Joana Carvalho**
- **Tiago Valinho**
- **Cristina Vasconcelos**
- **Guilherme Marques**

---

**© 2026 | Projeto Académico MBA Executivo ISAG**
*"Innovating for a Sustainable Bio-Future"*
