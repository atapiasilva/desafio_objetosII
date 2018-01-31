class Carta

    attr_reader :numero, :pinta
    def initialize(pin, num)
        @pinta = pin
        @numero = num
    end

end

cartapin = ['diamante','espadas','corazones','trebol']
cartanum = [1,2,3,4,5,6,7,8,9,10, 'J', 'Q', 'K']
opciones = 0

array = []


while opciones !=4
    puts 'Jugar'
    puts 'Mostrar'
    puts 'Salir'
    puts 'Jugar'

    opciones = gets.chomp

    case opciones
        when 'jugar'
            j1= Carta.new(cartapin.sample, cartanum.sample)
            array.push(j1)
            puts "Su pinta es #{j1.pinta} y su numero es #{j1.numero}"
            j2 = Carta.new(cartapin.sample, cartanum.sample)
            array.push(j2)
            puts "Su pinta es #{j2.pinta} y su numero es #{j2.numero}"
            j3 = Carta.new(cartapin.sample, cartanum.sample)
            array.push(j3)
            puts "Su pinta es #{j3.pinta} y su numero es #{j3.numero}"
            j4 = Carta.new(cartapin.sample, cartanum.sample)
            array.push(j4)
            puts "Su pinta es #{j4.pinta} y su numero es #{j4.numero}"
            j5= Carta.new(cartapin.sample, cartanum.sample)
            array.push(j5)
            puts "Su pinta es #{j5.pinta} y su numero es #{j5.numero}"

        when 'mostrar'
            array.each do |e|
                puts "#{e.pinta} #{e.numero}"
            end

        when 'salir'  
            break

        when 'jugar'
            array = []
            j1= Carta.new(cartapin.sample, cartanum.sample)
            array.push(j1)
            puts "Su pinta es #{j1.pinta} y su numero es #{j1.numero}"
            j2 = Carta.new(cartapin.sample, cartanum.sample)
            array.push(j2)
            puts "Su pinta es #{j2.pinta} y su numero es #{j2.numero}"
            j3 = Carta.new(cartapin.sample, cartanum.sample)
            array.push(j3)
            puts "Su pinta es #{j3.pinta} y su numero es #{j3.numero}"
            j4 = Carta.new(cartapin.sample, cartanum.sample)
            array.push(j4)
            puts "Su pinta es #{j4.pinta} y su numero es #{j4.numero}"
            j5= Carta.new(cartapin.sample, cartanum.sample)
            array.push(j5)
            puts "Su pinta es #{j5.pinta} y su numero es #{j5.numero}"

    end


end           
