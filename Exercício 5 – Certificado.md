![Print](Prints%20dos%20Exercícios/Exercicio5.png)

O comando sudo openssl x509 -req -days 365 -in aluno.csr -signkey aluno.key -out aluno.crt foi utilizado para gerar e assinar o Certificado Digital final.

O que aconteceu aqui?

Em um ambiente de produção real, enviaríamos o arquivo .csr (gerado no exercício anterior) para uma Autoridade Certificadora (CA) verdadeira (como Verisign, Let's Encrypt, etc.). A CA usaria a chave privada deles para assinar o certificado, garantindo para o mundo que somos quem dizemos ser.

Como estamos em um ambiente de laboratório/teste, criamos um Certificado Autoassinado (Self-Signed Certificate). Isso significa que usamos a nossa própria chave privada (aluno.key) para assinar o nosso próprio pedido de certificado (aluno.csr).
