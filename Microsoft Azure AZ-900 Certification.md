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

   

6. **Benefícios da Nuvem Azure**

   1. *Alta disponibilidade*:  A alta disponibilidade se concentra em garantir a disponibilidade máxima, independentemente de interrupções ou eventos que possam ocorrer.

      - Ao arquitetar sua solução, você precisará considerar as garantias de disponibilidade do serviço. O Azure é um ambiente de nuvem altamente disponível com garantias de tempo de atividade, dependendo do serviço. Essas garantias fazem parte dos **SLAs (Contratos de Nível de Serviço - Azure Service Level Agreements)**.

      - Os **SLAs** diz respeito à qualidade das entregas, sempre levando em consideração os objetivos e metas estipuladas. O **SLAs** do Azure são representados como um percentual relacionado à disponibilidade do serviço ou do aplicativo. Essa disponibilidade também é conhecida como "tempo de atividade" (**Up Time**). Uma **SLAs** também geralmente inclui detalhes de como o que é definido como "tempo de inatividade" (**Downtime**), quando o serviço está indisponível e qualquer crédito a que você possa ter direito se o **SLA** não for cumprido.

      - **SLAs** de 99%, 99,9% e 99,95% são mais comuns.

      - **Cada serviço do Azure tem seu próprio SLA**.

        

   2. *Escalabilidade*: A escalabilidade refere-se à capacidade de ajustar recursos para atender à demanda.

      - A capacidade de escalar significa que você poderá adicionar mais recursos para lidar melhor com o aumento da demanda

      - O outro benefício da escalabilidade é que você não está pagando além do necessário pelos serviços. Como a nuvem é um modelo baseado em consumo, você paga apenas pelo que usa. Se a demanda cair, você poderá reduzir seus recursos e, assim, reduzir seus custos.

      - **A escala geralmente vem em duas variedades: vertical e horizontal**

      - **Dimensionamento vertical:** Com a escala vertical, se você estivesse desenvolvendo um aplicativo e precisasse de mais capacidade de processamento, poderia escalar verticalmente para adicionar mais CPUs ou RAM à máquina virtual. Por outro lado, se você percebesse que superestimou as necessidades, poderia reduzir verticalmente, diminuindo as especificações de CPU ou RAM.
   
      - **Dimensionamento Horizontal (Elasticidade):** Com a escala horizontal, se você experimentasse um salto repentino acentuado na demanda, seus recursos implantados poderiam ser expandidos (automaticamente ou manualmente). Por exemplo, você pode adicionar máquinas virtuais ou contêineres por meio da expansão. Da mesma forma, se houver uma queda significativa na demanda, os recursos implantados poderão ser reduzidos horizontalmente (de maneira automática ou manual).
   
        
   
   3. *Confiabilidade*: Resiliência é a capacidade que um sistema tem de se recuperar de falhas e continuar funcionando. Ela também é um dos pilares do [**Microsoft Azure Well-Architected Framework**]([How to use the Azure Well-Architected Framework documentation - Microsoft Azure Well-Architected Framework | Microsoft Learn](https://learn.microsoft.com/en-us/azure/well-architected/what-is-well-architected-framework)).
   
      - Devido ao design descentralizado, a nuvem naturalmente dá suporte a uma infraestrutura confiável e resiliente.
      - Com um design descentralizado, a nuvem permite que você tenha recursos implantados em várias regiões do mundo.
      - Com essa escala global, mesmo que ocorra um evento catastrófico em uma região, as outras regiões ainda estarão em funcionamento. 
      -  Você pode criar aplicativos para aproveitar automaticamente essa confiabilidade maior. Em alguns casos, o próprio ambiente de nuvem mudará automaticamente para uma região diferente, sem que você precise realizar nenhuma ação.
   
   4. *Previsibilidade*: A previsibilidade na nuvem permite que você avance com confiança. A previsibilidade pode se concentrar na previsibilidade de desempenho ou na previsibilidade de custo. Tanto a previsibilidade de desempenho quanto a de custo são bastante influenciadas pelo [**Microsoft Azure Well-Architected Framework**]([How to use the Azure Well-Architected Framework documentation - Microsoft Azure Well-Architected Framework | Microsoft Learn](https://learn.microsoft.com/en-us/azure/well-architected/what-is-well-architected-framework)).
   
      - **Desempenho**: A previsibilidade de desempenho se concentra em prever os recursos necessários para oferecer uma experiência positiva aos clientes. O dimensionamento automático, o balanceamento de carga e a alta disponibilidade são apenas alguns dos conceitos de nuvem que dão suporte à previsibilidade de desempenho. 
      - **Custo**: A previsibilidade de custos se concentra em prever o custo dos gastos com a nuvem.  Com a nuvem, você pode acompanhar o uso de recursos em tempo real, monitorar os recursos para garantir a maior eficiência de uso possível e aplicar a análise de dados para encontrar padrões e tendências que ajudam a planejar melhor as implantações de recursos. Operando na nuvem e usando a análise e as informações da nuvem, você pode prever custos futuros e ajustar os recursos conforme o necessário.
   
   5. *Segurança*: A nuvem oferece ferramentas de segurança que atendem às necessidades dos clientes mas, é importante lembrar que a implementação de muitas delas devem ser realizadas pelo cliente.
   
      -  **Se você quiser o controle máximo da segurança**, a **infraestrutura como serviço** (**IaaS**) fornecerá recursos físicos, mas permitirá que você gerencie os sistemas operacionais e o software instalado, incluindo aplicação de patches e manutenção.
      - **Se você quiser que a aplicação de patches e a manutenção sejam tratadas automaticamente**, as implantações de **plataforma como serviço ou software como serviço** (**PaaS** e **SaaS**) podem ser as melhores estratégias de nuvem para você.
   
   6. *Governança*: A auditoria baseada em nuvem ajuda a sinalizar qualquer recurso que esteja fora de conformidade com seus padrões corporativos e fornece estratégias de mitigação.
   
      - Dependendo do seu modelo operacional, patches de software e atualizações também podem ser aplicados automaticamente, o que ajuda na governança e na segurança.
      - Ao estabelecer uma presença de governança o mais cedo possível, você poderá manter sua presença de nuvem atualizada, protegida e bem gerenciada.
   
   7. *Gerenciabilidade*: Um dos principais benefícios da computação em nuvem são as opções de capacidade de gerenciamento. Há dois tipos de capacidade de gerenciamento para computação em nuvem que você aprenderá nesta série e ambos trazem excelentes benefícios.
   
      - **Gerenciamento da Nuvem:** O gerenciamento da nuvem diz respeito a gerenciar seus recursos de nuvem. Na nuvem, você pode:
        - Escalar automaticamente a implantação de recursos com base na necessidade.
        - Implantar recursos com ase em um modelo pré-configurado, removendo a necessidade de configuração a necessidade de configuração manual.
        - Monitorar a integridade dos recursos e substituir automaticamente os recursos com falha.
        - Receber alertas automáticos com base em métricas configuradas, de modo a ficar ciente do desempenho em tempo real.
      - **Gerenciamento na Nuvem:**  O gerenciamento na nuvem diz respeito à maneira de gerenciar seu ambiente de nuvem e seus recursos. Você pode gerenciá-los:
        - Por meio de um portal da Web.
        - Usando uma interface de linha de comando.
        - Usando APIs.
        - Usando o PowerShell.
