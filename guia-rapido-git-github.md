# Guia Rápido Git/GitHub para Projetos

Este é um resumo dos comandos essenciais para iniciares e gerires projetos com Git e GitHub.

---

## Inicializar um novo projeto

```bash
# Inicializar repositório Git local
git init

# (Opcional) Criar README.md
echo "# nome-do-projeto" > README.md

# (Opcional) Criar .gitignore para ignorar ficheiros desnecessários
echo ".idea/" > .gitignore

# Adicionar todos os ficheiros
git add .

# Fazer o primeiro commit
git commit -m "Primeiro commit"
```

---

## Ligar ao GitHub

1. Criar um repositório no GitHub (sem README, .gitignore, nem licença).
2. Copiar URL do repositório.

```bash
# Renomear branch para main (padrão moderno)
git branch -M main

# Ligar o repositório local ao remoto no GitHub
git remote add origin https://github.com/teu-username/nome-do-repo.git

# Enviar o commit para o GitHub
git push -u origin main
```

---

## Trabalhar com alterações diárias

```bash
# Verificar estado dos ficheiros alterados
git status

# Adicionar ficheiros alterados (todos)
git add .

# Ou adicionar ficheiros específicos
git add ficheiro1 ficheiro2

# Fazer commit com mensagem explicativa
git commit -m "Mensagem descritiva da alteração"

# Enviar para o GitHub
git push
```

---

## Dicas úteis

- Usa mensagens claras nos commits, tipo:
  - "Corrigir bug no formulário de login"
  - "Adicionar funcionalidade de pesquisa"
  - "Atualizar estilos CSS para o header"

- Evita enviar ficheiros da IDE (ex: `.idea/`) incluindo-os no `.gitignore`.

- Antes de enviar, podes ver o que foi alterado com:
  ```bash
  git diff
  ```

- Para remover ficheiros já enviados e que não queres no repositório:
  ```bash
  git rm --cached ficheiro-ou-pasta
  git commit -m "Remover ficheiros desnecessários"
  git push
  ```

---

## Recursos para aprender mais

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com)
- [Pro Git Book (gratuito)](https://git-scm.com/book/en/v2)

---

Guarda este ficheiro para teres sempre à mão o fluxo básico para trabalhar com Git e GitHub!
