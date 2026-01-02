// CLASSES DE UM JOGO
class Heroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    atacar() {
        let ataque;

// Estrutura que decide qual ataque para o devido tipo de herói
        switch (this.tipo.toLowerCase()) {
            case "mago":
                ataque = "magia";
                break;
            case "guerreiro":
                ataque = "espada";
                break;
            case "monge":
                ataque = "artes marciais";
                break;
            case "ninja":
                ataque = "shuriken";
                break;
            default:
                ataque = "um ataque qualquer";
        }

// Saída
        console.log(`O ${this.tipo} chamado(a) ${this.nome} de idade ${this.idade} anos atacou usando ${ataque}`);
    }
}

// Variáveis de nome/idade/tipo de herói que devem ser alterados
let nomeHeroi = "Alessandra";
let idadeHeroi = 31;
let tipoEscolhido = "lutador de mma";

const heroiDeAventura = new Heroi(nomeHeroi, idadeHeroi, tipoEscolhido);


heroiDeAventura.atacar();
