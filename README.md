# Kotlin Parking Lot
Proyecto de evaluación para el título de Kotlin Developer en Jetbrains Academy. Consiste en realizar un parking con las especificaciones

[![Kotlin](https://img.shields.io/badge/Code-Kotlin-blueviolet)](https://kotlinlang.org/)
[![LISENCE](https://img.shields.io/badge/Lisence-MIT-green)]()
![GitHub](https://img.shields.io/github/last-commit/joseluisgs/Kotlin-ParkingLot)


![imagen](https://www.adesso-mobile.de/wp-content/uploads/2021/02/kotlin-einfu%CC%88hrung.jpg)

## Acerca de
Este proyecto de la academia Jetbrains fue realizado con el fin de evaluar la capacidad de desarrollo de Kotlin. Consiste en jugar con un Parking

- [Kotlin Parking Lot](#kotlin-parking-lot)
  - [Acerca de](#acerca-de)
  - [Enunciado](#enunciado)
    - [Parte 1](#parte-1)
      - [Description](#description)
    - [Parte 2](#parte-2)
      - [Description](#description-1)
    - [Parte 3](#parte-3)
      - [Description](#description-2)
    - [Parte 4](#parte-4)
      - [Description](#description-3)
    - [Parte 5](#parte-5)
      - [Description](#description-4)
  - [Autor](#autor)
    - [Contacto](#contacto)
  - [Licencia](#licencia)

## Enunciado
### Parte 1
#### Description
Parking lots are an urban necessity. They provide places for you to leave your car without having to worry about it being stolen or towed. Modern car parking systems are automated and are capable of self-management. In this project, you will create a similar system, but in a simplified form.

Let's start by writing a program that can place your car in a parking lot and free the lot when the car leaves. This will be the "skeleton" of our functional parking lot, and we’ll add on to it in the following steps. At busy times, the parking lot may run out of vacant spaces. The program will provide us with aggregated information about the current state of the lot.


### Parte 2
#### Description
At this stage, our minimalistic parking lot has two parking spots. Let's assume that the first spot is occupied and the second one is free.

The parking lot should allow the user to park the car. This is implemented using the park command. After the user has entered this command, the registration number and the color of the car should be specified. For example, park KA-01-HH-1234 Blue. The registration number should not contain spaces. The color can be written in either uppercase and lowercase letters.

As the first spot is already taken, the program should allocate the second spot and print: Blue car parked in spot 2. The color should match what the user inputs.

To pick up the car, the user should print the command leave and then the number of the parking spot, for example, leave 1. If there is no car in the given spot, the program should print an error: There is no car in spot 1. Otherwise, it should notify the user that the spot is now available: Spot 1 is free.

### Parte 3
#### Description
Two spots are not enough for a parking lot, so let's increase the number of parking spaces. We'll jump straight to 20 spaces, numbered from 1 to 20. Initially, all the spots are vacant.

When the user wants to park the car, the program should find an available parking spot with the lowest number.

The user can write commands park and leave repeatedly and type exit to end the program.

If the parking lot is full and there's no room, the program should type Sorry, the parking lot is full..

If there are several available spots for a car, the program should always assign the spot with the lowest number.

### Parte 4
#### Description
In real life, parking lots vary in size. At this stage, we will get better at making art imitate life. To do this, we will make our program customizable by adding a create command that allows the user to specify the number of spots. For example, the command create 3 makes a parking lot with three spots. The number of spots should be positive. The program output should be the following: Created a parking lot with 3 spots.

Other commands like park or leave should return an error Sorry, a parking lot has not been created. until the user enters the create command. If the user calls create again, the previous parking state should be reset.

It is also important to keep track of which spaces are occupied by which cars. For this, add a status command that prints all occupied spots in ascending order. For each spot, it should print the spot number, the car’s plate registration number, and the color of the car, all separated by spaces like the example below. If there are no occupied spots, the program should print: Parking lot is empty.


### Parte 5
#### Description
The command reg_by_color prints all registration numbers of cars of a particular color, taking color as a parameter. The color may be written in uppercase or lowercase letters. For example, reg_by_color BLACK. The answer should contain registration numbers separated by commas. The order should be the same as in the status command. If there are no cars of this color, the output should be like this: No cars with color BLACK were found..

The command spot_by_color is similar to the previous one, but it prints the parking space numbers of all the cars of a particular color.

The command spot_by_reg returns you the number of the spot where a car is located based on its registration number, for example, spot_by_reg KA-01. This command will also return an error message if your car was not found: No cars with registration number KA-01 were found. For convenience, let's suppose that all car registration numbers are unique.

## Autor

Codificado con :sparkling_heart: por [José Luis González Sánchez](https://twitter.com/joseluisgonsan)

[![Twitter](https://img.shields.io/twitter/follow/joseluisgonsan?style=social)](https://twitter.com/joseluisgonsan)
[![GitHub](https://img.shields.io/github/followers/joseluisgs?style=social)](https://github.com/joseluisgs)

### Contacto
<p>
  Cualquier cosa que necesites házmelo saber por si puedo ayudarte 💬.
</p>
<p>
    <a href="https://twitter.com/joseluisgonsan" target="_blank">
        <img src="https://i.imgur.com/U4Uiaef.png" 
    height="30">
    </a> &nbsp;&nbsp;
    <a href="https://github.com/joseluisgs" target="_blank">
        <img src="https://cdn.iconscout.com/icon/free/png-256/github-153-675523.png" 
    height="30">
    </a> &nbsp;&nbsp;
    <a href="https://www.linkedin.com/in/joseluisgonsan" target="_blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/ca/LinkedIn_logo_initials.png/768px-LinkedIn_logo_initials.png" 
    height="30">
    </a>  &nbsp;&nbsp;
    <a href="https://joseluisgs.github.io/" target="_blank">
        <img src="https://joseluisgs.github.io/favicon.png" 
    height="30">
    </a>
</p>


## Licencia

Este proyecto está licenciado bajo licencia **MIT**, si desea saber más, visite el fichero [LICENSE](./LICENSE) para su uso docente y educativo.