# Mini Simulados por Dominio

## Como usar

- 4 blocos de 5 questoes (20 questoes no total).
- Tempo recomendado: 8 a 10 minutos por bloco.
- Correcao imediata com registro no caderno de erros.

## Bloco A: Resiliencia

1. Cenario exige failover automatico entre zonas com minimo downtime. Qual estrategia e mais aderente?  
A) Instancia unica maior. B) Multi-AZ com monitoramento e failover nativo. C) Backup semanal manual. D) Escala vertical apenas.  
**Resposta:** B. **Por que A erra:** mantem ponto unico de falha.

2. Aplicacao com pico imprevisivel precisa absorver carga sem perder requisicoes.  
A) Fila desacoplada + consumidores elastico. B) Processamento sincrono fixo. C) Retry manual no cliente. D) Bloquear requisicoes extras.  
**Resposta:** A. **Por que B erra:** saturacao sob pico.

3. Requisito de DR com RPO baixo e custo moderado.  
A) Backup anual. B) Pilot light. C) Sem replicacao. D) Apenas snapshots locais.  
**Resposta:** B. **Por que C erra:** sem estrategia de recuperacao.

4. Alta disponibilidade de banco relacional transacional.  
A) Read replica apenas. B) Multi-AZ. C) Cache local. D) Instancia spot.  
**Resposta:** B. **Por que A erra:** replica nao substitui failover sincronizado.

5. Distribuicao global de conteudo estatico com baixa latencia.  
A) CloudFront. B) EC2 unica regiao. C) NAT Gateway. D) SQS.  
**Resposta:** A. **Por que B erra:** latencia alta fora da regiao.

## Bloco B: Performance

6. Leitura massiva e repetitiva em dados quentes de sessao. Melhor apoio?  
A) Cache gerenciado. B) Snapshot diario. C) Log manual. D) ASG sem cache.  
**Resposta:** A. **Por que D erra:** escala compute sem reduzir latencia de dado.

7. API com throughput variavel e baixa operacao.  
A) Serverless com escala automatica. B) EC2 fixa. C) Processo cron. D) Monolito sem balanceador.  
**Resposta:** A. **Por que B erra:** capacidade fixa pode saturar.

8. DynamoDB com leitura irregular e picos.  
A) Capacity mode sob demanda. B) Provisionado estatico sem autoscaling. C) Banco local. D) Planilha CSV.  
**Resposta:** A. **Por que B erra:** risco de throttling.

9. Consulta analitica sobre dados em S3 sem ETL pesado inicial.  
A) Athena. B) NAT Gateway. C) IAM Identity Center. D) Route 53.  
**Resposta:** A. **Por que D erra:** DNS nao executa consulta.

10. Conectividade privada a servico AWS sem sair para internet.  
A) VPC Endpoint. B) NAT publico. C) Bastion obrigatorio. D) VPN on-prem para tudo.  
**Resposta:** A. **Por que B erra:** rota pela internet e custo maior.

## Bloco C: Seguranca

11. Credencial de aplicacao com rotacao automatica.  
A) Secrets Manager. B) Arquivo texto em EC2. C) Variavel fixa em pipeline. D) KMS sozinho.  
**Resposta:** A. **Por que D erra:** KMS nao faz ciclo de vida de segredo.

12. Menor privilegio em IAM significa:  
A) Politica ampla para simplificar. B) Permissao minima necessaria por funcao. C) Mesmo role para tudo. D) Sem logs.  
**Resposta:** B. **Por que A erra:** amplia superficie de risco.

13. Necessidade de trilha de auditoria de API calls.  
A) CloudTrail. B) CloudFront. C) EFS. D) Snowball.  
**Resposta:** A. **Por que B erra:** distribuicao, nao auditoria.

14. Criptografia de dados em repouso gerenciada por chave cliente.  
A) KMS com CMK. B) SG inbound. C) ASG policy. D) IAM group.  
**Resposta:** A. **Por que D erra:** IAM group nao cifra dados.

15. Segmentar trafego entre camadas na VPC.  
A) Security Groups e NACLs por funcao. B) Tudo em subnet publica. C) Porta liberada 0.0.0.0/0. D) Um unico SG amplo.  
**Resposta:** A. **Por que C erra:** exposicao excessiva.

## Bloco D: Custo

16. Dado raramente acessado, retencao longa.  
A) Classe de arquivamento adequada. B) Standard para tudo. C) EBS io2 para backup frio. D) Replicar sem necessidade.  
**Resposta:** A. **Por que B erra:** custo recorrente desnecessario.

17. Carga previsivel 24x7 com EC2.  
A) Estrategia de compra com desconto de compromisso. B) Spot para banco critico unico. C) On-demand sem analise. D) Escala manual diaria.  
**Resposta:** A. **Por que B erra:** risco de interrupcao.

18. Lambda com execucao curta e esporadica para reduzir custo operacional.  
A) Bom encaixe serverless. B) ECS permanente obrigatorio. C) Cluster dedicado fixo. D) Banco como fila.  
**Resposta:** A. **Por que C erra:** custo fixo alto para carga eventual.

19. Evitar custo de transferencia indevida para servicos AWS internos.  
A) Endpoints privados quando aplicavel. B) NAT para tudo. C) Tunnel manual. D) S3 publico.  
**Resposta:** A. **Por que B erra:** rota mais cara para casos internos.

20. Processo de revisao de custo continuo.  
A) Budgets + alertas + revisao mensal. B) Ver fatura apenas no fim do ano. C) Ignorar tags. D) Sem ownership de gasto.  
**Resposta:** A. **Por que C erra:** sem tags perde rastreabilidade.
