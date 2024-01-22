class Atletas {
  constructor(nome, nota){
    this.nome = nome;
    this.nota = nota;
  }
  obterMedia(){
    // Ordem crescente
    this.nota.sort((a, b) => a - b)
    // Tira as nota maior e menor
    let soma = this.nota.slice(0, 4);
    //Calculo da media
    let calculo = soma.reduce((a, b) => a + b, 0)
    //Retorno do calculo
    return calculo / soma.length
}
 apresentarResultados() {
        // Apresentação dos resultados ao usuário
        console.log(`Atleta: ${this.nome}`);
        console.log(`Notas Obtidas: ${this.nota.join(',')}`);
        console.log(`Média Válida: ${this.obterMedia().toFixed(2)}`);
        console.log('\n');
    }
}

//Matriz dos atletas
let atletas = [
    new Atletas("Cesar Abascal", [10, 9.34, 8.42, 10, 7.88]),
    new Atletas("Fernando Puntel", [8, 10, 10, 7, 9.33]),
    new Atletas("Daiane Jelinsky", [7, 10, 9.5, 9.5, 8]),
    new Atletas("Bruno Castro", [10, 10, 10, 9, 9.5])
];

// FUnção de prova real
atletas.forEach(atleta => atleta.apresentarResultados());
