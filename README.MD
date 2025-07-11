## Saludos en go

Este paquete proporciona  una forma simple de obtener saludos de personas 

## Instalacion
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/Jeskaai/greetings 
```
## Uso

Aqui tienes un ejemplo de como utilizar el paquete en tu codigo:

```go

package main

import{
    "fmt"
    "github.com/Jeskaai/greetings"
}

func main(){
    message, err := greetings.Hello("Juanes")

    if err != nil{
        fmt.Println("Ocurrio un error: ", err)
        return
    }

    fmt.println(message)
}
