Seminario Ruby
==============

#### Ejercicio 1

Instalar Ruby y usar ruby--version para comprobar la versión instalada. Instalar tambien irb, rubygems y rdoc.

> sudo apt-get install ruby1.9.3

Aqui compruebo la versión instalada:

![captura1](https://dl.dropbox.com/s/j8zqm3k0p4f7fmx/version_ruby.png)

#### Ejercicio 2

Crear un programa en Ruby que imprima los números desde el 1 hasta otro contenido en una variable.

    #!/usr/bin/ruby
    for i in(0..9)
        puts i
    end

#### Ejercicio 3

¿Se pueden crear estructuras de datos mixtas en Ruby? Crear un array de hashes de arrays e imprimirlo.

    arrays = { 
            :a => ['a','e'],
            :b => ['i','o'],
            :c => ['u','son','las','vocales']
    }
    puts arrays.inspect
    
#### Ejercicio 4

Crear una serie de funciones instanciadas con un URL que devuelvan algún tipo de información sobre el mismo: fecha de última modificación, por ejemplo. Pista: esa información está en la cabecera HTTP que devuelve

#### Ejercicio 5
