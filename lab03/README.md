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
# Tarefa 3
> Nenhum produto selecionado<br />
![Tela 01](images/tarefa03_tela01.png)<br />
> primeiro produto selecionado<br />
![Tela 02](images/tarefa03_tela02.png)<br />
> segundo produto selecionado<br />
![Tela 03](images/tarefa03_tela03.png)<br />
> compra de um dos produtos efetiva<br />
![Tela 04](images/tarefa03_tela04.png)<br />
> diagrama de blocos do aplicativo<br />
![Tela 05](images/tarefa03_tela05.png)<br />