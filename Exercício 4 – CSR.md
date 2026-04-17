![Print](Prints%20dos%20Exercícios/Exercicio4.png)

O comando sudo openssl req -new -key aluno.key -out aluno.csr foi utilizado para gerar o CSR.

O que é o CSR?
CSR significa Certificate Signing Request (Requisição de Assinatura de Certificado). Ele é essencialmente um pacote de texto criptografado gerado no servidor onde o certificado será instalado.

Ele contém duas coisas fundamentais:

A Chave Pública que fará par com a chave privada (aluno.key) gerada no passo anterior.

As Informações de Identidade da organização/indivíduo (País, Estado, Organização, Domínio/Common Name).

O processo funciona como um "pedido de RG". Nós geramos o CSR e o enviamos para uma Autoridade Certificadora (CA). A CA verifica nossa identidade baseada nos dados do CSR e, se aprovado, usa a nossa chave pública contida nele para gerar e assinar o nosso Certificado Digital final (.crt).

Entendendo o comando:

req -new: Indica que queremos uma nova requisição de certificado.

-key aluno.key: Informa ao OpenSSL qual chave privada ele deve usar para vincular e assinar digitalmente este pedido.

-out aluno.csr: Define o nome do arquivo gerado.
