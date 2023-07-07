# nasm-sb
Repositório de NASM para a disciplina de software 

# Integrantes G1

180076272 - Jonas de Souza Fagundes

190031891 - Kayran Vieira de Oliveira

200043722 - Thais Fernanda de Castro Garcia

190034084 - Marcus Vinicius Oliveira de Abrantes

160125260 - Ingrid Lorraine Rodrigues da Silva

190126892 - Thiago Elias dos Reis

# NASM
Repositório de duas tarefas:

Pré-processador:
- 2 - Construa macros para simular o comando switch em C
  
Montador NASM:
- 1 - Exemplifique como debugar um programa em NASM usando um software de debug

## Baixando o GDB
Para baixar o GDB em distribuições Debian/Ubuntu:
```
sudo apt-get install gdb
```
## Debug utilizando o GDB

Criando um executável do programa:
```
nasm -f elf64 -o exemplo.o exemplo.asm
ld exemplo.o -o exemplo
```
Após compilar o programa em Assembly, rode o GDB:
```
gdb -q exemplo
```
Os breakpoints são definidos usando o comando `break` ou `b`. Para gerar um breakpoint em uma label ou linha, use o seguinte comando:
```
break <linha>   # ou break <nome-da-label> 
```
Após definição dos breakpoints, execute o programa com o comando: 
```
run
```
Para a visualização da interface pelo terminal:
```
layout asm
```
