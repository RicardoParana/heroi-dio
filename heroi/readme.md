1```javascript
class Heroi {
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo;
  }

  atacar() {
    let ataque;

    switch (this.tipo) {
      case 'mago':
        ataque = 'atacou usando magia';
        break;
      case 'guerreiro':
        ataque = 'atacou usando espada';
        break;
      case 'monge':
        ataque = 'atacou usando artes marciais';
        break;
      case 'ninja':
        ataque = 'atacou usando shuriken';
        break;
      default:
        ataque = 'atacou usando shuriken';
    }

    console.log(`O ${this.tipo} atacou usando ${ataque}`);
  }
}

// Exemplo de uso
const heroiMago = new Heroi('Merlin', 100, 'mago');
const heroiGuerreiro = new Heroi('Arthur', 30, 'guerreiro');
const heroiMonge = new Heroi('Kung Fu Panda', 25, 'monge');
const heroiNinja = new Heroi('Hanzo', 28, 'ninja');

heroiMago.atacar();       // Saída: O mago atacou usando magia
heroiGuerreiro.atacar();  // Saída: O guerreiro atacou usando espada
heroiMonge.atacar();      // Saída: O monge atacou usando artes marciais
heroiNinja.atacar();      // Saída: O ninja atacou usando shuriken```