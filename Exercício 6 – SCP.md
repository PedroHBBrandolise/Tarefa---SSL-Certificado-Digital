![Print](Prints%20dos%20Exercícios/Exercicio6.png)

O comando scp foi utilizado para demonstrar a transferência segura de arquivos através de uma conexão SSH.

Adaptação do Laboratório: Como este ambiente foi construído com apenas uma máquina virtual, a transferência foi simulada utilizando o endereço de loopback (localhost ou 127.0.0.1). Isso obriga o sistema a empacotar o arquivo (aluno.crt) e enviá-lo através dos protocolos de rede reais, criptografados pelo SSH, enviando-o da pasta de sistema para o diretório local do usuário.

Este método comprova o funcionamento da ferramenta de cópia segura (scp), garantindo que a conexão não possa ser interceptada em texto claro por terceiros caso fosse uma rede externa real.
