# Plano Estratégico The Navigator Company 2026–2028

**Microsite Estático | Trabalho Académico MBA ISAG**

---

## ⚠️ Disclaimer Académico

Este é um **projeto académico** desenvolvido no âmbito do 10º MBA Executivo do ISAG (Instituto Superior de Administração e Gestão). O conteúdo apresentado **não representa a estratégia real da The Navigator Company** e foi elaborado exclusivamente para fins didáticos e de aprendizagem.

---

## 📋 Sobre o Projeto

Microsite estático que apresenta uma proposta de Plano Estratégico 2026–2028 para a The Navigator Company, assente na **Diferenciação Focada na Sustentabilidade e Inovação**.

### Estrutura do Site

- **Página Principal (index.html):** 9 secções navegáveis
  - Sobre o Projeto
  - Sumário Executivo
  - Visão, Missão e Valores
  - Análises Estratégicas (PESTEL, 5 Forças, FCS, VRIO)
  - Análise SWOT
  - Objetivos & Indicadores (8 KPIs)
  - Plano de Ações (7 iniciativas)
  - Créditos & Referências

- **Balanced Scorecard (bsc.html):** Painel interativo
  - 4 perspectivas (Financeira, Clientes, Processos, Aprendizagem)
  - Toggle entre vista de cartões e tabela
  - Exportação para CSV
  - Ícones SVG personalizados

---

## 🎨 Design & Identidade Visual

### Paleta de Cores Navigator

```css
--nav-dk1: #1C3D2E;   /* Texto principal / títulos / botões sólidos */
--nav-lt1: #FFFFFF;   /* Fundo light e texto invertido */
--nav-dk2: #3C3C3C;   /* Texto secundário */
--nav-lt2: #C7E7A1;   /* Fundo hero/chapters */
--nav-accent1: #B3E28D; /* Primária de realce */
--nav-accent2: #E6E8A4;
--nav-accent3: #A8CE68;
--nav-accent4: #7AA64A;
--nav-accent5: #665C3B;
--nav-accent6: #F2F2D5;
```

### Tipografia

- **Fonte principal:** Source Sans Pro (do template Dimension)
- **Alternativa:** Inter (se necessário)
- **Contrastes:** AA mínimo (WCAG 2.1)

### Template Base

- **Dimension** by [HTML5 UP](https://html5up.net)
- Licença: [Creative Commons Attribution 3.0](https://html5up.net/license)
- Totalmente responsivo (mobile-first)

---

## 📁 Estrutura de Ficheiros

```
C:\dev\navigator\
│
├── index.html                  # Página principal
├── bsc.html                    # Balanced Scorecard
├── README.md                   # Este ficheiro
│
├── assets/
│   ├── css/
│   │   ├── main.css           # Estilos do template
│   │   ├── theme.css          # Paleta Navigator (variáveis CSS)
│   │   └── noscript.css
│   ├── js/
│   │   ├── jquery.min.js
│   │   ├── browser.min.js
│   │   ├── breakpoints.min.js
│   │   ├── util.js
│   │   └── main.js            # Funcionalidades do template
│   ├── sass/                  # Fontes SASS (opcional)
│   └── webfonts/              # Ícones FontAwesome
│
├── images/                     # Imagens do projeto
│   ├── logo_Navigator_vp_pos_rgb.png
│   ├── logo_Navigator_vp_neg_rgb.png
│   ├── floresta_01.png
│   ├── fabrica_bobina_gigante_papel.png
│   ├── brotos_eucalipito.png
│   ├── estufa_01.png
│   ├── paineis_fotovoltaicos.png
│   ├── trabalhador_01.png
│   ├── papel_uwf.png
│   ├── plantas.png
│   └── bg.png
│
└── temp/                       # Ficheiros originais (PDF, PPTX)
    ├── Navigator_v1.pdf
    └── Navigator_v1.pptx
```

---

## 🚀 Como Usar

### 1. Abrir Localmente

1. Descarregar todos os ficheiros para uma pasta local
2. Abrir `index.html` num navegador moderno (Chrome, Firefox, Edge, Safari)
3. Navegar pelas secções através do menu lateral
4. Aceder ao Balanced Scorecard via menu ou link direto para `bsc.html`

### 2. Publicar no GitHub Pages

```bash
# 1. Criar repositório no GitHub
git init
git add .
git commit -m "Primeiro commit: Plano Estratégico Navigator 2026-2028"

# 2. Adicionar remote
git remote add origin https://github.com/SEU_USERNAME/navigator-strategic-plan.git

# 3. Push para GitHub
git push -u origin main

# 4. Ativar GitHub Pages
# Ir a Settings → Pages → Source: main branch → Save
# O site estará disponível em: https://SEU_USERNAME.github.io/navigator-strategic-plan/
```

### 3. Customizar GitHub Pages (opcional)

No ficheiro `index.html`, ajustar links absolutos se necessário:

```html
<!-- Manter links relativos (recomendado) -->
<link rel="stylesheet" href="assets/css/main.css" />
<link rel="icon" type="image/png" href="images/logo_Navigator_vp_pos_rgb.png" />
```

---

## 🔧 Editar Conteúdos

### Alterar Dados do Balanced Scorecard

No ficheiro `bsc.html`, localizar o objeto JavaScript `bscData` (aprox. linha 250):

```javascript
const bscData = {
  "Financeira": {
    "Objetivos": [ /* editar aqui */ ],
    "KPIs": [ /* editar aqui */ ],
    "Metas2028": [ /* editar aqui */ ],
    "Iniciativas": [ /* editar aqui */ ]
  },
  // ... outras perspectivas
};
```

**Nota:** Manter sempre a mesma estrutura JSON para garantir compatibilidade com as funções de renderização e exportação.

### Substituir Imagens

1. Colocar novas imagens na pasta `images/`
2. Editar referências em `index.html` e `bsc.html`:

```html
<!-- Exemplo -->
<span class="image main"><img src="images/NOVA_IMAGEM.png" alt="Descrição" /></span>
```

3. **Importante:** Sempre incluir atributo `alt` para acessibilidade

### Modificar Paleta de Cores

Editar ficheiro `assets/css/theme.css`:

```css
:root {
  --nav-dk1: #NOVA_COR;  /* Alterar valor hexadecimal */
  --nav-lt1: #NOVA_COR;
  /* ... */
}
```

As variáveis CSS propagam-se automaticamente por todo o site.

---

## ✅ Acessibilidade (WCAG 2.1 AA)

### Conformidade Implementada

- ✅ **Contraste de cores:** Rácio mínimo 4.5:1 (texto normal) e 3:1 (texto grande)
- ✅ **Textos alternativos:** Todas as imagens têm atributo `alt` descritivo
- ✅ **Navegação por teclado:** Menu e links acessíveis via Tab/Enter
- ✅ **Estrutura semântica:** HTML5 semântico (`<header>`, `<nav>`, `<article>`, `<footer>`)
- ✅ **Responsividade:** Layout adapta-se a ecrãs 320px – 3840px

### Validar Acessibilidade

Ferramentas recomendadas:
- [WAVE Web Accessibility Evaluation Tool](https://wave.webaim.org/)
- [axe DevTools](https://www.deque.com/axe/devtools/) (extensão Chrome/Firefox)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) (Chrome DevTools)

---

## 📦 Otimização de Imagens

### Converter para WebP (Opcional)

Para melhor performance, converter imagens PNG/JPG para WebP:

```bash
# Instalar cwebp (ImageMagick ou libwebp)
# Windows (via Chocolatey)
choco install webp

# Converter imagens
cwebp -q 85 floresta_01.png -o floresta_01.webp
cwebp -q 85 fabrica_bobina_gigante_papel.png -o fabrica_bobina_gigante_papel.webp
# ... repetir para todas as imagens
```

Depois, atualizar referências no HTML:

```html
<picture>
  <source srcset="images/floresta_01.webp" type="image/webp">
  <img src="images/floresta_01.png" alt="Floresta de eucalipto Navigator" />
</picture>
```

---

## 🎯 Funcionalidades do Balanced Scorecard

### 1. Vista de Cartões (Cards)
- Layout em grelha responsiva
- Ícones SVG personalizados por perspectiva
- Cores diferenciadas por categoria
- Hover effects para interatividade

### 2. Vista de Tabela
- Tabela HTML completa com todas as perspectivas
- Scroll horizontal em dispositivos móveis
- Formatação clara e legível

### 3. Exportação CSV
- Botão "Exportar CSV" gera ficheiro descarregável
- Formato compatível com Excel/Google Sheets
- Separador: ponto-e-vírgula (;)
- Encoding: UTF-8 com BOM

### 4. Toggle de Vistas
- JavaScript vanilla (sem dependências externas)
- Transições suaves entre vistas
- Estado persistente durante a sessão

---

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estrutura semântica
- **CSS3:** Variáveis CSS, Flexbox, Grid, Animações
- **JavaScript (ES6+):** Manipulação DOM, JSON, exportação CSV
- **SVG:** Ícones vetoriais inline
- **FontAwesome:** Ícones complementares (via template)

**Sem dependências de build:** Não requer Node.js, npm, Webpack ou qualquer ferramenta de compilação.

---

## 📊 Dados do BSC (JSON)

O Balanced Scorecard utiliza dados estruturados em JSON, facilitando:

- **Manutenção:** Alterar dados sem tocar no HTML/CSS
- **Reutilização:** Exportar para outras ferramentas (Excel, BI)
- **Extensibilidade:** Adicionar novas perspectivas facilmente

### Estrutura do JSON

```javascript
{
  "Nome_da_Perspectiva": {
    "icon": "identificador_do_icon",
    "color": "var(--css-variable)",
    "Objetivos": [ "string", "string", ... ],
    "KPIs": [ "string", "string", ... ],
    "Metas2028": [ "string", "string", ... ],
    "Iniciativas": [ "string", "string", ... ]
  }
}
```

---

## 👥 Equipa do Projeto

**Instituição:** ISAG – European Business School
**Programa:** 10º MBA Executivo
**Unidade Curricular:** Estratégia Empresarial
**Ano Letivo:** 2024/2025

**Professores Orientadores:**
- Prof. Dr. Victor Tavares
- Prof. Marco Dias

**Estudantes:**
- Bruno Silva
- Joana Carvalho
- Tiago Valinho
- Cristina Vasconcelos
- Guilherme Marques

---

## 📜 Licença e Créditos

### Template Dimension
- **Autor:** [HTML5 UP](https://html5up.net)
- **Licença:** [Creative Commons Attribution 3.0](https://creativecommons.org/licenses/by/3.0/)
- **Uso:** Livre para projetos pessoais e comerciais com atribuição

### Conteúdo Académico
- **Propriedade:** Autores do trabalho académico
- **Uso:** Exclusivamente educativo
- **Nota:** Não representa estratégia oficial da Navigator Company

### Imagens e Logótipos
- **Propriedade:** The Navigator Company
- **Uso:** Educativo e ilustrativo (contexto académico)
- **Fonte:** Website oficial e materiais públicos

---

## 🔗 Links Úteis

- **The Navigator Company:** [www.thenavigatorcompany.com](https://www.thenavigatorcompany.com/)
- **ISAG Business School:** [www.isag.pt](https://www.isag.pt/)
- **HTML5 UP Templates:** [html5up.net](https://html5up.net/)
- **Web Content Accessibility Guidelines:** [www.w3.org/WAI/WCAG21/quickref](https://www.w3.org/WAI/WCAG21/quickref/)

---

## 📞 Suporte

Para questões sobre este projeto académico, contactar os autores via:

- **Email:** [através do ISAG Business School]
- **LinkedIn:** [perfis dos autores]

---

## 📝 Changelog

### v1.2.0 (Novembro 2024)
- ✅ Página BSC com background consistente (bg.png desfocado)
- ✅ Botões reformulados para consistência com home
- ✅ Header BSC com gradiente igual ao hero da home
- ✅ Identidade visual unificada em todo o site

### v1.1.0 (Novembro 2024)
- ✅ Background desfocado implementado (bg.png)
- ✅ Correções de contraste para WCAG AA/AAA
- ✅ Todos os textos com rácio > 7:1

### v1.0.0 (Novembro 2024)
- ✅ Lançamento inicial do microsite
- ✅ 9 secções completas na página principal
- ✅ Balanced Scorecard interativo com 4 perspectivas
- ✅ Exportação CSV funcional
- ✅ Design responsivo e acessível (AA)
- ✅ Paleta de cores Navigator implementada
- ✅ Ícones SVG personalizados

---

**Desenvolvido com dedicação para o 10º MBA Executivo ISAG | 2024-2025**

*"A força da Navigator não está apenas no que produz, mas em como transforma recursos, conhecimento e propósito em valor para o futuro."*
