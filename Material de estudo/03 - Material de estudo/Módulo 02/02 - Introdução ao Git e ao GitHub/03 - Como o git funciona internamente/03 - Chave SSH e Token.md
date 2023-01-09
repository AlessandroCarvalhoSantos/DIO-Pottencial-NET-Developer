<center><b>Vídeo 03 Chave SSH e Token</b></center> 

- Chaves SSH

  - Estabelece uma chave segura do nosso computador no git hub

  - Primeiro passo é gerar uma chave no computador

  - ```
    ssh-keygen -t ed25519 -C email_do_git
    ```

  - Depois ele pergunta o local que as chaves serão geradas

  - Depois entre com uma senha

  - depois use o comando cat + nomeChavePublica e a adicione no github

  - ```
    cat id_ed25519.pub
    ```

    Adicione no GitHub em chaves sshKey copiando o resultaod do comando a cima

  - Depois é necessário inicializar a chave no PID

  - ```
    eval $(ssh-agent -s)
    ```

  - Agora mostre a chave privada para ele

  - ```
    ssh-add id_ed25519
    ```

  - No primeiro uso ele pode pedir um confirmação só dar yes 

  - O processo no linux é igual

- Tokens de acesso pessoal

  - Criado o token que serve como senha, criado no git hub e use o método https. Usado para acessar quando for usar uma vez em algum computador diferente. O token é visto uma vez no github. Então salve seu token.