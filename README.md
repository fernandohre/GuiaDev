# Guia do Desenvolvedor 1.0
Este é um guia base para que o desenvolvedor execute boas práticas de programação e saiba como lidar com adversidades durante um projeto.

## Código limpo
É de conhecimento notório que no mundo de desenvolvimento de software 80% do esforço é gasto com manutenção. Dessa forma, fica evidente que devemos codificar de forma mais clara possível para que a manutenção corretiva ou preventiva siga um fluxo contínuo sem travar o desenvolvedor. A seguir vamos visualizar a nomenclatura incoerente de um método:

```c#
public string con() {
  //Implementação do método
  //return alguma coisa
}
```

Observe que a nomenclatura do método não é condizente com o que ele se propõe a fazer, ou seja, caso um novo desenvolvedor dê manutenção nesse código, ele gastará algumas horas para entender o fluxo e além disso entender o que o método realmente se propõe a fazer. Veja só, ocorreu um esforço a mais para entendimento e não para produzir uma nova implementação.

Para que isso não aconteça, devemos pensar em nomes melhores que deixe claro o que o método se propõe a fazer. Veja a seguir:

```c#
public string obtenhaStringDeConexao() {
  //Implementação do método
  return stringDeConexao;
}
```
Observe que a nomenclatura do método já deixa claro o que ele se propõe a fazer.

## Não repita as mesmas coisas!
Geralmente em um projeto de software é comum utilizarmos a orientação a objetos para abstrair o mundo real e traduzí-lo para software. Então se queremos representar uma pessoa, criamos uma classe pessoa com seus atributos como: Nome, endereço, data de nascimento.
Se queremos representar um professor, criamos uma classe professor e colocamos seus atributos. Mas espere! é aqui que alguns de nós caimos em uma cilada e começamos a repetir alguns atributos em comum! Torna-se necessário usarmos o conceito de abstração na orientação a objetos. Então teriamos uma classe abstrata pessoa e a classe professor herda de pessoa, já que professor é uma pessoa! veja que se surgir uma terceira classe chamada: Diretor, esta também tem atributos em comuns com pessoa, logo passa a herdar de pessoa.
![Capturar](https://user-images.githubusercontent.com/12806350/66788863-a0799e80-eebf-11e9-99fe-540778bab83f.PNG)



