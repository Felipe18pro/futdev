# FutDev
Nosso codigo JavaScript implementa um sistema de gerenciamento de jogadores de futebol através de um terminal interativo.

## Funções
- exibir menu
```Javascript
function exibirMenu() {

    console.log(`

    Menu:

        1. Inserir Jogador

        2. Alterar Jogadores

        3. Excluir Jogador  

        4. Listar Jogadores

        5. Resultados do Jogador

        6. Sair

    `)

    rl.question('Escolha uma opção: ', (opcao) => {

        switch (opcao) {

            case '1':

                inserirJogadores()

                break

            case '2':

                alterarJogador()

                break

            case '3':

                excluirJogador()
                break
            case '4':
                listarJogadores()
                break
            case '5':
                resultadosDoJogador()
                break
            case '6':
                console.log('Sair')
                rl.close()
                break
            default:
                console.log('Opção inválida, tente novamente.')
                exibirMenu()
                break
        }
    })
}
```
