## Tarefa 1
> <img src="images/diagrama.png" width="1000">

## Tarefa 2
Link para o projeto no Codepen: [React 03 - Componente Barra](https://codepen.io/santanche/pen/KKzmbwR)

**HTML**
~~~html
<div id="root"></div>
~~~

**JavaScript**
~~~javascript
class Barra extends React.Component {
  render() {
    let resultado = "";
    for (let b = 1; b <= this.props.tamanho; b++)
      resultado += "=";
    return resultado;
  }
}

const elemento = <div>
                   <h2>O dinossauro</h2>
                   <Barra tamanho="10"/>
                   <h2>pulou na lama.</h2>
                 </div>
ReactDOM.render(elemento, 
        document.getElementById("root"));
~~~
