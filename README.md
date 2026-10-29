# 🎓 Gerador de Capa para Google Classroom

Aplicação web interativa, leve e sem necessidade de instalação para geração, personalização e exportação de capas/banners oficiais no formato do **Google Classroom** (proporção padrão ~4:1), desenvolvida para cursos do **SENAI São Paulo**.

---

## 🚀 Funcionalidades

### 📝 1. Personalização dos Dados do Curso
- **Título do Curso**: formatação inteligente que aplica automaticamente gradiente moderno caso contenha termos como "IA" ou "Inteligência Artificial".
- **Tipo de Curso**: ex: *Aperfeiçoamento Profissional*, *Qualificação*, etc.
- **Carga Horária**: exibição visual acompanhada de ícone de relógio.
- **Nome do Professor / Docente**: faixa dedicada logo abaixo da carga horária com efeito translúcido (*glassmorphism*). Se o campo for deixado em branco, a faixa é ocultada automaticamente.
- **Identificação da Turma e Período**: ex: *Turma 2026 / Noturno*.
- **Área / Segmento**: ex: *TI - Software*, *Mecânica*, *Gestão*, etc.

### 🎨 2. Controle de Fundo da Capa
- **Presets Rápidos**:
  - 🟢 **Verde Excel** (Padrão)
  - 🔵 **Azul Tecnologia**
  - 🟣 **Roxo IA Generativa**
  - 🔴 **Vermelho SENAI**
  - ⚫ **Grafite Minimalista**
- **Cores Personalizadas Livres**:
  - Seletor de cores nativo (*Color Picker*) para escolha livre.
  - Suporte a **Gradiente Diagonal** (com Cor Inicial e Cor Final) ou **Cor Sólida Única**.

### 🧩 3. Caixas em Destaque (`icon-box`)
- **Quantidade Flexível**: escolha entre **0 (nenhuma), 1, 2, 3 ou 4 caixas**. O layout e os tamanhos dos cartões adaptam-se dinamicamente (`normal`, `compact` e `mini`).
- **Ícone PNG do Computador**: botão para selecionar qualquer imagem/ícone direto do seu PC (PNG, SVG, JPG, WebP), com prévia e botão de remoção.
- **Emojis com Atalhos**: campo para digitar/colar emojis com paleta de atalhos rápidos de 1 clique (📊, 🤖, 💻, 📈, ⚡, 🧠, 💡, 🐍, 🚀, 🎯).
- **Legenda**: texto em caixa alta personalizável abaixo de cada ícone.
- **Cores Individuais**: defina a cor de fundo e a cor da borda/destaque de cada caixa separadamente.

### 💾 4. Exportação em Alta Resolução
- **Download em PNG**: renderização nítida em alta densidade de pixels (escala 3x) utilizando `html2canvas`.
- **Imprimir / Salvar em PDF**: folhas de estilo prontas para impressão otimizada via navegador (`@media print`).

---

## 📂 Estrutura de Arquivos

```text
capa-classroom/
├── capa_para_google_classroom_excel_ia.html   # Aplicação completa (HTML, CSS e JS)
└── README.md                                  # Documentação do projeto
```

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 & CSS3**: layout moderno com Flexbox, CSS Grid e efeitos visuais Glassmorphism.
- **JavaScript Vanilla**: manipulação reativa do DOM e carregamento de imagens locais via `FileReader API`.
- **[html2canvas (v1.4.1)](https://html2canvas.hertzen.com/)**: captura do canvas e conversão para imagem PNG sem perda de qualidade.
- **[Font Awesome 6](https://fontawesome.com/)**: ícones vetoriais da interface e do banner.
- **[Google Fonts - Inter](https://fonts.google.com/specimen/Inter)**: tipografia moderna e legível.

---

## 💻 Como Utilizar

1. Dê um duplo clique no arquivo [`capa_para_google_classroom_excel_ia.html`](file:///Users/rafael.selvagio/Projetos/MyApps/SoftwaresIA/capa-classroom/capa_para_google_classroom_excel_ia.html) para abri-lo em qualquer navegador (Google Chrome, Microsoft Edge, Firefox, Safari ou Brave).
2. Utilize o painel **"Personalizar Dados da Capa"** para inserir as informações da sua turma.
3. Escolha a cor de fundo e configure as caixas de destaque com emojis ou imagens PNG do seu computador.
4. Clique no botão **"Baixar Capa em PNG"** no topo da página.
5. No Google Classroom, abra a sua turma, clique em **"Personalizar" > "Fazer upload de foto"** e envie o arquivo PNG gerado.

