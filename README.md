# MiniretoSemana4
//: Mini reto Semana 4

import UIKit




enum Velocidades : Int {
    
    case apagado = 0
    case velocidadBaja = 20
    case velocidadMedia = 50
    case velocidadAlta = 120
    case velocidadInicial

    init ( velocidadInicial : Int ){
        
        self = . velocidadInicial
    }
}





class Auto {
    
    var velocidad : Int
    let velocidadInicial = Velocidades.apagado
    
    init ( velocidad : Int) {
        
        self.velocidad = velocidad
        
    
    
    func cambioDeVelocidad ( velocidad : Velocidades) -> ( actual : Int , VelocidadEnCadena : String){
        
        switch velocidad {
            
        case Velocidades.apagado:
            print(Velocidades.apagado , "Velocidad Baja")
            
        case Velocidades.velocidadBaja :
            print(Velocidades.velocidadBaja , "Velocidad media" )
            
        case Velocidades.velocidadMedia :
            print(Velocidades.velocidadMedia , "Velocidad Alta")
            
        default:
            print( Velocidades.velocidadAlta , "Velocidad Media")
        }
        }
    }
    




