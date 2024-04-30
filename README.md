# notas-atletas
Atividade 1
Bom irei explicar como a classe/função funciona. Eu gosto muito de programar e espero conseguir um emprego de Jovem Aprendiz na área tecnologica. 

Obs: sobre o resultado do calculo da média tentei deixar o resultado mais próximo possivel! Levei horas para fazer então espero que esteja funcionando corretamente ai para vocês..

PASSO A PASSO:

º class Atletas - Definição da classe atleta.
º constructor() - Definição do modo constructor, contendo nome & nota.
º obterMedia() - Definição da primeira função, obterMedia().
º this.nota.sort((a, b) => a - b) - Definição da ordem crescente das notas.
º let soma = this.nota.slice(0, 4); - Remoção das notas maiores e menores no calculo da média & Definição de variavel, e permanecendo as notas do "meio".
º let calculo = soma.reduce((a, b) => a + b, 0) - Calculo da média usando o mesmo template do this.nota.sort((a, b) => a - b ) porem adicionando adição no lugar de subtração por causa do .reduce().
º return calculo / soma.length - Retorno do calculo ja contendo divisão logo na etapa return, variavel calculo / pela variavel some, porem adicinando o .length por causa que estamos dividindo o total de notas pela quantidade de notas.
º apresentarResultados() - Logo vindo a função "apresentarResultados()" para apresentar no console, ja que estamos falando de JS e não HTML por causa disso o "console.log()", então dentro dela contendo 3 console.log(), um para o nome, um para a nota e outro para a média. 

Nome: 
console.log(`Atleta: ${this.nome}`);

Notas Obtidas:
console.log(`Notas Obtidas: ${this.nota.join(',')}`);

Média Válida:
console.log(`Média Válida: ${this.obterMedia().toFixed(2)}`);

Espaçamento de uma linha:

console.log(`\n`)

Obs: coloquei o ".toFixed()" para não deixar os números semanticamente desalinhados, fazendo com que eles apareçam os 3 primeiros digitos da média. O ".join()" para não deixar os números dentro de um array, e sim fora. Contendo uma virgula e um caractere de espaço. Por ultimo um "console.log(`\n`)" para a quebra de linha, porem uma só, para os dados dos atletas ficarem em caixas.

º Matriz dos Atletas:

let atletas = [
    new Atletas("Cesar Abascal", [10, 9.34, 8.42, 10, 7.88]),
    new Atletas("Fernando Puntel", [8, 10, 10, 7, 9.33]),
    new Atletas("Daiane Jelinsky", [7, 10, 9.5, 9.5, 8]),
    new Atletas("Bruno Castro", [10, 10, 10, 9, 9.5])
];

- Modifiquei a matriz dos atletas pondo elas como acesso de objeto ao inves de tem que usar o método ".1.1-1.1-3." etc.. adptei para o acessamento de objetos, para ficar melhor e mais curto o código legivel/prático. 

º Chamada de função, prova real:
atletas.forEach(atleta => atleta.apresentarResultados());
- Por ultimo, a chamda de função para executar o código, utilizando o método ".forEach()" para cada chamada de array ser executada e separadas em caixinhas por causa do console.log(`\n`), o (atleta => atleta.apresentarResultados()) atleta => ou >= os dois sendo válido da mesma maneira, e com a chamada da função apresentarResultados() dando nisso os consoles.logs() e o atletas para a chmada da varial de chamda de objeto então dando o código funcional. 

Estou aprendendo e tentando aprender o máximo possivel, gosto muito de programar fiquei 2 semanas sem fazer programação e agora estou voltando, porem esqueci de muita coisa. E estou tentando buscar um emprego de Jovem Aprendiz de Programação no Mercado. 

- Attenciosamente Nicholas SC. 


