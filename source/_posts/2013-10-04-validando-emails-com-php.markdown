---
layout: post
title: "Validando emails com PHP"
date: 2013-10-04 21:07
comments: true
categories: php
author: Danilo Lima
---

Cansado de escrever funções extensas em javascript ou montar expressões regulares para validar emails na sua aplicação?
Saiba que o PHP oferece uma opção bastante simples para isso!

É a constante _FILTER_VALIDATE_EMAIL_, da função *filter_var()*. Veja abaixo como usar

``` php Validando emails https://gist.github.com/dflima/6832922
$email = "me@example.com";

if(filter_var($email, FILTER_VALIDATE_EMAIL)) {
    echo "Email válido.";
}
```

Por hoje é só. Até a próxima!
