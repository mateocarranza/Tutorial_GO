# Tutorial GO

Go, también conocido como Golang o Google Go,es un lenguaje de programación concurrente, compilado de código abierto (open source) relativamente nuevo ya que data de once años de antigüedad hablando históricamente, donde su trayectoria ha permitido ir mejorando, puliendo y madurando todos sus detalles. Se encuentra inspirado en la sintaxis de lenguaje C y Algol, con tipado estático

## Instalación de Golang
Lo primero que hay que hacer es instalar go para ello:<br/>
 -Iremos a su página principal https://golang.org/ .<br/>
 -Tocar el botón de descargar.<br/>
 -Elegimos en qué sistemas queremos descargarlo.<br/>

también necesitaremos un editor de texto yo recomiendo visual code y es el que voy a utilizar para realizar este tutorial.

## Rest Api

Para poder entender un poco más de Go vamos a realizar una Rest Api.

Lo primero que vamos a hacer es realizar la arquitectura de nuestro proyecto.

<p align="center"> <img src="imagenes/arquitectura.:PNG" width="350"/>  </p> 

Dentro del myproyecto/main.go es donde daremos arranque a nuestra aplicación.

Dentro de de la carpeta pkg es donde pondré el resto del código, en algunos proyectos todo el código se encuentra en el directorio raíz, esto puede ocurrir porque es un proyecto pequeño.

dentro de pkg/server encontraremos todo lo necesario para que funcione nuestro server HTTP

## comencemos 
 
lo primero que vamos a hacer es arrancar nuestro servidor HTTP

<pre><code>
    package main
 
    import (
    "fmt"
    "log"
    "net/http" 
    )
 
    func main() {
        
    log.Fatal(http.ListenAndServe(":8080", nil))
    fmt.Println("Server abierto en http://localhost:8080")
 
    }
</code></pre>

