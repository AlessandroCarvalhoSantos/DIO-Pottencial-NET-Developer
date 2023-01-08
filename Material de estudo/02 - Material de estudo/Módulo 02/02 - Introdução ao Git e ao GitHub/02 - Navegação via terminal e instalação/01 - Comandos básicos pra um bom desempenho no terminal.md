<center><b>Vídeo 01 de Comandos básicos pra um bom desempenho no terminal</b></center> 

- **GUI e CLI**

  - GUI
    - Graphic user interface
  - CLI
    - Comand line interface

- Algumas diferenças 

  |   Windows   |  Unix  |
  | :---------: | :----: |
  |     cd      |   cd   |
  |     dir     |   ls   |
  |    mkdir    | mkdir  |
  | del / rmdir | rm -rf |

- OBS: alguns desses comando possuem frag que auxiliam na execução do comando.

-  Lista todos arquivos e pastas do caminho atual

  - Windows: dir 
  - Linux: ls

- Comando de navegação (Igual para Windows e linux)
  - cd pasta -> Abre a pasta atual
  - cd / -> Abre a pasta/caminho raiz
  - cd caminho -> Abre o caminho especificado
  - cd .. ->Volta uma pasta
  - cd ../../ -> Volta duas pastas
  - cd ./ -> Abre a pasta atual

- Limpeza de tela

  -  Windows:
    - cls
  - Linux
    - clear
    - O comando ctrl+l limpa a tela também

- Auto-complete de comandos e pasta

  - Utilizamos TAB no Windows e Linux   

- Entrar como Admin no Linux

  - sudo su   depois digite a senha root

- Criação de pastas (igual para Windows e linux)

  - mkdir nome_pasta

- Comando echo (Igual par Windows e linux)

  - echo texto  ->Escreve um texto no terminal

- Criando um arquivo com texto

  echo texto > arquivo.extensao       

  - Escreve o texto em um arquivo txt e se não existir ele cria.     

- Comando de deletar

  - Windows

    del pasta/arquivo  (Deletar um arquivo ou os arquivos dentro de uma pasta)

  ​       rmdir pasta (Deleta uma pasta ou diretório se tiver vazia)

  ​       rmdir pasta /s /q (Deleta tudo dentro da pasta e pasta subsequentes)

  ​			/s -> Exclui uma árvore de diretório (o diretório especificado e todos os seus subdiretórios, incluindo todos 					os arquivos).

  ​			/q -> Especifica o modo silencioso. Não solicita confirmação ao excluir uma árvore de diretório. O parâmetro 					/q só funcionará se /s também for especificado.

  - Linux

    ​	rm arquivo  (deleta um arquivo)

  ​           rm -rf (Remove a pasta e todos os seus arquivos e pasta subsequentes)

  ​           -r (remove todas as pastas e arquivos)

  ​           -f (Força fazer algo sem pedir confirmação)

  ​					Podemos unir Flags no Linux da seguinte forma

  ​                                        -r -f ou -rf 

- Dica: se o terminal não retornou nada, é porque deve que ocorreu tudo certo no comando