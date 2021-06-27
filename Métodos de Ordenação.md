
# Métodos de Ordenação
## Matheus Marques 

[![N|Solid](https://media.giphy.com/media/XD9o33QG9BoMis7iM4/giphy.gif)](https://nodesource.com/products/nsolid)
## Temos como principais métodos de ordenação os seguintes elementos abaixo:👇

- Bubble sort,  Selection Sort, Quick sort, Insertion sort.
 
# Mas oque é ordenação?🤔
Ordenação é o ato de se inserir os elementos de uma sequência de informações, ou dados, em uma ordem predefinida. O termo técnico em inglês para ordenação é sorting, que a tradução significa "classificação".

# Bubble Sort👻
- Ou ordenação por flutuação (literalmente "por bolha"), é um dos mais simples. A ideia é percorrer o vetor diversas vezes, e a cada passagem fazer flutuar para o topo o maior elemento da sequência. Essa movimentação lembra a forma como as bolhas em um tanque de água procuram seu próprio nível, e disso vem o nome do algoritmo. 

# Exemplos de execução👨🏼‍💻
-  O Bubble sort pode ser aplicado em Arrays e Listas dinâmicas. Se o objetivo é ordenar os valores em forma decrescente, então, a posição atual é comparada com a próxima posição e, se a posição atual for maior que a posição posterior, é realizada a troca dos valores nessa posição. Caso contrário, não é realizada a troca, apenas passa-se para o próximo par de comparações. 
 Lembrando também que ele não é um algoritmo muito eficiente, é estudado para fins de desenvolvimento de raciocínio.

# Exemplo de implementação 🧛🏼‍♂️ 
[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858155233485651968/unknown.png)](https://nodesource.com/products/nsolid)

# Selection sort 👨🏼‍🦽
O Selection Sort segue uma rotina bem simples e direta: encontrar o menor elemento e colocá-lo na primeira posição. A ordenação nada mais é do que aplicar essa rotina repetidas vezes para o restante do array.

Assim como no Bubble Sort, é necessário para cada item da lista percorrê-la toda (logo, serão necessários dois loops: um para cada elemento da lista e outro para cada um desses elementos percorrer toda a lista).

Suas principais vantagens estão na fácil implementação do algoritmo, além de ocupar pouca memória se comparado com os outros algoritmos😢.
E sua principal desvantagem é o seu longo tempo de  execução.

# Exemplos de execução 🤓 
Para entender melhor a ideia que algoritmo é aplicado ao invés de uma lista, pense que temos duas sublistas: uma sublista que está ordenada e outra que está desordenada.

[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858161583666757642/unknown.png)](https://nodesource.com/products/nsolid)
Assim como no bubble sort ele pode ser aplicado em Arrays e listas dinâmicas, embora também como no exemplo anterior Trata-se de um algoritmo simples, voltado mais  para estudos e ordenação de pequenos arranjos.
# Exemplo de implementação 🤯
[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858162935725424680/unknown.png)](https://nodesource.com/products/nsolid)

# Insertion sort😌
Insertion Sort, ou ordenação por inserção, é um algoritmo de ordenação que, dado uma estrutura (array, lista) constrói uma matriz final com um elemento de cada vez, uma inserção por vez. Assim como algoritmos de ordenação quadrática, neste algoritmo a lista é percorrida da esquerda para a direita, à medida que avança vai deixando os elementos mais à esquerda ordenados.

O algoritmo funciona da mesma forma que as pessoas usam para ordenar cartas em um jogo de baralho como o pôquer.
[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858164250412318754/unknown.png)](https://nodesource.com/products/nsolid)
# Exemplo de implementação 🤭
O Insertion sort é um algoritmo simples e eficiente quando aplicado em pequenas listas.
E também é o mais rápido entre os outros métodos considerados básicos (Bubblesort e Seleção Direta).
[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858165522200789012/unknown.png)](https://nodesource.com/products/nsolid)

# Quick sort
O Quicksort é o algoritmo mais eficiente na ordenação por comparação. Nele se escolhe um elemento chamado de pivô, a partir disso é organizada a lista para que todos os números anteriores a ele sejam menores que ele, e todos os números posteriores a ele sejam maiores que ele. Ao final desse processo o número pivô já está em sua posição final. Os dois grupos desordenados recursivamente sofreram o mesmo processo até que a lista esteja ordenada.
[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858167936832634930/unknown.png)](https://nodesource.com/products/nsolid)

# Exemplos de execução
O quick sort certamente é o algoritmo mais eficiente em listas totalmente desordenadas, ele se torna muito eficiente em relação aos outros no quesito de tempo. Na lista de ordem 3 e na de ordem 2 a diferença de tempo do quick sort em comparação aos outros é muito grande.

# algoritmo que exemplifica o modelo proposto:
      public class QuickSort {
     static void Vector(int n) {
    n = 10000;
    int array[] = new int[n];
}
# b) Como gerar 10000 números aleatórios e colocá-los em um array 
static void numerosAleatorios() {

    int i = (int) (1 + Math.random() * 10000);
}
# c) Como medir o tempo de execução de um método 

static void tempoExecucao() {
    long inicio = System.currentTimeMillis();
    long fim = System.currentTimeMillis() - inicio;

}
# d) Como ordenar um array com o algoritmo 1 e totalizar a quantidade de trocas no algoritmo 1 
static void quickSort(int vetor[]) {
    quickSort(vetor, 0, vetor.length - 1);
}

static void quickSort(int vetor[], int i, int s) {
    int e = i, d = s;
    int item = vetor[((e + d) / 2)];
    while (e <= d) {
        while (vetor[e] < item) {
            e++;
        }
        while (vetor[e] < item) {
            d++;
        }
        if (e <= d) {
            int aux; //Variável auxlixar para as trocas
            aux = vetor[e];
            vetor[e] = vetor[d];
            vetor[d] = aux;
            d--;
            e++;
        }
    }
    if (d - i > 0) {
        quickSort(vetor, i, d);
    }
    if (s - e > 0) {
        quickSort(vetor, e, s);
    }
}
}
algoritmo que exemplifica o modelo proposto:
public class QuickSort {
   static void Vector(int n) {
    n = 10000;
    int array[] = new int[n];
}
## b) Como gerar 10000 números aleatórios e colocá-los em um array 

static void numerosAleatorios() {

    int i = (int) (1 + Math.random() * 10000);

}
## c) Como medir o tempo de execução de um método 

static void tempoExecucao() {
    long inicio = System.currentTimeMillis();
    long fim = System.currentTimeMillis() - inicio;


}

## d) Como ordenar um array com o algoritmo 1 e totalizar a quantidade de trocas no algoritmo 1 
static void quickSort(int vetor[]) {
    quickSort(vetor, 0, vetor.length - 1);
}

static void quickSort(int vetor[], int i, int s) {
    int e = i, d = s;
    int item = vetor[((e + d) / 2)];
    while (e <= d) {
        while (vetor[e] < item) {
            e++;
        }
        while (vetor[e] < item) {
            d++;
        }
        if (e <= d) {
            int aux; //Variável auxlixar para as trocas
            aux = vetor[e];
            vetor[e] = vetor[d];
            vetor[d] = aux;
            d--;
            e++;
        }
    }
    if (d - i > 0) {
        quickSort(vetor, i, d);
    }
    if (s - e > 0) {
        quickSort(vetor, e, s);
    }
}
}
[![N|Solid](https://cdn.discordapp.com/attachments/750712207461056563/858170138855342080/unknown.png)](https://nodesource.com/products/nsolid)

