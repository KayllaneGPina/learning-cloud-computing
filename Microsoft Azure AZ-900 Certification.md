# Microsoft Azure AZ-900 Certification

 

## Computação em Nuvem

1. **O que é computação em nuvem**

   A computação em nuvem é o fornecimento de serviços de computação pela Internet, habilitando inovações mais rápidas, recursos flexíveis e economias de escala.

   

2. **Responsabilidade compartilhada**

   Comece com um datacenter corporativo tradicional. A empresa é responsável por manter o espaço físico, garantir a segurança e manter ou substituir os servidores se algo acontecer. O departamento de TI é responsável por manter toda a infraestrutura e o software necessários para manter o datacenter em funcionamento. É provável que eles também sejam responsáveis por manter todos os sistemas corrigidos e na versão correta.

   Com o modelo de responsabilidade compartilhada, essas responsabilidades são compartilhadas entre o provedor de nuvem e o consumidor. Segurança física, energia, resfriamento e conectividade de rede são responsabilidade do provedor de nuvem. O consumidor não fica na mesma localização do datacenter, portanto, não faria sentido que o consumidor tivesse algumas dessas responsabilidades.

   Ao mesmo tempo, o consumidor é responsável pelos dados e pelas informações armazenados na nuvem. (Você não gostaria que o provedor de nuvem pudesse ler suas informações). O consumidor também é responsável pela segurança de acesso, o que significa que você só dá acesso àqueles que precisam.

   

   O modelo de responsabilidade compartilhada está fortemente vinculado aos tipos de serviço de nuvem (abordados posteriormente neste roteiro de aprendizagem): **IaaS (infraestrutura como serviço), PaaS (plataforma como serviço) e SaaS (software como serviço).** **A IaaS coloca a maior responsabilidade sobre o consumidor**, com o provedor de nuvem sendo responsável pelas questões básicas de segurança física, energia e conectividade. Na outra ponta do espectro, o SaaS coloca a maior parte da responsabilidade no provedor de nuvem. A PaaS, sendo um meio termo entre IaaS e SaaS, situa-se no meio desses dois cenários e distribui uniformemente a responsabilidade entre o provedor de nuvem e o consumidor.

   

   ![ModeloResposabilidadeCompartilhada](https://learn.microsoft.com/pt-br/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg)

   

3. **Modelos de nuvem**

   1. *Nuvem privada:*

      - As organizações criam um ambiente em nuvem em seu datacenter.
      - As organizações são responsáveis por operar os serviços que fornecem.
      - Não fornece acesso aos usuários fora da organização;

   2. *Nuvem pública:*

      - Pertencente a serviços de nuvem ou provedor de hosting.
      - Fornece recursos e serviços a várias organizações e usuários.
      - Acessada via conexão de rede segura (geralmente pela internet).

   3. *Nuvem híbrida:*

      - Combina nuvens públicas e privadas para permitir que os aplicativos sejam executados no local mais adequado.

   4. *Nuvem multicloud:*

      -  Multicloud é uma combinação da utilização de diferentes nuvens (públicas, privadas e híbridas), utilizando vários provedores de Cloud, como Google Cloud Plataform, Huawei Cloud, Amazon Web Services entre outros.

      

4. **Comparação de modelos de nuvem**

   1. *Nuvem pública:* 
      - Nenhuma despesa de capital para escalar verticalmente.
      - Os aplicativos podem ser provisionados e desprovisionados rapidamente.
      - As organizações pagam apenas pelo que utilizam (Pay as you go)
   2. *Nuvem privada:*
      - As organizações têm controle total sobre os recusos e a segurança.
      - As organizações são responsáveis pela manutenção e pelas atualizações de hardware e software.
   3. *Nuvem híbrida:*
      - As organizações determinam onde executar seus aplicativos.
      - As organizações controlam a segurança, a conformidade e os requisistos legais.
      - Fornece a maior flexibilidade.

   

5. **Custo de capital versus custo operacional (FinOps)**

   1. *Despesas de capital (CapEx):*
      - O gasto inicial de dinheiro em infraestrutura física.
      - As despesas do CapEx têm um valor que se reduz com o tempo.
   2. *Despesas operacionais (OpEx):*
      - Gastar com produtos e serviços conforme necessário, pagamento conforme o uso.
      - Seja cobrado imediatamente.
   3. Modelo baseado em consumo:
      - Os provedores de serviços em nuvem operam em um modelo baseado no consumo, o que significa que os usuários finais pagam somente pelos recursos que usam.
      - Melhor previsão de custos.
      - São fornecidos preços para recursos e serviçoes individuais.
      - A  cobrança é feita com base no seu uso real.
      
      
   
   **A computação em nuvem se enquadra na OpEx porque opera em um modelo baseado em consumo.** Na computação em nuvem, você não paga pela infraestrutura física, pela eletricidade, pela segurança nem por nada que esteja associado à manutenção de um datacenter. Você paga pelos recursos de TI que usa. Se você não usar nenhum recurso de TI durante o mês, não pagará nada.
