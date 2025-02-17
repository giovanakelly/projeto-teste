# projeto-teste
Cadastro de disciplinas e inscrição em aulas
package planejador_de_aulas;

import java.util.Scanner;

public class saragiovana {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		Scanner sc = new Scanner(System.in);

		String data, disciplina, sala, conteudo, professor, aluno, info, mat, ftp, pm;
		;
		int q, escolha;

		System.out.println("Informe se você é aluno ou profesor: \n1 - para Professor \n2 - para Aluno");
		q = sc.nextInt();
		sc.nextLine();
		int contador = 0;

		if (q == 1) {
			System.out.println("Por favor cadastre sua aula abaixo");

			do {
				System.out.print("Nome do professor: ");
				professor = sc.nextLine();

				if (professor.trim().isEmpty()) {
					System.out.println("Digite novamente.");
				}

			} while (professor.trim().isEmpty());

			do {
				System.out.print("Nome da disciplina: ");
				disciplina = sc.nextLine();

				if (disciplina.trim().isEmpty()) {
					System.out.println("Digite novamente.");
				}

			} while (disciplina.trim().isEmpty());

			do {
				System.out.print("Número da sala: ");
				sala = sc.nextLine();

				if (sala.trim().isEmpty()) {
					System.out.println("Digite novamente.");
				}

			} while (sala.trim().isEmpty());

			do {
				System.out.print("Data da aula: ");
				data = sc.nextLine();

				if (data.trim().isEmpty()) {
					System.out.println("Digite novamente.");
				}

			} while (sala.trim().isEmpty());

			do {
				System.out.print("Nome do conteúdo: ");
				conteudo = sc.nextLine();

				if (conteudo.trim().isEmpty()) {
					System.out.println("Digite novamente.");
				}
			} while (conteudo.trim().isEmpty());

			System.out.println("\nAula cadastrada com sucesso " + professor + "!");
			System.out.println("Professor(a): " + professor);
			System.out.println("Disciplina: " + disciplina);
			System.out.println("Sala: " + sala);
			System.out.println("Data da aula: " + data);
			System.out.println("Conteúdo: " + conteudo);

		} else if (q == 2) {
			System.out.println("Informe seu nome: ");
			aluno = sc.nextLine();

			System.out.println("Digite 1 para disciplina ou 2 para sair: ");
			escolha = sc.nextInt();
			sc.nextLine();

			if (escolha == 1) {
				System.out.println("Cadastre-se abaixo");

				do {
					System.out.println("Roberta | Informatica Básica | 19:00");
					System.out.println("Deseja se cadastrar? S / N");
					info = sc.nextLine();

					if (info.toUpperCase().equals("S")) {
						contador++;
						System.out.println("Cadastro realizado!");
					} else {
						break;
					}
				} while (info.toUpperCase().equals("N"));

				do {
					System.out.println("Adriano | Matemática Básica | 19:40");
					System.out.println("Deseja se cadastrar? S / N");
					mat = sc.nextLine();

					if (mat.toUpperCase().equals("S")) {
						contador++;
						System.out.println("Cadastro realizado!");
					} else {
						break;
					}
				} while (mat.toUpperCase().equals("N"));

				do {
					System.out.println("Monique | Fundamentos e Tecnicas da Programação | 20:10");
					System.out.println("Deseja se cadastrar? S / N");
					ftp = sc.nextLine();

					if (ftp.toUpperCase().equals("S")) {
						contador++;
						System.out.println("Cadastro realizado!");
					} else {
						break;
					}
				} while (ftp.toUpperCase().equals("N"));

				do {
					System.out.println("Heles | Psicologia da Mente | 21:10");
					System.out.println("Deseja se cadastrar? S / N");
					pm = sc.nextLine();

					if (pm.toUpperCase().equals("S")) {
						contador++;
						System.out.println("Cadastro realizado!");
					} else {
						break;
					}
				} while (pm.toUpperCase().equals("N"));

				System.out.println("Cadastro realizado " + aluno + "!");
				System.out.println("Total de cadastros realizados " + contador);
			} else if (escolha == 2){
				System.out.println("Obrigado pela atenção!");
			}
			else {
				System.out.println("ERRO");
			}

		}

	}

}
