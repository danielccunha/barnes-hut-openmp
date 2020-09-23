# Trabalho Barnes Hut

Implementação da paralelização do problema Galaxy na matéria de Programação Paralela e Distribuída. Esse repositório possui o código na pasta **src** e os dados relatados no relatório na pasta **data**.

## Compilação

```sh
cd src
gcc barnes_hut.c -o main.out -lm -fopenmp
```

## Execução

Dentro da pasta _src_ tem o arquivo **in.txt**. Este é o input do algoritmo, atualmente usando a entrada informada no enunciado do trabalho. O algoritmo permite a execução utilizando 1, 2, 4, 8 ou 16 threads, de acordo com a entrada.

O programa opcionalmente recebe dois parâmetros, o primeiro sendo o número de threads e o segundo o nome do arquivo. Segue exemplos de uso do programa, especificando o número de threads e passando os dados de input (sem informar o arquivo):

```sh
# 1 thread
./main.out < in.txt

# 2 threads
./main.out 2 < in.txt

# 4 threads
./main.out 4 < in.txt

# 8 threads
./main.out 8 < in.txt

# 16 threads
./main.out 16 < in.txt
```
