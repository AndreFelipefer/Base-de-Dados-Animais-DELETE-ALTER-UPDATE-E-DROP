# Exercícios SQL para Manipulação de Dados em Animais

## Este conjunto de exercícios utiliza um arquivo SQL chamado animais.sql para realizar diversas operações em uma base de dados de animais. Os exercícios incluem a renomeação de personagens, alterações de peso e cor, adição de campos, exclusões condicionais e remoção de colunas. Siga as instruções acima para praticar e aprimorar suas habilidades em SQL!

1- Altere o nome do Pateta para Goofy:
```SQL
UPDATE animais SET nome = 'Goofy' WHERE nome = 'Pateta';
```

![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/07f0831b-4876-4aed-a72f-5ec3ef61d8d4)


2- Altere o peso do Garfield para 10 quilogramas:
```SQL
UPDATE animais SET peso = 10 WHERE nome = 'Garfield';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/b3809bd3-274c-42d1-9f31-43078125e103)

3- Altere a cor de todos os gatos para laranja:
```SQL
UPDATE animais SET cor = 'laranja' WHERE tipo = 'gato';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/413ac45b-dbef-4728-b8f7-4b4bd76614a6)

4- Crie um campo 'altura' para os animais:
```SQL
ALTER TABLE animais ADD altura DECIMAL(9, 2);
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/d26af922-0b3d-48f5-8170-02f927c549f4)

5- Crie um campo 'observação' para os animais:
```SQL
ALTER TABLE animais ADD  observacao varchar(200);
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/dc6ff5eb-202e-4ae9-b2a5-bfa6edf3629b)

6- Remova todos os animais que pesam mais que 200 quilogramas:
```SQL
DELETE FROM animais WHERE peso > 50;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/1e40b96f-b67f-4798-8144-e48500949dd5)

7- Remova todos os animais cujo nome inicie com a letra 'C':
```SQL
DELETE FROM animais WHERE nome LIKE '%C';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/a50cba85-9a4d-4a29-bf43-ad53cb72ddce)

8- Remova o campo 'cor' dos animais:
```SQL
ALTER TABLE animais DROP  cor;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/80a144f3-0c87-4b1c-a48c-840483fd5a7d)

9- Remova todos os gatos e cachorros
```SQL
DELETE FROM animais WHERE tipo IN ('gato', 'cachorro');
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/b53b5dc3-cb3f-4bbd-ae33-39c0a392e489)

10- Remover o campo data de nascimento dos animais:
```SQL
ALTER TABLE animais DROP data_nascimento;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/c4743000-d44b-4802-86b1-dcae0d9f3de9)

11- Remover todos os animais:
```SQL
DELETE FROM animais;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/c09d595c-1bbc-42dc-a8f6-fb5b1cfef825)

12- Remover a tabela especies:
```SQL
DROP TABLE especies;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais-DELETE-ALTER-UPDATE-E-DROP/assets/129207232/469ab704-1de0-4f97-bd7e-04899e03ef03)

##Obrigado!
