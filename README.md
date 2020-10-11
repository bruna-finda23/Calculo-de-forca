# Calculo-de-forca
//
onEvent("button_limpar", "click", function( ) {
  console.log("Clicou no LIMPAR");
  setText("text_input_massa", "");
  setText("text_input_acelera", "");
  setText("label_resultado", "Resultado:");
});
onEvent("button_calcular", "click", function( ) {
  console.log("Clicou no CALCULAR");
  var massa = 0;
  var acelera = 0;
  massa = getText("text_input_massa");
  acelera = getText("text_input_acelera");
  console.log("Massa informada: " + massa);
  setText("label_resultado", "A Força é: " + (massa * acelera + " N."));
});
