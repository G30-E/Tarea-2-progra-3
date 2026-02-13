Algoritmo SegundoMayorMenor(arreglo):
    mayor = -∞
    segundoMayor = -∞
    menor = +∞
    segundoMenor = +∞

    Para cada número en arreglo:
        // Actualizar mayores
        Si número > mayor:
            segundoMayor = mayor
            mayor = número
        Sino si número > segundoMayor Y número != mayor:
            segundoMayor = número

        // Actualizar menores
        Si número < menor:
            segundoMenor = menor
            menor = número
        Sino si número < segundoMenor Y número != menor:
            segundoMenor = número

    Retornar (segundoMayor, segundoMenor)