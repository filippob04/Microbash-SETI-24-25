# 💻 µBash-SETI-24-25

Microbash è una mini-shell scritta in C come progetto del laboratorio di **Sistemi di Elaborazione e Trasmissione dell’Informazione (SETI)**, a.a. 2024/2025.

## 🧑‍💻 Membri

- [Baldini Filippo](mailto:6393212@studenti.unige.it)
- [Giacomo Cerlesi](mailto:6364436@studenti.unige.it)
- [Giovanni Pio Antonuccio](mailto:5603204@studenti.unige.it)

## Scopo

L'obiettivo di Microbash è fornire un'implementazione semplificata di una shell Unix, per esercitarsi con le principali system call POSIX per la gestione dei processi.

## Funzionalità principali

- **Prompt** che mostra la directory corrente seguita da `$`
- **Parsing** dei comandi da standard input, inclusi:
  - Redirezioni (`<` e `>`) con sintassi *senza spazi*
  - Pipe (`|`) tra comandi
  - Espansione di variabili di ambiente (`$VAR`)
- **Esecuzione di comandi esterni**, con supporto per pipe e redirezioni
- **Comando built-in `cd`**, con sintassi rigida:
  - Deve essere l’unico comando della linea
  - Non può avere redirezioni o pipe

## Esempi di comandi validi

```bash
cd dir
ls -l | grep foo >out.txt
cat /proc/cpuinfo | grep processor | wc -l
```
