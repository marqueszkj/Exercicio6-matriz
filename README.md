# Controle de Vendas por Produto

## Sobre a solução

O programa foi desenvolvido em linguagem C e registra as vendas de **3 produtos** ao longo de **4 dias**. O usuário digita a quantidade vendida de cada produto em cada dia, e o programa calcula o total vendido de cada produto e o total geral de unidades.

### Como funciona

1. As quantidades são guardadas em uma matriz `vendas[3][4]`, em que cada linha é um produto e cada coluna é um dia.
2. A leitura é feita produto por produto: primeiro os 4 dias do produto 1, depois os 4 dias do produto 2, e assim por diante.
3. Durante a leitura, cada quantidade é somada ao vetor `total_produto`, e o total de cada produto é somado ao `total_geral`.
4. Ao final, o programa exibe o total de cada produto e o total geral.

### Recursos utilizados

- Matriz bidimensional (`int vendas[3][4]`) para armazenar as vendas
- Vetor (`int total_produto[3]`) para guardar o total de cada produto
- Dois laços `for` aninhados para percorrer produtos e dias
- `scanf()` para entrada de dados e `printf()` para exibir os resultados

## Como compilar e executar

```bash
gcc vendas.c -o vendas
./vendas
```

## Exemplo de execução

Entrada (4 valores por produto, na ordem dos dias):

```
Digite a qte do xº produto no yº dia:
10 20 30 40
5 5 5 5
1 2 3 4
```

Saída:

```
Saída:
Produto 1: 100 unidades
Produto 2: 20 unidades
Produto 3: 10 unidades
Total geral: 130 unidades
```
