Seminario Ruby
==============

##### Antonio Melero Bello

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

    #!/usr/bin/env usr/bin/ruby
    #Devolver informacion de cabecera HTTP
    require 'net/http'
    url = ARGV[0]
    puts "URL:" << url
    http = Net::HTTP.new(url, 80)
    respuesta = http.request_head('/')
    puts respuesta['Last-Modified'].to_s
    puts respuesta["content-type"].to_s
    puts respuesta["date"].to_s
    puts respuesta["age"].to_s
    puts respuesta["Server"].to_s

#### Ejercicio 5

Para instalar vagrant hay que ejecutar el siguiente comando:

    sudo gem install vagrant


