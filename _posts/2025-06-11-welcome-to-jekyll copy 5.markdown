---
layout: post
title: "Alô você"
date: 2025-06-13 09:00:00 +0000
categories: alo você
---

Se você está começando na programação ou já trabalha em equipes de desenvolvimento, certamente sabe que o **Git** é uma ferramenta indispensável para o controle de versão. E para facilitar sua vida, apresentamos um **resumo visual (Git Cheat Sheet)** com os comandos mais importantes para dominar o Git com eficiência e confiança.

Neste artigo, vamos explicar como usar os principais comandos do Git com base em uma tabela prática, ideal para iniciantes e desenvolvedores experientes. Vamos nessa?



## 1. Criar um Repositório Git

O primeiro passo para trabalhar com Git é criar ou clonar um repositório:

### Iniciar novo projeto:

```bash
git init
git add .
git commit -m "primeiro commit"
```

### Clonar repositório existente:

```bash
git clone <url>
```

Esses comandos criam a base do seu projeto versionado.



## 2. Exibir Alterações e Histórico

Antes de modificar qualquer coisa, é crucial saber o que foi alterado:

### Verificar status dos arquivos:

```bash
git status
```

### Comparar diferenças entre versões:

```bash
git diff
git diff <ID1> <ID2>
```

### Ver histórico de commits:

```bash
git log
```

Essas ferramentas ajudam a rastrear mudanças e entender o fluxo do projeto.



## 3. Reverter Alterações com Segurança

Errou alguma coisa? Sem problemas:

### Voltar ao último commit:

```bash
git reset --hard
```

### Desfazer último commit sem perder mudanças:

```bash
git reset --soft HEAD~1
```

### Editar o último commit:

```bash
git commit --amend
```

Com esses comandos, você consegue corrigir erros com tranquilidade.


## 4. Atualizar e Sincronizar com o Repositório Remoto

Manter seu repositório atualizado com a equipe é essencial:

### Buscar alterações remotas:

```bash
git fetch
```

### Mesclar alterações remotas:

```bash
git pull
```

### Aplicar patches:

```bash
git am
```


## 5. Trabalhar com Branches no Git

Branches são fundamentais para organizar o desenvolvimento de novas funcionalidades:

### Criar e mudar para uma nova branch:

```bash
git checkout -b minha-branch
```

### Mesclar branches:

```bash
git merge minha-branch
```

### Excluir branch:

```bash
git branch -d minha-branch
```



## 6. Resolver Conflitos de Merge

Durante um merge, conflitos são inevitáveis:

### Verificar conflitos:

```bash
git diff --base <arquivo>
git diff --ours <arquivo>
git diff --theirs <arquivo>
```

### Resolver e continuar:

```bash
git add <arquivo>
git rebase --continue
```



## 7. Publicar e Compartilhar seu Código

Pronto para compartilhar seu trabalho?

### Enviar alterações para o repositório remoto:

```bash
git push
```

### Criar uma nova tag:

```bash
git tag v1.0
```

### Gerar patch para revisão:

```bash
git format-patch origin
```

## Workflow Visual do Git

A imagem que inspirou este post resume o fluxo de trabalho ideal no Git em 8 etapas:

1. **Create** (criação do repositório)
2. **Browse** (explorar arquivos e histórico)
3. **Change** (fazer alterações)
4. **Revert** (reverter mudanças)
5. **Update** (sincronizar com o remoto)
6. **Branch** (trabalhar com branches)
7. **Commit** (confirmar mudanças)
8. **Publish** (compartilhar com o time)

![Fluxo do Git](/blog/assets/image.png "Fluxo do Git")

---
layout: post
title: "Meu Primeiro Post com Código Python no Jekyll"
date: 2025-06-13 20:30:00 -0300
categories: [programacao, python, jekyll]
tags: [python, jekyll, code, tutorial]
---

Olá a todos! Neste post, vou demonstrar como é simples inserir e destacar código Python em um blog Jekyll.

### Bloco de Código Simples (Inline Code)

Para inserir pequenos trechos de código em linha, use acentos graves (` `` `):

Um exemplo simples é `print("Olá, mundo!")`.

### Bloco de Código com Destaque de Sintaxe (Syntax Highlighting)

Para blocos de código maiores e com destaque de sintaxe, o Jekyll usa a sintaxe de [fenced code blocks](https://www.markdownguide.org/extended-syntax/#fenced-code-blocks) do Markdown, adicionando o nome da linguagem após os três acentos graves.

Aqui está um exemplo em Python:

```python
# Este é um script Python simples
def fibonacci(n):
    """
    Gera a sequência de Fibonacci até n termos.
    """
    a, b = 0, 1
    sequence = []
    while len(sequence) < n:
        sequence.append(a)
        a, b = b, a + b
    return sequence

# Chamando a função
num_terms = 10
fib_sequence = fibonacci(num_terms)
print(f"Sequência de Fibonacci com {num_terms} termos: {fib_sequence}")

# Exemplo de uso de bibliotecaaa
import requests

try:
    response = requests.get("[https://api.github.com/users/octocat](https://api.github.com/users/octocat)")
    response.raise_for_status() # Lança exceção para códigos de status de erro
    data = response.json()
    print(f"Nome do usuário: {data['name']}")
    print(f"Bio: {data['bio']}")
except requests.exceptions.RequestException as e:
    print(f"Erro ao fazer requisição: {e}")
```

