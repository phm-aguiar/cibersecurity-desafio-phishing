# Phishing para capturar senha de uma pagina da internet
Usaremos o site do ``` Facebook ``` como exemplo. 

### Ferramentas utilizadas:

- Kali Linux (https://www.kali.org/)
- Setoolkit (Ferramenta pré-instalada no Kali Linux)

### Pontos Importantes:
 - Caso esteja usando uma VM, certifique-se que a configuração da rede esteja no modo: Bridged Adapter(Inglês) ou Placa de modo Bridge(Português).
 - Funcionará para os dispositivos na mesma rede.
 - Ao clonar a pagina deve ser clonado a pagina onde digita o login e senha.

### Resumo (Passo-a-passo): Configuração da ferramenta setoolkit para construção do Phishing no Kali Linux:

 - Acesso root: sudo su
 - Iniciando o setoolkit: setoolkit
 - Tipo de ataque: Social-Engineering Attacks
 - Vetor de ataque: Web Site Attack Vectors
 - Método de ataque: Credential Harvester Attack Method 
 - Método de ataque: Site Cloner
 - Obtendo o endereço da máquina: ifconfig
 - URL para clone: http://www.facebook.com
 - Enviar o IP da maquina para alguém

### Detalhamento (Passo-a-passo): Configuração da ferramenta setoolkit para construção do Phishing no Kali Linux:

01 - Acesso root no modo administrador: aplicar o comando ``` sudo su ```, em seguida vai pedir para digitar a senha do administrador.

![image](https://github.com/user-attachments/assets/eabaade4-3d43-425a-bea8-6172b8bc7688)

02 - Em seguida, iniciar a ferramenta ``` setoolkit ``` com o comando: setoolkit. Ao acessar pela primeira vez, vai solicitar para aceitar os termos da ferremanta. Então, digite YES.

![image](https://github.com/user-attachments/assets/4caa7c67-207d-4e9a-b8c1-4b0b490841c4)

03 - Vai abrir a ferramenta com as opção, portanto, selecione a opção: ``` 01) Social-Engineering Attacks ```. 

![image](https://github.com/user-attachments/assets/382ca0bb-b191-4661-9f62-1b4cc21e1367)

04 - Seguindo com as configurações, selecione: ``` 2) Web Site Attack Vectors ```.

![image](https://github.com/user-attachments/assets/6894a2e5-94c9-41c5-99a3-f894f51a3827)

05 - Agora, selecione a opção: ```3) Credential Harvester Attack Method ```.

![image](https://github.com/user-attachments/assets/b2cfab7f-9671-4ab0-a752-18da8e9e843e)

06 - Mais uma configuração, selecionar a opção: ``` 2) Site Cloner ```.

![image](https://github.com/user-attachments/assets/49fd500e-c21f-431b-bc30-69a8ca044a16)

07 - Para seguir com a configuração, neste passo, a ferramenta identifica o IP que está rodando. O ``` Setoolkit ```, vai usar essa maquina como um servidor receber o login e senha rackeada. Então, mantém como está é apenas clicar no botão ``` Entrer ```. Você vão perceber que vai apresentar o o IP da maquina na tela.

![image](https://github.com/user-attachments/assets/0fe7af53-6ee9-4f50-bb81-08d9988c3894)

08 - Nesta opção, digitar a URL que irá clonar, no nosso exemplo é o: ``` http://www.facebook.com ```.

![image](https://github.com/user-attachments/assets/ae36dc56-d1b5-449b-b386-312bc1042054)

09 - Após clicar no entrer, a configuração está pronta e aguardando alguém clicar e tentar logar no Facebook. Na tela, fica desta forma, aguardando.

![image](https://github.com/user-attachments/assets/bde4993f-7fe6-4333-bc1d-fb0ee8e40af0)

10 - Enviar para alguém o IP que aparece no setimo passo, que é o IP da maquina.

### Resultados
Após alguém realizar o login e senha, a tela de comando apresentará alguns textos. Mas em alguma linha dessas vai mostrar conforme a imagem abaixo, com a captura.

![image](https://github.com/user-attachments/assets/eb9ea83b-5a06-4103-8ddc-50138b0e6978)

