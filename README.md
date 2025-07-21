# Introdução AZ900 - Continuação

1. Benefícios da nuvem
2. Tipos de serviços de nuvem
3. Regiões
4. Pares de regiões
5. Recursos do Azure

## Benefícios da nuvem

### Alta disponibilidade
Concentra em garantir a disponibilidade máxima, independentemente de interrupões ou eventos que possam ocorrer.

### Escalabilidade
Permite que as empresas ajustem sua capacidade de computação conforme a necessidade, pagando apenas pelo que usa.

### Elasticidade
Permite que as empresas ajustem dinamicamente seus recursos de TI para atender às demandas. Essa capacidade de escalar para cima ou para baixo conforme a necessidade evita o desperdício de recursos e garante que a infraestrutura esteja sempre otimizada para o momento.

### Confiabilidade
Permite que as empresas tenham recursos implantados em várias regiões do mundo, oferecendo recursos como backup de dados, recuperação de desastres e continuidade dos negócios.

### Previsibilidade
Importante para a gestão de serviços em nuvem, pode ser alcançado através de rpéticas como FinOps. Permite que equipes diferentes trabalhem juntas para equilibrar desempenho, custo e qualidade.

### Segurança
Oferecem  várias ferramentas de segurança, mas vale lembrar que a implementação de muitas delas devem ser realizadas pelo cliente.

### Governança
Ajuda as empresas a equilibrar a inovação com o controle, garantindo que os recursos em nuvem sejam usados de forma eficiente e segura.

### Gerenciabilidade
Oferce maior controel sobre os recursos, otimização de custos, agilidade no desenvolvimento e implementação de aplicações, além de segurança aprimorada.

## Tipos de serviços de nuvem

### IaaS (Infraestrutura como serviço)
É um modelo de computação em nuvem onde os recursos computacionais como servidores, armazenamento e redes são disponibilizados sob demanda pela internet. As empresas podem utilizar esses recursos sem a necessidade de adquirir, gerenciar e manter sua própria infraestrutura física.

### PaaS (Plataforma como serviço)
É um modelo de computação em nuvem que oferece uma plataforma completa, incluindo hardware, software e infraestrutura, para o desenvolvimento, excecução e gerenciamento de aplicativos, permite que desenvolvedores se concentrem na criação de aplicativos, enquanto o provedor de nuvem cuida da infraestrutura subjacente.

### SaaS (Software como serviço)
E um modelo de computação em nuvem que oferece software através da internet. As empresas que oferecem SaaS cuidam da infraestrutura, manutenção e atualização, enquanto os clientes acessam o software através de um navegador ou aplicativo.

### Comparação dos serviços de nuvem (IaaS, PaaS e SaaS)
IaaS fornece infraestrutura virtualizada, PaaS oferece uma plataforma para desenvolvimento e SaaS entrega aplicativos prontos para uso.

## Regiões
São áreas geográficas onde os provedores de nuvem possuem data centers. Cada região é projetada para fornecer serviços de nuvem de forma redundante e confiável, com múltiplas zonas de disponibilidade.

### Zona de disponibilidade
São locais fisicamente separados dentro de uma região. Eles são projetados para oferecer alta disponibilidade, de forma que, se uma zona falhar, outras zonas na mesma região possam continuar operando normalmente.

## Pares de regiões
São pares predefinidos de regiões dentro de um provedor de nuvem que são projetaos para trabalhar em conjunto. O objetivo principal é fornecer redundância geográfica e recuperação de desastres.

## Recursos do Azure
São os blocos de construção fundamentais para a sua estrutura e aplicativos na nuvem. Eles incluem serviços de computação, armazenamento, rede, banco de dados, análise, interligência artificial, entre outros. Cada recuros é provisionado e gerenciado por meio do Azure Resource Manager, permitindo organização, implantação e gerenciamento eficientes.

### Assinatura do Azure
É como uma conta que organiza e gerencia todos os recursos de nuvem que você usa, como máquinas virtuais, banco de dados, etc. Ela também define como esses recursos são cobrados, gerlmente por departamento ou projeto.
* **Limite de cobrança**: gere relatórios de cobrança e faturas separados para cada assinatura.

* **Limite do controle de acesso**: gerenciar e controlar acesso aos recursos que os usuários podem provisionar com assinaturas específicas.

#### Múltiplas assinaturas
Uma organização pode ter várias assinaturas do Azure, por exemplo, uma para cada departamento, ou uma para desenvolvimento e outra para produção.

#### Conta individual
Um usuário também pode ter várias assinaturas, como uma assinatura do Visual Studio Enterprese com créditos mensais e outra assinatura paga conforme o usu.

### Grupos de gerenciamento
Fornecem um nível de escopo de governança acima das assinaturas. Quando você organiza assinaturas em grupos de gerenciamento, as condições de governança aplicadas são propagadas por herança a todas as assinaturas associadas.

*Isto é uma atividade de curso de AZ 900 da DIO*
