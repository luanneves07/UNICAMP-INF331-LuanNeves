# Tarefa 1
![tarefa 01](images/tarefa01.png)
# Tarefa 2
![tarefa 02](images/tarefa02.png)
### Sequência:

- O componente **ProductSelect** dispara uma mensagem no tópico IProductProducer que está assinado pelo componente **Auction**;
- Assim que a mensagem é recebida, o componente **Auction** envia uma notificação (mensagem) no tópico **IDemand** que é assinado pelo **Provider**;
- O componente **Provider** identifica que o cliente quer realizar a compra de um produto e envia uma mensagem de oferta no tópico **IOffer**;
- O tópico **IOffer** é assinado pelo componente de rankeamento **RankedProducts** que possui uma propriedade de configuração de seu estado para identificar quantos produtos serão requisitados na saída. <br/>Após realizar o cálculo, o mesmo envia uma mensagem no tópico **IRankedOffer** que é assinado pelo componente **Screen** ;
- O componente **Screen** é utilizado para armazenar as ofertas rankeadas.
- O componente **ProductView** disponibiliza uma interface para que seja possível visualizar os produtos rankeados
# Tarefa 3
## Nenhum produto selecionado
<img src="images/tela01.jpg" width="400">

## primeiro produto selecionado
<img src="images/tela02.jpg" width="400">

## segundo produto selecionado
<img src="images/tela03.jpg" width="400">

## compra de um dos produtos efetiva
<img src="images/tela04.jpg" width="400">

## Diagrama de blocos do aplicativo
![diagrama](images/diagrama.png)

## Aplicação
[DinoUnicamp](app/DinoUnicamp.aia)