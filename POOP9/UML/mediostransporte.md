@startuml
scale 1

abstract class MediosTransporte{
    
}

class TransporteAcuatico{
    -velocidad: int
    -capacidad: String
    -cuerpoDeAgua: String
    +aumentarVelocidad(): void
    +noAventarse(): void
    +protocolosPorMareos(): void
}

class Barco{
    -puertoOrigen: String
    -puertoDestino: String
    -dias: int
    +abordadPasajeros(): void
    +tierraALaVista(): void
    +elevarAnclas(): void
}

class Trajinera{
    -nombre: String
    -lugar: String
    -fiesta: String
    +pedirMariachi(int horas): void 
    +atraccion(): void
    +vuelta(): void
}

class TransporteAereo{
    -altitud: int
    -piloto: String
    -compañia: String
    +despegar(): void
    +horasEnAire(): void
    +alertaDeTurbolencia(): void
}

class Avion{
    -destinoPais: String
    -tipo: String
    -modelo: String
    +demora(int horas): void
    +equipaje(): void 
    +aterrizaje(): void 

}

class Helicoptero{
    -recorrido: String
    -costo: int 
    -duracion: int 
    +visitaA(): void
    +observar(): void
    +descripcion(String lugar): void 
}

class TransporteTerrestre {
    -tipoDeRuta: String
    -pasajeros: int
    -velocidad: String
    +abrirPuertas(): void
    +cerrarPuertas(): void
    +velocidad(): void 
}

class Subterraneo{
    -linea: String
    -numDeLineas: int
    -tiempoDeEspera: int
    +salirDeLaUnidad(): void 
    +entrarALaUnidad(): void 
    +anunciarParada(): void 
}

class Metro{
    -estacion: String
    -direccion: String
    -numerosDeEstaciones: int 
    +alertaDeRetraso(): void 
    +alertaDeLLegada(): void
    +alertaDeFallo(): void
}

class Suburbano{
    -destino: String
    -paradero: String
    -numeroID: String
    +llegada(): void
    +vagonLLeno(): void
    +puertaProblema(): void
}

class Supraterraneo{
    -calle: String
    -Zona: String
    -paradero: String
    +salida(): void 
    +pedirParada(): void
    +pedirBajada(String lugar): void
}

class Taxi{
    -plataforma: String 
    -placa: String
    -identificacion: String
    +tarifa(): void
    +limiteDeZona(): void
    +revasar(): void
}

class Combi{
    -cantidad: int
    -destino: String
    -trafico: String
    +recorrase(): void 
    +subaleHayLugares(): void 
    +pagarPasaje(): void 
}

MediosTransporte<|-- TransporteAcuatico
TransporteAcuatico<|-- Barco
TransporteAcuatico<|-- Trajinera

MediosTransporte<|-- TransporteAereo
TransporteAereo<|-- Avion
TransporteAereo<|-- Helicoptero

MediosTransporte<|-- TransporteTerrestre
TransporteTerrestre<|-- Subterraneo
Subterraneo<|-- Metro
Subterraneo<|-- Suburbano
TransporteTerrestre<|-- Supraterraneo
Supraterraneo<|-- Taxi
Supraterraneo<|-- Combi


@enduml