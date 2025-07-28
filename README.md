
# Minishell

Project developed as part of the 42 Lisboa curriculum.

## 🧠 Objective

Implement a basic shell from scratch that replicates core Unix shell behaviors, including command execution, redirections, pipes, environment variables, and built-in commands.

## 🔧 Features

- Execution of external commands (e.g., `ls`, `grep`, `cat`, etc.)
- Built-in commands: `cd`, `echo`, `pwd`, `export`, `unset`, `env`, `exit`
- Redirections: `>`, `>>`, `<`, `<<` (heredoc)
- Piping between commands (`ls | grep something`)
- Environment variable expansion (`$PATH`, `$USER`, etc.)
- Parsing with support for single and double quotes
- Signal handling (`Ctrl+C`, `Ctrl+\`)
- Process management using `fork`, `execve`, `waitpid`

## 🛠️ How to Compile

```bash
make
```

## ▶️ How to Use

```bash
./minishell
```

The shell will be ready to accept commands.

## 🧪 Example

```bash
$ echo Hello World
Hello World

$ ls -la | grep minishell | wc -l

$ export USER=Kayki
$ echo $USER
Kayki
```

## 📚 What I Learned

- Process management with `fork`, `execve`
- File redirection using `dup2`
- String parsing and tokenization logic
- Signals management through processes
- Memory management and modular C design
- A deeper understanding of how Unix shells work internally

## 🧑‍💻 Author

[Kayki Rocha](https://github.com/UnderOfAll) – 42 Lisboa Student
[Laher Maciel](https://github.com/LaherMaciel) - 42 Lisboa Student
