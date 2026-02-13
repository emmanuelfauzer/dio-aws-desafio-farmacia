# 📊 Estimativa de Custos AWS -- Mensal

**Projeto:** Plataforma Farmacêutica Digital\
**Arquitetura:** EC2 + RDS + S3\
**Região estimada:** us-east-1

------------------------------------------------------------------------

## 1️⃣ Amazon EC2 (Camada de Aplicação)

### Cenário considerado:

-   2 instâncias t3.medium\
-   730 horas/mês (24x7)\
-   30 GB EBS por instância\
-   Application Load Balancer

### Cálculo estimado:

  Item                        Valor aproximado
  --------------------------- -------------------
  2x EC2 t3.medium            \~US\$ 61
  EBS (60 GB total)           \~US\$ 6
  Application Load Balancer   \~US\$ 18
  **Subtotal EC2**            **\~US\$ 85/mês**

------------------------------------------------------------------------

## 2️⃣ Amazon RDS (Banco de Dados)

### Cenário considerado:

-   1 instância db.t3.medium\
-   100 GB armazenamento (GP2)\
-   Backup automático habilitado\
-   Multi-AZ desabilitado

### Cálculo estimado:

  Item                     Valor aproximado
  ------------------------ -------------------
  RDS db.t3.medium         \~US\$ 55
  Armazenamento (100 GB)   \~US\$ 11
  Backup adicional         \~US\$ 5
  **Subtotal RDS**         **\~US\$ 71/mês**

> Caso habilite Multi-AZ, o valor pode chegar a \~US\$ 120--140/mês.

------------------------------------------------------------------------

## 3️⃣ Amazon S3 (Armazenamento)

### Cenário considerado:

-   200 GB armazenamento padrão\
-   50.000 requisições mensais

### Cálculo estimado:

  Item                          Valor aproximado
  ----------------------------- -------------------
  200 GB (S3 Standard)          \~US\$ 4.60
  Requisições e transferência   \~US\$ 5
  **Subtotal S3**               **\~US\$ 10/mês**

------------------------------------------------------------------------

# 💰 Resumo Geral

  Serviço              Custo Estimado
  -------------------- --------------------
  EC2                  \~US\$ 85
  RDS                  \~US\$ 71
  S3                   \~US\$ 10
  **Total Estimado**   **\~US\$ 166/mês**

------------------------------------------------------------------------

## 💵 Estimativa em Reais (Dólar a R\$ 5,00)

**US\$ 166 ≈ R\$ 830/mês**

------------------------------------------------------------------------

## 🎯 Cenário Otimizado para Redução de Custos

-   Uso de instâncias reservadas (1 ano)\
-   Redução para db.t3.small\
-   Políticas de ciclo de vida no S3\
-   Auto Scaling sob demanda

**Estimativa otimizada:** \~US\$ 110--130/mês

------------------------------------------------------------------------

## 📌 Observação

Os valores são estimativas e podem variar conforme região, volume real
de uso, tráfego de rede e variação cambial.
