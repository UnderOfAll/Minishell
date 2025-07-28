
# Minishell

Projeto desenvolvido como parte do currículo da 42 Lisboa.

## 🧠 Objetivo

Criar um shell funcional do zero, com comportamento similar ao bash, incluindo execução de comandos, redirecionamentos, pipes, variáveis de ambiente e comandos built-in.

## 🔧 Funcionalidades

- Execução de comandos externos (como `ls`, `grep`, `cat`, etc.)
- Comandos built-in: `cd`, `echo`, `pwd`, `export`, `unset`, `env`, `exit`
- Redirecionamentos: `>`, `>>`, `<`, `<<` (heredoc)
- Pipes entre comandos (`ls | grep x`)
- Variáveis de ambiente (`$PATH`, `$USER`, etc.)
- Expansão de variáveis dentro de strings
- Parsing com suporte a aspas simples/dobras
- Tratamento de sinais (Ctrl+C, Ctrl+\)
- Gerenciamento de processos com `fork`, `execve`, `waitpid`

## 🛠️ Como compilar

```bash
make
```

## ▶️ Como usar

```bash
./minishell
```

Depois disso, o shell está pronto para receber comandos.

## 🧪 Exemplo

```bash
$ echo Hello World
Hello World

$ ls -la | grep minishell | wc -l

$ export USER=Kayki
$ echo $USER
Kayki
```

## 📚 O que aprendi

- Execução de programas com `fork`, `execve`
- Manipulação de arquivos e redirecionamento com `dup2`
- Parsing de strings e lógica de separação de tokens
- Gerenciamento de memória e organização modular de código em C
- Como funciona um shell real "por dentro"

## 🧑‍💻 Feito por

[Kayki Rocha](https://github.com/UnderOfAll) – Estudante da 42 Lisboa
[Laher Maciel](https://github.com/LaherMaciel) - Estudante da 42 Lisboa
