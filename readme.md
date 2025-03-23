class Comida {
    constructor(nome, calorias) {
        this.nome = nome;
        this.calorias = calorias;
    }

    descricao() {
        return `${this.nome} tem aproximadamente ${this.calorias} calorias.`;
    }

    comer() {
        return `Você comeu ${this.nome}!`;
    }
}

class Pizza extends Comida {
    constructor(nome, calorias, sabor) {
        super(nome, calorias);
        this.sabor = sabor;
    }

    descricao() {
        return `${this.nome} é uma pizza de ${this.sabor} com ${this.calorias} calorias.`;
    }

    comer() {
        return `Você devorou uma fatia de pizza de ${this.sabor}!`;
    }
}

class Sorvete extends Comida {
    constructor(nome, calorias, sabor) {
        super(nome, calorias);
        this.sabor = sabor;
    }

    descricao() {
        return `${this.nome} é um sorvete sabor ${this.sabor} com ${this.calorias} calorias.`;
    }

    comer() {
        return `Você saboreou um sorvete de ${this.sabor}, que delícia!`;
    }
}

const pizzaMussarela = new Pizza("Pizza de Mussarela", 285, "mussarela");
const sorveteChocolate = new Sorvete("Sorvete de Chocolate", 207, "chocolate");

console.log(pizzaMussarela.descricao());
console.log(pizzaMussarela.comer());

console.log("----------------------");

console.log(sorveteChocolate.descricao());
console.log(sorveteChocolate.comer());


