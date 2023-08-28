GraphQL - Curso FullCycle

BUG - CORRIGIDO:

Olá Pessoal.

Tudo bem com vocês?

Realmente havia um pequeno erro, pois na criação das Models de (course / category) a propriedade Description apontava para um ponteiro do tipo string, mas ao definirmos a nossa struct em /internal/database/course.go e category.go não havíamos incluído o apontamento ao ponteiro, desta forma quando utilizamos a variável description ela está lendo o valor de description através do ponteiro.

Para melhor compreensão:

&: É o endereço do ponteiro

*: É o apontamento do qual o ponteiro está referenciado através do nome da variável

Abaixo segue o repositório atualizado com está correção, acessem o último commit para um melhor entendimento do que foi corrigido.

Link: https://github.com/devfullcycle/13-GraphQL

Qualquer dúvida estamos à disposição.

Obrigado.

Abraços.