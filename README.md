# Blog do Leon Flicts

Bem-vindo(a) ao repositório do meu blog pessoal, hospedado via GitHub Pages:

🌐 [leonflicts42.github.io/blog](https://leonflicts42.github.io/blog)

---

## 📘 Sobre

Este é um site estático desenvolvido com **HTML**, **CSS** (provavelmente Sass ou similar) e **JavaScript**. O conteúdo é gerado manualmente (ou com um gerador simples) e disponibilizado através do branch `gh-pages`, o que permite hospedagem gratuita por meio do GitHub Pages.

O foco principal do blog é compartilhar:
- Tutoriais técnicos
- Reflexões pessoais
- Notícias e análises

---

## 🚀 Como rodar localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/leonflicts42/blog.git
   cd blog
   ```

2. Abra o site localmente:
   - Simples: abra o `index.html` no navegador.
   - Com servidor local (opcional):
     ```bash
     npx http-server . -c-1
     ```
     isso ajuda na navegação entre páginas via links relativos.

3. Edite e visualize suas mudanças no navegador.

---

## ✍️ Estrutura do projeto

```text
/
├── index.html         # Página inicial
├── posts/             # Publicações do blog (HTML ou MD convertidos)
│   ├── 2025-06-01-primeiro-post.html
│   └── ...
├── assets/
│   ├── css/           # Estilos (ex: styles.css)
│   ├── js/            # Scripts
│   └── images/        # Imagens usadas nos posts
├── about.html         # Página de “Sobre mim”
└── CNAME?             # (se usar domínio personalizado)
```

---

## 🧩 Como publicar mudanças

O deployment é automático via branch `gh-pages`. Basicamente:

1. Faça alterações nos arquivos HTML/CSS/JS.
2. Commit e push para o GitHub.
3. As mudanças aparecem em https://leonflicts42.github.io/blog em poucos minutos.

Se você usar outro branch (ex: `main`) e uma ação ou plugin de CI/CD para transferir o conteúdo para `gh-pages`, basta seguir o fluxo já configurado.

---

## ✅ Contribuições

Contribuições são bem-vindas! Você pode contribuir de forma simples:

- Submeta correções de texto, melhorias de layout ou performance.
- Abra issues para reportar bugs ou sugerir conteúdo.
- Envie PRs com novos posts (se desejar!).

---

## 🛠️ Tecnologias e ferramentas

- **GitHub Pages** – hospedagem sem servidor.
- **HTML**, **CSS**, **JavaScript** – base do site.
- (Opcional) pré-processadores e bundlers, conforme o repositório.

---

## 📄 Licença

Este repositório é distribuído sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 📫 Contato

Desenvolvido por **Leon Flicts**. Para sugestões ou feedbacks, crie uma issue ou entre em contato via ✉️ email: exemplo@dominio.com.

---

*Obrigado por visitar meu blog! 🚀*
