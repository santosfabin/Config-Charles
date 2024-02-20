# Configurando o Charles

- Show memory usage
    - Como o Charles foi feito em Java, ele usa um limite de memória. Vamos verificar quanto de memória ele está usando, pois caso esteja com um limite baixo, precisaremos aumentá-lo.
    - Vá em "Edit" no canto superior esquerdo e depois em "Preferences...".
    - Habilite a última opção e em seguida clique em “OK”.
        
        ![Untitled](Configurando%20o%20Charles/Untitled.png)
        
- Aumento de memória
    - Para aumentar a exibição de MB baixados no canto inferior direito, iremos fazer os ajustes necessários.
    - Em seu terminal digite:
        
        ```bash
        whereis charles
        ```
        
    - Ele mostrará um caminho até o arquivo.
    - Então vamos alterar um valor para que ele utilize mais memória.
    - Com qualquer editor, edite esta linha para um valor que você deseje de memória.
        
        ![Untitled](Configurando%20o%20Charles/Untitled%201.png)
        
- Proxy no navegador
    - Em "Proxy" no canto superior esquerdo, vá até a opção "Proxy Settings...".
    - Vejo o IP que tem.
        
        ![Untitled](Configurando%20o%20Charles/Untitled%202.png)
        
    - Agora vamos até nosso navegador e acessar nossa extensão que manipula qual proxy usar.
    - No meu caso estou usando o “**FoxyProxy**”.
    - Indo em “Options”.
        
        ![Untitled](Configurando%20o%20Charles/Untitled%203.png)
        
    - Adicione uma proxy em “Add”.
    - Preencha de acordo com a porta que está no Charles.
    - Então clique em "Save".
        
        ![Untitled](Configurando%20o%20Charles/Untitled%204.png)
        
    
- Adicionando certificado
    - Ao tentar usar o Charles, ele dá um erro de certificado.
    - Então vamos adicionar o certificado ao navegador.
    - “Help” → “SSL Proxying” → “Save Charles Root Certificate…”.
    - Salve onde preferir.
    - No navegador, vá em Configurações e digite na busca "Certificate" ou "Certificado".
    - Como estou no Firefox, irei em "View Certificates...".
        
        ![Untitled](Configurando%20o%20Charles/Untitled%205.png)
        
    - Em seguida em “Import…”.
        
        ![Untitled](Configurando%20o%20Charles/Untitled%206.png)
        
    - Agora basta colocar seu certificado.
