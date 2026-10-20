# Dashboard de Vendas Interativa - Desafio Porsche

Este repositório contém a resolução do desafio prático de transformação de uma base de dados estática do Excel em uma dashboard web interativa, responsiva e totalmente publicada em nuvem sem o uso de ferramentas tradicionais de BI.

## 🔗 Link da Dashboard no Ar (inserir)
[CLIQUE AQUI PARA ACESSAR A DASHBOARD EM PRODUÇÃO](SUA_URL_DO_GITHUB_PAGES_AQUI)

---

## Perguntas de Negócio Escolhidas
Para direcionar a utilidade estratégica da tela, definimos duas perguntas principais:
1. **Faturamento Total por Marca/Modelo:** Essencial para entender qual fabricante traz a maior receita bruta e lidera o market share interno.
2. **Evolução do Volume de Vendas por Ano:** Permite identificar tendências temporais de crescimento de mercado e sazonalidade física de lotes.

---

## Tratamento e Sanitização dos Dados
A planilha base original enviada continha erros estruturais graves identificados e corrigidos manualmente antes da ingestão na IA:
- **Correção de Cabeçalhos:** Substituição de títulos genéricos automáticos (`Coluna1`, `Coluna2`) pelos nomes de negócio reais (`Modelo`, `Preço`, etc.).
- **Limpeza de Erros do Excel:** A célula correspondente ao preço da FERRARI estava quebrada apresentando `##########`. Através de cálculo reverso baseado no Faturamento Global (Dividindo Faturamento por Quantidade), identificamos e tratamos o valor puro correto de `1500000.00`.
- **Sanitização de Moeda:** Remoção de símbolos gráficos de texto (`R$`, pontos de milhar e espaços) para converter as colunas de valor e quantidades em inteiros/decimais numéricos puros calculáveis.
- **Inclusão Estratégica:** Adicionados registros de vendas reais da marca **Porsche** para contextualização ao tema do projeto.

---

## Identidade Visual (Design System)
- **Tema:** Estrito *Dark Mode Premium* focado na experiência esportiva automobilística.
- **Paleta de Cores:** Fundo grafite profundo escuro (`#141416`), painéis cinza fosco (`#1e1e22`) e detalhes visuais interativos no marcante Vermelho Porsche (`#d5001c`).
- **Arquitetura de Tecnologia:** Construído puramente utilizando HTML5 estrutural, CSS3 isolado e vanilla Javascript acoplado à biblioteca open-source `Chart.js` via CDN.
