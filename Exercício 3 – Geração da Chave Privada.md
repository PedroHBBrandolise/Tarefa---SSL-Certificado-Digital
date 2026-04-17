![Print](Prints%20dos%20Exercícios/Exercicio3.png)

O comando openssl genrsa -out aluno.key 2048 foi utilizado para criar a nossa Chave Privada.

O que é a Chave Privada?

Na criptografia assimétrica, trabalhamos com um par de chaves: uma Pública (que é distribuída livremente) e uma Privada. A chave privada é o "segredo" do servidor. Ela é usada para descriptografar os dados que foram criptografados com a chave pública e também para assinar digitalmente documentos e certificados, garantindo a identidade de quem os envia. Ela nunca deve ser compartilhada com ninguém.

Entendendo o comando:

genrsa: Indica ao OpenSSL para gerar uma chave usando o algoritmo RSA (um dos padrões mais seguros e comuns).

-out aluno.key: Especifica o nome do arquivo de saída onde a chave será salva.

2048: Define o tamanho da chave em bits. Uma chave de 2048 bits é o padrão atual recomendado para equilibrar alta segurança com boa performance no processamento.
