# Criando uma máquina virtual no portal do Azure.

Breve introdução
1. Criando a máquina.
2. Conectando a VM
3. Instalando o servidor
4. Exibindo a página de boas vindas.
5. Fontes

## Criando a máquina

Primeiro, acesse o portal do azure através do link [Portal do Azure](https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize?redirect_uri=https%3A%2F%2Fportal.azure.com%2Fsignin%2Findex%2F&response_type=code%20id_token&scope=https%3A%2F%2Fmanagement.core.windows.net%2F%2Fuser_impersonation%20openid%20email%20profile&state=OpenIdConnect.AuthenticationProperties%3D5rfrOAc05bm1iMnacUsMObp3eWdKwEJ41a3ZA4zrX6-f6rV0QBXSP2YifhOGbrkwLDjnxEtj7nnclEEQaFpR5XruSql3NAVZzCTFobENvYgirFhByaEi2cheS6RcphWXT8UQ2c54px8CcW9almBHuS_PJ2PG5PY8qpyadCgGUtr-SOsjUzyiwmavFqL30hE8IuHauQ_ictlEsgwp26YSsEy7xw2wUXRFb1A9DX2K1r1v330rqkym5g9tbGxHqkcQ4xMV80RGMYvUvUShWP8zJHcHcbkbPkQsGGPCVSDMTFxwLITNFWk_OgC5KvSraUTEo_tEsEWAMdAwXSLaUFWwV-t2qpj5rWKYgGZVHM_fQV84lKFJL_GKMLYA8EJ_d8RGnn2vNeQv0MzuzWKAbXUKNvRXI-61fnNiZIklK5P-05L6URRMfRRb9EZY8BEpRAnV56pyeMbVSB80Uyo9q9IsPlQ2Do-9xTsjxYB9dwpWKzA&response_mode=form_post&nonce=638869267920167917.Nzk3NWIxNmYtN2Y0My00ODFlLWFmZDktM2Q4MGZlZTMwZTJkM2EzNTQ5ZTAtNzcxNC00NTQ1LTk3YzItMWMwZjljM2FhZjQ1&client_id=c44b4083-3bb0-49c1-b47d-974e53cbdf3c&site_id=501430&client-request-id=5bbb6159-139e-4945-a1ff-695b1b3f6bc6&x-client-SKU=ID_NET472&x-client-ver=8.3.0.0)
No campo de pesquisa digite máquina virtual, depois em serviços clique em criar e selecione Máquina Virtual do Azure.

Em detalhes da instância, preencha conforme imagem abaixo:

![instancia](/image/Instance%20details.png)

**! ATENÇÃO**:
Poderá aparecer uma opção para escolher a zona, para saber mais clique no botão indicado.

![zona](/image/Zona.png)

Agora entre com a sua conta de administrador, fornecendo o usuário e a senha:

![admin](/image/admin.png)

Em Regras de porta de entrada, selecione **Permitir portas selecionas**, e depois selecione **RDP (3389)** e **HTTP (80)**.

![portas](/image/portas.png)

O resto deixe padrão, e selecione **Examinar** + **Criar**, conforme ilustrado abaixo:

![criar](/image/criar.png)

Após a validação da execução, clique em **Criar**.

![criar2](/image/criar2.png)

Concluída a implantação, clique em **Ir para o recurso**.

![recursos](/image/recurso.png)

## Conectando a máquina virtual

Na página de visão geral da sua VM, clique em **Conectar**.

![conectar](/image/conectar.png)

Agora, siga os passos abaixo:

* Mantenha as opções para se conectar por endereço de IP pela porta **3399** (configurada anteriormente) e clique em **Baixar arquivo RDP**.
* Abra o arquivo baixado e clique em **Conectar**
* Na janela **Segurança do Windows**, selecione **Mais opções** e **Usar uma conta diferente**. Digite o nome de usuário como localhost\XXXXXXX, insira a senha que você criou para a máquina virtual e clique em **OK**.

**! ATENÇÃO**:
Poderá aparecer um aviso de certificado, clique em **Sim** ou **Continuar**.

## Instalando o servidor WEB

Execute o comando abaixo no PowerShell:

Install-WindowsFeature -name Web-Server -IncludeManagementTools 

## Exibindo a página de boas-vindas do 

Passo a passo:

* Acesse o portal
* Selecione a VM
* copie o endereço de IP passando mouse sob e clicando em **copiar para transferência**
* Cole em um guia do navegador
* A página de boas-vindas aparecerá

##

Fontes:

Por falta de acesso ao portal do azure as imagens foram extraída de [microsoft learning](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal).

*Isto é uma atividade de curso de AZ 900 da DIO*