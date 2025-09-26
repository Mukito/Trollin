# Trollin com python

Vamos fazer um clone do Trello em Python com o framework Flet e depois implantá-lo no fly.io!
https://fly.io/


https://flet.dev/img/docs/trolli-tutorial/trolli-app.gif


O código para este tutorial pode ser encontrado aqui com commits autoexplicativos.  (https://gallery.flet.dev/trolli/#/boards)
Certifique-se de executar após a clonagem. E aqui está uma demonstração ao vivo. `pip install -r requirements.txt`

--------------------------------------------------------------------------

# Por que Flet? 
A maioria dos desenvolvedores está, sem dúvida, familiarizada com a situação de ter desenvolvido um aplicativo de console que 
acaba tendo um público mais amplo do que o pretendido originalmente, ou precisar desenvolver uma ferramenta interna para não desenvolvedores, 
mas que está destinada a ter uma pequena base de usuários e/ou uma vida útil relativamente curta. Em situações como essas, muitas vezes pode 
parecer estranho usar uma ferramenta superdimensionada, como o electron, uma estrutura rica em recursos como o flutter (ironia reconhecida!), 
ou tentar lidar rapidamente com alguma outra estrutura de plataforma cruzada, como o .NET MAUI. O que realmente gostaríamos é ser capaz de lançar uma 
interface do usuário em nossa lógica que pareça genericamente decente, tenha desempenho aceitável e, idealmente, leve menos tempo para escrever do que 
a lógica de negócios e, de preferência, na mesma linguagem em que o resto da lógica foi escrita - ou seja, uma linguagem com a qual já somos proficientes 
(atualmente a única biblioteca lançada é em Python, mas C#, As bibliotecas Typescript e Golang estão no roteiro). É exatamente isso que a plataforma Flet pretende proporcionar.

O Flet adota uma abordagem diferente para muitos novos frameworks de interface do usuário que é indiscutivelmente mais intuitivo para a maioria dos 
programadores experientes. Divergindo da abordagem declarativa atualmente onipresente e optando por um modelo imperativo.

Tendo sugerido que o Flet foi projetado com GUIs simples em mente, vamos, no entanto, tentar fazer algo um pouco mais complicado do que, por exemplo, 
um painel simples com alguns filtros, e tentar algo como uma versão mínima do Trello - e conceder a ele o nome totalmente independente, Trolli. 
Para os propósitos deste tutorial, assumirei que o leitor está familiarizado com o conceito básico e a configuração de um projeto Flet 
(leia os tutoriais e os documentos, se não) e, em vez disso, focarei mais em aspectos que não fazem parte dos tutoriais existentes.

