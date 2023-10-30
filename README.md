# Semana-3
## Primeiro desafio: instalar minikube ou S3 para gerenciar.
<br> Vamos instalar primeiro o kubectl com o seguinte comando abaixo
    
    sudo curl -LO "https://dl.k8s.io/release/$(curl -L -s   https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

<br> Agora precisamos garantir que o arquivo tenha permissão para ser executado, podemos fazer isso utilizando o comando:

    sudo chmod +x kubectl
<br> É importante tambem mover nosso arquivo para um diretorio que esteja no PATH para que possamos digitar comandos dele sem necessariamente estar no diretorio do mesmo, para isso podemos utilizar 

    sudo mv kubectl /usr/local/bin/
<br> Tudo pronto, para verificar se tudo correu bem podemos digitar o comando abaixo para ver se tudo foi instalado corretamente

    kubectl --help
<br> Caso uma pagina de ajuda se abra significa que a instalação ocorreu corretamente
