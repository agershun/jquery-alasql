jquery-alasql
=============

jQuery plugin for [Alasql](https://github.com/agershun/alasql) JavaScript database

The idea: make it simple as:
```
    $.sql('CREATE TABLE cities (city STRING, country STRING));');
    $.sql("INSERT INTO country VALUES ('Gent', 'Belgium'),('Paris', 'France'),('Beijing','Russia')");
    var people = [
      { name: 'Joan Palmer', city: 'Gent'},
      { name: 'Brenda Alba', city: 'Paris'},
      { name: 'Lee Hi', city: 'Beijing'},
    ];
    var res = $.sql('SELECT * FROM ? JOIN cities ON city WHERE country == "Belgium"', [people]);
```

