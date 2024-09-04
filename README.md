# Calculadora de IMC

Esta é uma simples calculadora de Índice de Massa Corporal (IMC) desenvolvida em PHP. O IMC é uma medida internacional usada para calcular se uma pessoa está no peso ideal, abaixo do peso ou acima do peso.

## Como funciona

A função `calcularIMC` recebe o peso (em quilogramas) e a altura (em metros) de uma pessoa e retorna o IMC correspondente.

### Fórmula do IMC

\[
IMC = \frac{peso}{altura^2}
\]

### Exemplo de uso

```php
<?php
function calcularIMC($peso, $altura) {
    if ($altura <= 0) {
        return "Altura deve ser maior que zero.";
    }

    $imc = $peso / ($altura * $altura);
    return $imc;
}

// Exemplo de uso:
$peso = 70; // em kg
$altura = 1.75; // em metros

$imc = calcularIMC($peso, $altura);
echo "O IMC é: " . number_format($imc, 2);
?>
```
Acesso à Calculadora Online
Você pode acessar a calculadora online através deste link: [Calculadora de IMC](http://calculadoraimc.rf.gd/?i=1)
