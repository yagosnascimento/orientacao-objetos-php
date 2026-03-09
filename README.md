# orientacao-objetos-php
PHP Orientado a Objetos (POO) é um paradigma fundamental no desenvolvimento PHP moderno (versões 5+), estruturando o código em classes e objetos para melhorar a organização, manutenção e reutilização. Baseia-se em conceitos como encapsulamento, herança, polimorfismo e classes, e
é indispensável para o uso de frameworks e boa engenharia de software.

---
Procedural:
```
$a = 10;
$b = 20;
$operador = 'soma';

function calcular ($a, $b, $operador){
  if ($operador == 'soma'){
    return $a + $b;
  }
  return false;
}

echo calcular($a, $b, $operador);
```

Orientado a objetos:
```
class Calculadora{
  public $a = 10;
  public $b = 20;
  public $operador = 'soma';

  public function calcular(){
    if ($this->operador == 'soma'){
      return $this->a + $this->b;
      }
  }
}

$calcular = new Calculadora();
echo $calcular->calcular();
