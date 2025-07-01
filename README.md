# Criando uma máquina virtual no portal do Azure.

Breve introdução
1. Criando a máquina.
2. Conectando a VM
3. Instalando o servidor
4. Exibindo a página de boas vindas.

## Criando a máquina

Primeiro, acesse o portal do azure através do link [Portal do Azure](https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize?redirect_uri=https%3A%2F%2Fportal.azure.com%2Fsignin%2Findex%2F&response_type=code%20id_token&scope=https%3A%2F%2Fmanagement.core.windows.net%2F%2Fuser_impersonation%20openid%20email%20profile&state=OpenIdConnect.AuthenticationProperties%3D5rfrOAc05bm1iMnacUsMObp3eWdKwEJ41a3ZA4zrX6-f6rV0QBXSP2YifhOGbrkwLDjnxEtj7nnclEEQaFpR5XruSql3NAVZzCTFobENvYgirFhByaEi2cheS6RcphWXT8UQ2c54px8CcW9almBHuS_PJ2PG5PY8qpyadCgGUtr-SOsjUzyiwmavFqL30hE8IuHauQ_ictlEsgwp26YSsEy7xw2wUXRFb1A9DX2K1r1v330rqkym5g9tbGxHqkcQ4xMV80RGMYvUvUShWP8zJHcHcbkbPkQsGGPCVSDMTFxwLITNFWk_OgC5KvSraUTEo_tEsEWAMdAwXSLaUFWwV-t2qpj5rWKYgGZVHM_fQV84lKFJL_GKMLYA8EJ_d8RGnn2vNeQv0MzuzWKAbXUKNvRXI-61fnNiZIklK5P-05L6URRMfRRb9EZY8BEpRAnV56pyeMbVSB80Uyo9q9IsPlQ2Do-9xTsjxYB9dwpWKzA&response_mode=form_post&nonce=638869267920167917.Nzk3NWIxNmYtN2Y0My00ODFlLWFmZDktM2Q4MGZlZTMwZTJkM2EzNTQ5ZTAtNzcxNC00NTQ1LTk3YzItMWMwZjljM2FhZjQ1&client_id=c44b4083-3bb0-49c1-b47d-974e53cbdf3c&site_id=501430&client-request-id=5bbb6159-139e-4945-a1ff-695b1b3f6bc6&x-client-SKU=ID_NET472&x-client-ver=8.3.0.0)

## Tipos de nuvem

#### Nuvem privada

É um ambiente de computaçõ em nuvem que oferece os benefícios da nuvem para uma única organização, com recursos dedicadis e isolado.
* Recursos de computação em nuvem dedicados e isolados para uma única organização
* Maior controle sobre a infraestrutura, segurança e personalidade do ambiente
* Acesso restrito aos usuários da organização

#### Nuvem pública

É um serviço de computação onde os recursos, como armazenamento e poder de processamento, são oferecidos por terceiros através da internet, e podem ser utilizados por qualquer pessoa ou empresa mediante uma assinatura ou pagamento por uso.

* A infraestrutura é compartilhada entre múltiplos usuários.
* Possui capacidade de aumentar ou diminuir os recursos de acordo com a demanda
* Os serviços podem ser acessados de qualquer lugar atráves da internet

#### Nuvem Híbrida

É um ambiente de computação que combina uma nuvem privada com uma nuvem pública. Onde se pode combinar o controle e a segurança de uma nuvem privada com a escalabilidade e flexibilidade de uma nuvem pública.

* As empresas podem escolher onde executar suas aplicações e armazenar seus dados, movendo-os entre os ambientes conforme necessário.
* Pode otimizar os custos, utilizando a nuvem pública para tarefas que não exigem recursos dedicados, e a nuvem privada para tarefas que demandam mais controle.

## CapEx e OpEX

#### Despesas de Capital ( CapEx )

Refere-se a investimentos em ativos de longo prazo, como a compra de equipamentos ou a construção de um novo prédio.

#### Despesas Operacionais ( OpEx )

Refere-se aos custos do dia a dia para manter a empresa funiconando.

#### Princípais diferentes entre CapEx e OpEx

| Características | CapEx | OpEx |
| --- | --- | --- |
| Prazo | Longo prazo | Curto prazo |
| Natureza | Investimento em ativos | Despesas operacionais |
| Pagamento | Geralmente à vista | Geralmente recorrente |
| Impacto financeiro | Depreciação ao longo do tempo | Custo direto no período |
| Processo de compra | Mais rigorose e burocráticos | Mais rápido e menos burocrático |

#### Modelo baseado em consumo

É onde os clientes pagam por um serviço ou produto com base no quanto eles o utilizam, no lugar de ter um valor pré-determinado.
No modelo baseado em consumo, o provedor define um preço por unidade de uso e o cliente paga apenas pela quantidade de uso que realmente fizer durante um determinado período.

* Esse modelo permite um controle maior sobre os gastor, pois o cliente paga apenas pelo que utiliza.
* Empresas podem facilmente adicionar ou remover recursos conforme o crescimento ou mudança de demanda.
* Os clientes podem aumentar ou diminuir o uso conforme a necesssidade, sem compromisso de longo prazo.




*Isto é uma atividade de curso de AZ 900 da DIO*

