# ParserDSL

O projeto parserDSL foi desenvolvido na disciplina de Tópicos Avançados em Engenharia de Software, do curso de ciência da computação da Universidade Federal do Ceará

<b>OBJETIVO</b>

O parserDSL visa auxiliar os usuários a definir um analisador léxico de uma determinada linguagem de programação para ser gerado a partir de um arquivo .jj que pode ser interpretado pelo javaCC definindo apenas os tokens da linguagem.


<b>FUNCIONAMENTO</b>

Ao executar a DSL cria-se um arquivo .parserdsl e nele é apresentada uma interface em modelo de árvore, com um nó gramática. A partir deste nó é possível, ao clique do botão esquerdo, inserir tokens, que podem ser um símbolo Terminal(Palavra reservada) ou um Skip(strings a serem disconsideradas na leitura do código).

 Para cada um, terminal ou skip, é possível definir o nome do token e a sua descrição, esta última sempre entre aspas. Ao terminar de definir todos, basta clicar com botão esquerdo sobre o arquivo .parserdsl e, em acceleo model to text, selecionar Generate ParserDSL para gerar os arquivos parser.jj e mainClass.java.
 
 Tendo os dois arquivos no mesmo diretório, executa-se na linha de comando "javacc parser.jj" para gerar os arquivos necessários e em seguida se executa o arquivo mainClass.java que espera algum trecho de código para executar a análise léxica referente à linguagem definida.

<b>COMPLEMENTOS</b>

Para executar o compilador é necessário fazer download do JavaCC em https://javacc.org

