Visão Geral
Este é um aplicativo web interativo que funciona como uma Pokédex digital, exibindo detalhes de Pokémon (até a 1ª geração). Ele consome a PokeAPI para buscar dados em tempo real 
e apresenta informações como tipos, estatísticas, habilidades e descrições.

Principais Características
1. Funcionalidades
Detalhes Completos: Mostra nome, ID, imagem, peso, altura, tipos, habilidades e estatísticas (HP, ATK, DEF, etc.).

Navegação entre Pokémon: Setas para avançar/retroceder na lista.

Design Responsivo: Adapta-se a diferentes tamanhos de tela.

Dinâmica de Cores: Cores do tema mudam conforme o tipo do Pokémon.

2. Tecnologias Usadas
Frontend: HTML5, CSS3 e JavaScript.

API: PokeAPI (para dados e imagens).

Bibliotecas:

Font Awesome (ícones).

Normalize.css (padronização de estilos entre navegadores).

3. Fluxo do Código
Inicialização:

Obtém o ID do Pokémon da URL (ex: detail.html?id=25 → Pikachu).

Valida se o ID está entre 1 e 151.

Busca de Dados:

Faz chamadas paralelas à PokeAPI para buscar informações do Pokémon (pokemon) e da espécie (pokemon-species).

Renderização:

Preenche o DOM com os dados (imagem, nome, tipos, etc.).

Aplica cores dinâmicas baseadas no tipo primário do Pokémon.

Navegação:

Atualiza a URL e recarrega os dados ao clicar nas setas.

Destaques Técnicos

HTML
Semântica: Uso de <main>, <header>, e <progress>.

Acessibilidade Básica: Ícones com aria-label (poderia ser expandido).

CSS
Variáveis CSS: Para tipografia e sombras consistentes.

Flexbox: Layouts responsivos sem dependência de frameworks.

Pseudo-elementos: Como divisores entre seções (:before).

JavaScript
Async/Await: Para chamadas assíncronas à API.

Manipulação Dinâmica do DOM: Criando elementos como tipos e estatísticas programaticamente.

Gestão de Estado: currentPokemonId evita conflitos durante navegação rápida.
