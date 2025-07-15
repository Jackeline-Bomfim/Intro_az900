# Criando uma instância gerenciada de SQL do Azure.

Breve introdução
1. Criar uma instância gerenciada de SQL do Azure.
2. Criando banco de dados
3. Recuperando detalhes da conexão


## Criar uma instância gerenciada de SQL do Azure

Você pode efetuar esse processo através do Portal do Azure, PowerShell ou outras ferramentas utilizando a API REST, mas por aqui vamos seguir o passo a passo utilizando o Portal do Azure.

### Vamos lá!

* Acesse o [Portal do Azure](https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize?redirect_uri=https%3A%2F%2Fportal.azure.com%2Fsignin%2Findex%2F&response_type=code%20id_token&scope=https%3A%2F%2Fmanagement.core.windows.net%2F%2Fuser_impersonation%20openid%20email%20profile&state=OpenIdConnect.AuthenticationProperties%3DZ-9LObFS53mQoDQsWrZV1mVWH3PRBgfND9wtXUPd0f07jjvDIBIaco3FfQW03xTjDKgalKHmvYB_XW7qNn7MDbRnfJYPX7f4H22Ch7NADUFLw_myJmPf2oSocZKC8mdBbHDKQ5p1qFrK2GehmG2i_ial55jQy10T-SoOTUjWR8ppg8sjImmXa1_CMlSzyEU27FjR88ZyFQIkucqXUFFPaE7yhZESgAEQDM6mZzRkyal8p0wifJ9uRo5SN4_TxQN4HC4Rs8Jog67xtmzRJDLHoy6z4BXbIRj89QCt7e2M1o3CQwlR54KaBHcRIzEAHwBeku9Zv4n0GL2VLvt1z1SlQKlJSj4aPC7errCj6fjjn_vIy66DEGv_yTKZYXWjbhhxhvaz9Q4zl_qDVqXGGQ2bQrLBzcIOfy-9U9Jln_ZxWACbUqtEsp7vP0lV2XW_PjXuncc-3TCdc0e3ziHXLRDr2XUNNgAbgOy0Irfv9o6dzqw&response_mode=form_post&nonce=638879419121010114.OTAyNGQ2MTctNDMyZi00NjNmLTg3MmYtOTNmOTMyNDZhNmM5MjIxZDNkZDktYzllMy00Mzg4LTliZDktMmM4NDAxZWNiYmUy&client_id=c44b4083-3bb0-49c1-b47d-974e53cbdf3c&site_id=501430&instance_aware=true&client-request-id=9f7c8314-ff6c-4f4f-8830-1edf07475201&x-client-SKU=ID_NET472&x-client-ver=8.3.0.0).
* Selecione o **SQL do Azure**
* Clique em **Criar**
* Na tela de implantação do SQL, clique em **mostrar detalhes** 
* Escolha **Instância única** e selecione **Criar** 
Seguindo esses passos irá abrir a página para **criar instância gerenciada de SQL do Azure**.

![Instância](/img/instância.png)

Preencha as informações obrigatórias conforme a tabela abaixo:

![Tabela1](/img/Tabela%201.png)

Na parte de detalhes da instância gerenciada, selecione **Configurar Instância** gerenciada para abrir a página **Computação** + **Armazenamento**.

![Armazenamento](/img/armazenamento.png)

Abaixo segue a tabela de recomentações para a computação e o armazenamento para sua instância gerenciada SQL.

![tabela2](/img/Tabela%202.png)

Depois de efetuar as suas configurações clique em **Aplicar**, depois clique em **Próximo**.

#### Guia Rede

Preencha as informações de rede, isso é opional e caso não preenchido o portal aplicará as configurações padrão.

![Tabela3](/img/Tabela%203.png)

As informações de seguração deixe nos valores padrão.

A seguir temos as configurações adicionais, que também é opcional o seu preenchimento e caso não efetuado o portão aplicará as configurações padrão. Abaixo temos a tabela que oferece alguns detalhes sobre as informações que possa ajudar no preenchimento se obtado.

![tabela4](/img/tabela%204.png)

É recomendado configurar as marcas, então clique em **Avançar** e adicione marcas aos recursos, depois selecione **Examinar** + **criar**.

**Dica**: No ícone de notificações você consegue acompanhar o status da implantação.

## Criando o banco de dados

Ele também pode ser criado através de outras ferramentas mas iremos seguir explicando com o portal do azure.

* Acesse a instância
* Na página de visão geral, escolha **Novo banco de dados**.

![banco de dados](/img/banco%20de%20dados.png)
* Dê um nome ao banco de dados acessando a guia **Básico**
* Selecione **Nenhuma** para um banco de dados vazio ou restaure um banco de dados a partir do backup na guia **Fonte de dados**.
* Defina as demais configurações e selecione **Revisar** + **Criar**.
* Use **Criar** para implantar seu banco de dados.

## Recuperando detalhes da conexão

* Volte ao grupo de recursos e escolha o objeto de instância gerenciada de SQL que foi criado.
* Na guia **Visão Geral**, localize a propriedade Host. Copie o nome do host para sua área de transferência para a instância gerenciada de SQL para uso no próximo início rápido clicando no botão Copiar para área de transferência .

![recuperação](/img/recuperacao.png)

O valor copiado representa um **FQDN** que é o nome de domínio totalmente qualificado, que pode ser usado para se conectar à Instância Gerenciada de SQL. Isso é semelhante ao seguinte endereço de exemplo: *nome_do_seu_host.a1b2c3d4e5f6.database.windows.net*.

Fontes:

Por falta de acesso ao portal do azure as imagens foram extraída de [microsoft learning](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal).

*Isto é uma atividade de curso de AZ 900 da DIO*