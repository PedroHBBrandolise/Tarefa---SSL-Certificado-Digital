# Tarefa---SSL-Certificado-Digital
Segurança de Sistemas Computacionais

## ENTREGA FINAL

* **Nome:** Pedro Henrique Bufon Brandolise
* **Ambiente:** Kali Linux (versão 2026.1 amd64) executado em máquina virtual Oracle VirtualBox.
* **IP:** 127.0.0.1 (Localhost) - *Utilizado para a simulação de tráfego de rede e conexão SSH/Web na mesma máquina.*

**Dificuldades:**
As principais dificuldades encontradas envolveram o gerenciamento de permissões e a simulação de rede em um ambiente de máquina única:
1. Compreender a necessidade de privilégios de administrador (`sudo`) para criar e manipular diretórios restritos do sistema (como o `/etc/ssl/certificates/`).
2. Contornar a ausência de uma máquina remota para o teste do protocolo SCP, o que foi solucionado ativando o serviço SSH local e utilizando o endereço de *loopback* (localhost) para validar a transferência segura.
3. Entender a hierarquia de certificados do navegador para importar o arquivo `.crt` corretamente, diferenciando um certificado de Entidade Final (o meu) de uma Autoridade Certificadora Root.

**Conclusão:**
O laboratório proporcionou uma visão prática essencial sobre segurança digital, criptografia e infraestrutura de chaves públicas. Foi possível acompanhar de ponta a ponta o ciclo de vida de um certificado digital: gerando a chave privada (RSA), criando a requisição (CSR), emitindo um certificado autoassinado (X.509) e transferindo os arquivos de forma segura via SSH/SCP. Além disso, a simulação de erro de protocolo (HTTP vs HTTPS) demonstrou na prática como aplicações web e navegadores lidam com conexões seguras no nível da rede, consolidando conceitos que são fundamentais para o desenvolvimento de infraestruturas computacionais seguras.
