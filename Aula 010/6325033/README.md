README

Renan Dias
RA:6325033

Respostas:

Questão 1: Modelos de Serviço em Nuvem

a) A AWS EC2 representa o modelo IaaS (Infrastructure as a Service).
Nesse modelo, o usuário é responsável por gerenciar o sistema operacional, aplicações, dados e configurações, enquanto a AWS fornece a infraestrutura (máquinas virtuais, rede e armazenamento).

b)

SaaS: Amazon WorkMail ou AWS QuickSight
PaaS: AWS Elastic Beanstalk

Questão 2: Identidade e Acesso (IAM)

a) Um Usuário IAM representa uma identidade individual com credenciais próprias. Já um Grupo IAM é uma coleção de usuários que compartilham as mesmas permissões.

b) Criar uma Role IAM é mais seguro porque ela fornece permissões temporárias e específicas para a instância EC2, evitando o uso de credenciais fixas (como Root ou Admin), reduzindo riscos de vazamento e aumentando a segurança do ambiente.

Questão 3: Rede Virtual na AWS (VPC)

a) Uma Subnet é uma subdivisão da VPC usada para organizar e segmentar recursos em uma rede.
A Subnet Pública tem acesso direto à Internet, enquanto a Subnet Privada não possui acesso direto e depende de recursos intermediários para comunicação externa.

b) O componente obrigatório é o Internet Gateway (IGW) para permitir acesso à Internet.
Para inspeção de tráfego em nível de Subnet, utiliza-se o Network ACL (NACL).

Questão 4: Instâncias EC2

a) O termo é AMI (Amazon Machine Image).

b) O comando é: ssh -i minha_chave.pem ec2-user@54.123.45.67

Questão 5: Comandos AWS CLI
aws configure

Listar instâncias EC2:
aws ec2 describe-instances

Criar bucket S3 (região sa-east-1):
aws s3 mb s3://meu-bucket-tf10 --region sa-east-1

Descrever VPCs:
aws ec2 describe-vpcs

