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
<br> Caso uma pagina de ajuda se abra significa que a instalação ocorreu corretamente, mas ainda não acabou, porque ainda precisamos instalar o minikube para isso podemos utilizar um metodo parecido com a instalação do nosso kubectl, segue abaixo o comando que utilizaremos

        sudo curl -Lo minikube https://github.com/kubernetes/minikube/releases/download/v0.28.0/minikube-linux-amd64

<br> A partir de agora podemos assim como fizemos com o kubectl, ceder permissão ao nosso arquivo e move-lo para nosso diretorio incluso no PATH, dessa forma poderemos digitar seu comando de qualquer lugar que estivermos dentro da nossa VM 


        sudo chmod +x minikube
        sudo mv minikube /usr/local/bin/
<br> Podemos então conferir se instalação deu certo usando

        minukube --help
        
