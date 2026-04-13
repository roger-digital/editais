# 🔍 Buscador de Editais Públicos

Interface HTML estática + scraper Python automatizado via GitHub Actions.

## 📁 Estrutura

```
.
├── index.html                        ← Interface (GitHub Pages)
├── data.json                         ← Dados gerados pelo scraper
├── scraper.py                        ← Script de coleta
├── requirements.txt                  ← Dependências Python
└── .github/
    └── workflows/
        └── scrape.yml                ← Atualização automática diária
```

## 🚀 Como publicar

1. Crie um repositório no GitHub (pode ser privado ou público)
2. Envie todos os arquivos para o repositório
3. Vá em **Settings → Pages → Branch: main / root** e ative o GitHub Pages
4. Acesse **Actions → Atualizar Editais → Run workflow** para rodar pela primeira vez
5. Pronto! Sua URL será: `https://SEU_USUARIO.github.io/NOME_DO_REPO/`

## ⚙️ Atualização automática

O GitHub Actions roda o `scraper.py` **todo dia às 08h (Brasília)** e atualiza o `data.json` automaticamente.

## 🔎 Fontes
- ConcursosNoBrasil.com (27 estados)
- 32 portais de Institutos Federais
