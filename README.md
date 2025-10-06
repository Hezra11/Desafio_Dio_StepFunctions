# DESAFIO DIO ```AWS STEP FUNCTIONS```
Este desafio teve como objetivo desenvolver minhas habilidades na utilização do recurso AWS STEP FUNCTIONS, um serviço de fluxo de trabalho visual; desenvolvimento de aplicações; automação de processos e orquestração de microsserviços.

## Passo 1
Ao acessar o recurso, para minha primeira experiência com a ferramenta optei pelo modelo pré-definido: *“Processar um arquivo CSV do Amazon S3 usando um mapa distribuído”*. Este modelo pode iterar mais de 10 mil linhas de um arquivo CSV, usando uma função do Lambda. O arquivo CSV contém informações de envio dos pedidos do cliente e é armazenado em um bucket do Amazon S3. O Mapa distribuído itera em um lote de 10 linhas no arquivo CSV para análise de dados. A função do Lambda detecta qualquer pedido atrasado retornando esses pedidos atrasados em uma matriz. Para cada pedido atrasado o Mapa Inline envia uma mensagem para uma fila do Amazon SQS. 

## Passo 2 
Ao Criar a máquina de estado no console do Step Functions a partir da escolha do modelo segui na opção “executar uma demonstração” criando uma máquina de estado somente para leitura para, após a revisão criar o fluxo de trabalho e todos os recursos relacionados.

## Passo 3
No painel de templates é possível visualizar tanto o design quanto o código por trás do recurso, fácil para revisar, personalizar e implantar quaisquer recursos que desejar criar. Entendendo e confirmando os processos e as etapas do recurso, passei para a execução da máquina de estado.

## Passo 4
Na opção *“Implantar e Executar”* todos os recursos relacionados foram implantados em menos de 5 minutos pela AWS CloudFormation (algumas máquinas podem levar até 10 minutos para serem executadas).
Concluída a execução é possível visualizar todos os objetos do templates bem como a configuração de cada um deles. Na visualização do gráfico podemos verificar quais processos estão em andamento, com falhas ou finalizado com êxito.

# CONCLUSÃO
O orquestrador de serviços AWS Step Functions é um recurso de fácil execução, com um painel intuitivo, amigável, possibilitando trabalhar de forma simples, observando todas a etapas do processo, alterando, corrigindo ou implantando mais recursos.

# CÓDIGO DA MÁQUINA DE ESTADO CRIADA
<img width="886" height="753" alt="image" src="https://github.com/user-attachments/assets/b934462c-e0e3-498b-b997-40ab6c3812a5" />
<img width="886" height="740" alt="image" src="https://github.com/user-attachments/assets/7a1d2fa5-b041-4323-9f7c-2fcf6e18e55a" />
<img width="886" height="744" alt="image" src="https://github.com/user-attachments/assets/8a850ee3-50d2-4f58-8d2c-f6eff0acb0d7" />
<img width="881" height="221" alt="image" src="https://github.com/user-attachments/assets/e23e604b-476e-4821-9580-a7d3b934a5c2" />






