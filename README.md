# Estudo do Dataset mtcars em R

Este repositório contém exercícios feitos no **RGui** utilizando o dataset `mtcars`.  
O `mtcars` é um conjunto de dados interno do R com informações sobre diferentes carros, como eficiência de combustível, potência, peso, tipo de motor e transmissão.

Abaixo está um print do resultado do comando `mtcars`, mostrando todas as linhas e colunas do dataset:

<img width="636" height="553" alt="mtcars-output png" src="https://github.com/user-attachments/assets/25bfdd29-0ddf-4981-b65c-940dee4184de" />

Abaixo está o print mostrando apenas a coluna **`wt`**, que representa o peso de cada carro em milhares de libras (1000 lbs):

<img width="773" height="85" alt="{EB6F1C81-722F-45FD-A851-65F724B9CCBC}" src="https://github.com/user-attachments/assets/5b3456e7-cd1b-4640-918e-659bdfa8aef2" />

Essa visualização permite analisar especificamente o peso dos carros, sem precisar olhar toda a tabela. Também é possível usar esses valores para criar gráficos relacionando peso e outras variáveis, como milhas por galão (mpg).


Abaixo está o cálculo da **média do peso** dos carros utilizando a função `mean()`:

<img width="654" height="54" alt="{01F3F578-5FC2-4722-B55E-015FE61C7D0F}" src="https://github.com/user-attachments/assets/06be766e-bd8c-43f3-bc6d-8d0922c6683e" />

A média do peso dos 32 carros é **3.217 (× 1000 lbs)**, ou seja, aproximadamente **1.459 kg**.  
Isso indica que o carro "médio" do dataset pesa cerca de **1.460 kg**.

Abaixo está o cálculo do **desvio padrão do peso** dos carros utilizando a função `sd()`:

<img width="648" height="51" alt="{44827EE5-C779-4922-9EA1-6ADDC046E4F4}" src="https://github.com/user-attachments/assets/017e57d9-2235-4ba3-a38f-2d632ddefdf5" />

O desvio padrão do peso é **0.978 (× 1000 lbs)**, ou seja, aproximadamente **978 lbs (~444 kg)**.  
Isso indica que os pesos dos carros variam, em média, cerca de **444 kg** em relação à média geral.

Após a instalação, foi utilizada a função `count()` do pacote `plyr` para contar os valores da coluna `wt`:

<img width="233" height="532" alt="{525F94E8-4D22-4A9C-B955-046E2961D314}" src="https://github.com/user-attachments/assets/fd52764f-52b9-454d-996b-2f5177ff418c" />

Foi gerado um gráfico de dispersão relacionando o peso (`wt`) e a eficiência de combustível (`mpg`) dos carros:

<img width="605" height="512" alt="{4A9FACB2-5C9C-4E24-BC22-11D72CD1B391}" src="https://github.com/user-attachments/assets/baf4f49d-914c-4af2-8096-b5a077de9def" />

O gráfico mostra uma **relação inversa** entre as variáveis: carros mais pesados tendem a ter menor eficiência de combustível, ou seja, fazem menos milhas por galão (mpg).



