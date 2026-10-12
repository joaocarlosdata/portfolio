# Portfólio | João Carlos — Data Analytics

Site pessoal com **HTML, CSS e JavaScript puro**, visual azul e preto e dashboard interativo de desempenho escolar.

## Estrutura

```text
portfolio_joao_carlos_vscode/
├── index.html           # Estrutura e conteúdo das páginas
├── css/
│   └── style.css        # Aparência, cores e responsividade
├── js/
│   ├── dados.js         # Base de alunos usada no navegador
│   └── script.js        # Navegação, filtros, cálculos e gráficos
├── data/
│   └── alunos.json      # Cópia estruturada dos dados para estudo
├── assets/
│   └── foto-joao.jpeg   # Fotografia do portfólio
└── README.md            # Este guia
```

## Como abrir no VS Code

1. Extraia o ZIP.
2. Abra o **Visual Studio Code** e escolha **Arquivo > Abrir Pasta**.
3. Selecione a pasta `portfolio_joao_carlos_vscode`.
4. Abra `index.html` no navegador ou use a extensão **Live Server** no VS Code.
5. Teste o menu **Sobre mim**, o dashboard e os filtros **Escola**, **Sexo**, **Internet** e **Deslocamento**.

> Os arquivos funcionam sem bibliotecas externas. `dados.js` é carregado por uma tag `<script>` em vez de `fetch()`, permitindo também abrir `index.html` localmente.

## Onde editar

- **Seu texto:** `index.html` (procure `id="sobre"`).
- **Cores:** `css/style.css` (procure `:root`).
- **Foto:** substitua `assets/foto-joao.jpeg` mantendo o nome.
- **Filtros e gráficos:** `js/script.js` (função `render`).
- **Registros dos estudantes:** `js/dados.js`. O JSON em `data/` é uma cópia para consulta.

## Publicar no GitHub Pages

Repositório: https://github.com/joaocarlosdata/portfolio

1. Envie **o conteúdo desta pasta** para a raiz do repositório (o arquivo `index.html` precisa ficar na raiz).
2. Entre em **Settings > Pages**.
3. Selecione **Deploy from a branch**, branch `main`, pasta `/(root)` e salve.
4. Após a publicação, o endereço esperado será:
https://joaocarlosdata.github.io/portfolio/

## Sobre os dados

São 395 registros anonimizados de duas escolas. A média exibida é `(G1 + G2 + G3) / 3`, na escala de 0 a 20. Comparações entre grupos indicam **associações**, não efeitos causais. Nenhum CPF ou identificador pessoal é incluído.

## Nota de manutenção

`data/alunos.json` foi separado para facilitar análises futuras. A aplicação utiliza `js/dados.js`; se atualizar os dados, mantenha ambos sincronizados.
