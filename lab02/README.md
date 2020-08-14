# Tarefa sobre catálogo de componentes
> [jupyter notebook](notebook/components-01-catalog.ipynb)

# DCC Playground

## Tarefa Web Components 01
```html
<dcc-trigger label="Mundo" action="noticia/mundo/politica" value="Mundo - Política">
</dcc-trigger>

<dcc-trigger label="Brasil P" action="noticia/brasil/politica" value="Brasil - Política">
</dcc-trigger>

<dcc-trigger label="Brasil E" action="noticia/brasil/esporte" value="Brasil - Esporte">
</dcc-trigger>

<dcc-trigger label="Bahia" action="noticia/bahia/esporte" value="Bahia - Esporte">
</dcc-trigger>

<dcc-lively-talk id="doctor"
                 duration="0s"
                 character="doctor"
                 speech="News ">
  <subscribe-dcc topic="#/politica"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="nurse"
                 duration="0s"
                 character="nurse"
                 speech="News ">
  <subscribe-dcc topic="#/brasil/#"></subscribe-dcc>
  <subscribe-dcc topic="#/bahia/#"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="patient"
                 duration="0s"
                 character="patient"
                 speech="News ">
  <subscribe-dcc topic="#"></subscribe-dcc>
</dcc-lively-talk>
```
![output](images/dcc_t1.png)

## Tarefa Web Components 02
```html
<dcc-rss publish="rss/science" source="https://www.wired.com/category/science/feed">
  <subscribe-dcc topic="next_science/rss" role="step"></subscribe-dcc>
</dcc-rss>
<dcc-rss publish="rss/design" source="https://www.wired.com/category/design/feed">
  <subscribe-dcc topic="next_design/rss" role="step"></subscribe-dcc>
</dcc-rss>

<dcc-aggregator publish="aggregate/science" quantity="2">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-aggregator>

<dcc-trigger label="Science" action="next_science/rss">
</dcc-trigger>
<dcc-trigger label="Design" action="next_design/rss">
</dcc-trigger>

<dcc-lively-talk id="doctor"
                 duration="0s"
                 character="doctor"
                 speech="Agregate Science news -> ">
  <subscribe-dcc topic="aggregate/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="nurse"
                 duration="0s"
                 character="nurse"
                 speech="Science -> ">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk id="patient"
                 duration="0s"
                 character="patient"
                 speech="Design -> ">
  <subscribe-dcc topic="rss/design"></subscribe-dcc>
</dcc-lively-talk>
```
![output](images/dcc_t2.png)