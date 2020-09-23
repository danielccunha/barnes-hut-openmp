# Trabalho Galaxy

Implementação da paralelização do problema Galaxy na matéria de Programação Paralela e Distribuída. Esse repositório possui o código na pasta **src** e os dados relatados no relatório na pasta **data**.

## Compilação

```sh
cd src
gcc barnes_hut.c -o main.out -lm -fopenmp
```

## Execução

Dentro da pasta *src* tem o arquivo **in.txt**. Este é o input do algoritmo, atualmente usando a entrada informada no enunciado do trabalho.

O algoritmo permite a execução do utilizando 1, 2, 4, 8 ou 16 threads, de acordo com a entrada. Segue exemplos de uso do programa:

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
