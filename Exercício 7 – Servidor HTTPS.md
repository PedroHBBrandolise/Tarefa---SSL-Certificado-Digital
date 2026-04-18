![Print](Prints%20dos%20Exercícios/Exercicio7.png)

O erro ocorreu por uma incompatibilidade de protocolos.

O comando utilizado no terminal iniciou um servidor web básico usando apenas HTTP (texto puro). No entanto, tentamos acessar a página via HTTPS (conexão segura e criptografada).

Como resultado, tivemos falhas nos dois lados:

No Servidor (Terminal): Ele não conseguiu ler os dados criptografados enviados pelo navegador e retornou um erro HTTP 400 (Bad Request).

No Navegador: Ele aguardava um certificado de segurança, mas recebeu a mensagem de erro em texto puro do servidor, abortando a conexão com o erro SSL_ERROR_RX_RECORD_TOO_LONG.
