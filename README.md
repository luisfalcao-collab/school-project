    System.out.println("===== Sistema Escolar - Cálculo de Médias =====\n");

    // Entrada das 8 notas
    for (int i = 0; i < 8; i++) {
        System.out.print("Digite a nota " + (i + 1) + ": ");
        notas[i] = input.nextDouble();
    }

    // Cálculo das médias bimestrais (uma nota por bimestre)
    double b1 = notas[0];
    double b2 = notas[1];
    double b3 = notas[2];
    double b4 = notas[3];
    double b5 = notas[4];
    double b6 = notas[5];
    double b7 = notas[6];
    double b8 = notas[7];

    // Médias semestrais
    double semestre1 = (b1 + b2 + b3 + b4) / 4;
    double semestre2 = (b5 + b6 + b7 + b8) / 4;

    // Média final
    double mediaFinal = (semestre1 + semestre2) / 2;

    // Exibição dos resultados
    System.out.println("\n===== RESULTADOS =====");
    System.out.println("1º Bimestre: " + b1);
    System.out.println("2º Bimestre: " + b2);
    System.out.println("3º Bimestre: " + b3);
    System.out.println("4º Bimestre: " + b4);
    System.out.println("1º Semestre: " + String.format("%.1f", semestre1));
    System.out.println("----------------------");
    System.out.println("5º Bimestre: " + b5);
    System.out.println("6º Bimestre: " + b6);
    System.out.println("7º Bimestre: " + b7);
    System.out.println("8º Bimestre: " + b8);
    System.out.println("2º Semestre: " + String.format("%.1f", semestre2));
    System.out.println("----------------------");
    System.out.println("Média Final: " + String.format("%.1f", mediaFinal));

    input.close();
}
