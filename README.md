# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 12/02/2026
Empresa: Abstergo Industries
Responsável: Emmanuel Fauzer

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Emmanuel Fauzer. 
O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.
																																										
## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos especí­ficos. Os serviços escolhidos foram: Amazon EC2, Amazon RDS e Amazon S3. A seguir, serão descritas as etapas do projeto:

Etapa 1:
- Nome da ferramenta: Amazon Elastic Compute Cloud (EC2)
- Foco da ferramenta: Processamento e hospedagem da aplicação
- Caso de uso: Hospedagem do backend da plataforma da farmácia
- Justificativa da Escolha: O Amazon EC2 foi escolhido para hospedar a aplicação principal da farmácia (API backend e possíveis serviços administrativos).
- Benefício Financeiro: A empresa deixa de investir em servidores físicos (CAPEX) e passa a utilizar modelo OPEX, pagando apenas pelos recursos utilizados. Além disso, pode ajustar instâncias conforme a demanda (por exemplo, maior tráfego em campanhas promocionais).

Etapa 2:
- Nome da ferramenta: Amazon Relational Database Service (RDS)
- Foco da ferramenta: Banco de dados relacional gerenciado
- Caso de uso: Armazenamento de dados de clientes, pedidos, estoque e medicamentos.
- Justificativa da Escolha: Uma farmácia precisa de consistência transacional (ACID), principalmente para: Controle de estoque, Processamento de pedidos, Cadastro de clientes, Histórico de compras.
- Benefício Financeiro: Elimina a necessidade de manter equipe dedicada para administração de banco de dados e reduz riscos de falhas que poderiam gerar prejuízo financeiro.

Etapa 3:
- Nome da ferramenta: Amazon Simple Storage Service (S3)
- Foco da ferramenta: Armazenamento de objetos
- Caso de uso: Armazenamento de imagens de produtos, notas fiscais, receitas médicas digitalizadas e backups
- Justificativa da Escolha: O Amazon S3 foi escolhido por sua alta durabilidade (99.999999999%) e escalabilidade praticamente ilimitada.
- Benefício Financeiro: Armazenamento de baixo custo. Possibilidade de utilizar classes como S3 Standard-IA ou Glacier para reduzir custos. Eliminação de necessidade de storage local.

## Conclusão
A implementação dos serviços EC2, RDS e S3 na Abstergo Industries proporciona:
- Redução de custos com infraestrutura física
- Maior disponibilidade e confiabilidade
- Escalabilidade sob demanda
- Segurança e conformidade no armazenamento de dados
- Facilidade de manutenção
- A arquitetura escolhida é sólida, escalável e adequada para uma plataforma farmacêutica digital, permitindo crescimento sustentável da operação.

## Próximos passos:
- Implementação de monitoramento com CloudWatch
- Configuração de políticas de segurança com IAM
- Uso de Load Balancer para alta disponibilidade
- Avaliação futura de serviços serverless para otimização de custos

## Anexos
- Diagrama de Arquitetura da Solução
- Estimativa de Custos AWS

Assinatura do Responsável pelo Projeto:
Emmanuel Fauzer
