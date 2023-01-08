<center><b>Vídeo 02 Objetos internos do git</b></center> 

- Objetos fundamentais do git

  - Blobs

    - ```
      echo "conteudo" | git hash-object --stdin
      > fc31e91b26cf85a55e072476de7f263c89260eb1
      echo -e "conteudo" | openssl sha1
      (stdin)= 65b0d0dda479cc03cce59528e28961e498155f5c
      ```

    - O objeto blob possui meta-dados dentro dele

      - O tipo

      - O Tamanho

      - \0

      - Conteúdo do arquivo

      - ```
        echo -e 'blob 9\0conteudo' | openssl sha1
        > (stdin)= fc31e91b26cf85a55e072476de7f263c89260eb1
        ```

  - Trees

    - As trees armazenam os blobs
    - Ele pode possui vários blobs
    - Ela também possui meta-dados
      - O tipo
      - O tamanho
      - \0
      - blob
      - hash do blob 
      - o arquivo do blob
    - As trees podem apontar para outras arvores

  - Commits

    - O commit ele agrega tudo e estrutura para a gente ele pode apontar para outras árvores para o commit parente (realizado antes dele), armazena o nome do autor uma mensagem e a data de quando foi feito.
    - Os commit também possui uma hash tbm gerada a partir daquele commit

- Sistema distribuído seguro

  - Ele é seguro pois está na nuvem e nas maquinas de cada um.
