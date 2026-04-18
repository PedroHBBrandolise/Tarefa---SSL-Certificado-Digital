![Print](Prints%20dos%20Exercícios/Exercicio8.png)

A etapa final consistiu na validação do ficheiro aluno.crt através do visualizador de certificados do sistema, confirmando que a estrutura X.509 foi gerada corretamente.

O que foi validado:

Integridade dos Metadados: Verificou-se que todos os campos inseridos na etapa do CSR (País: BR, Estado: Sao Paulo, Localidade: Tiete, Organização: EEP) foram corretamente incorporados no certificado final.

Emissor e Titular: Como se trata de um certificado autoassinado (self-signed), os campos "Subject Name" (Titular) e "Issuer Name" (Emissor) apresentam as mesmas informações, demonstrando que a chave privada local foi utilizada para validar a própria identidade.

Validade: Confirmou-se o período de validade de um ano (365 dias), conforme definido no comando de geração do certificado.

Esta inspeção visual garante que o certificado está pronto para ser utilizado em serviços que exijam autenticação e criptografia, como servidores web HTTPS ou autenticação de rede.
