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
