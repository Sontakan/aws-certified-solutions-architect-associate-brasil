# Mini Simulados por Dominio

## Como usar

- 4 blocos de 5 questões (20 questões no total).
- Tempo recomendado: 8 a 10 minutos por bloco.
- Correção imediata com registro no caderno de erros.

## Bloco A: Resiliencia

1. Cenario exige failover automatico entre zonas com minimo downtime. Qual estrategia e mais aderente?  
A) Instancia unica maior. B) Multi-AZ com monitoramento e failover nativo. C) Backup semanal manual. D) Escala vertical apenas.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** B

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa A está errada:**
mantem ponto unico de falha.

</details>

2. Aplicacao com pico imprevisivel precisa absorver carga sem perder requisicoes.  
A) Fila desacoplada + consumidores elastico. B) Processamento sincrono fixo. C) Retry manual no cliente. D) Bloquear requisicoes extras.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
saturacao sob pico.

</details>

3. Requisito de DR com RPO baixo e custo moderado.  
A) Backup anual. B) Pilot light. C) Sem replicacao. D) Apenas snapshots locais.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** B

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa C está errada:**
sem estrategia de recuperacao.

</details>

4. Alta disponibilidade de banco relacional transacional.  
A) Read replica apenas. B) Multi-AZ. C) Cache local. D) Instancia spot.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** B

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa A está errada:**
replica nao substitui failover sincronizado.

</details>

5. Distribuicao global de conteudo estatico com baixa latencia.  
A) CloudFront. B) EC2 unica regiao. C) NAT Gateway. D) SQS.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
latencia alta fora da regiao.

</details>

## Bloco B: Performance

6. Leitura massiva e repetitiva em dados quentes de sessao. Melhor apoio?  
A) Cache gerenciado. B) Snapshot diario. C) Log manual. D) ASG sem cache.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa D está errada:**
escala compute sem reduzir latencia de dado.

</details>

7. API com throughput variavel e baixa operacao.  
A) Serverless com escala automatica. B) EC2 fixa. C) Processo cron. D) Monolito sem balanceador.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
capacidade fixa pode saturar.

</details>

8. DynamoDB com leitura irregular e picos.  
A) Capacity mode sob demanda. B) Provisionado estatico sem autoscaling. C) Banco local. D) Planilha CSV.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
risco de throttling.

</details>

9. Consulta analitica sobre dados em S3 sem ETL pesado inicial.  
A) Athena. B) NAT Gateway. C) IAM Identity Center. D) Route 53.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa D está errada:**
DNS nao executa consulta.

</details>

10. Conectividade privada a servico AWS sem sair para internet.  
A) VPC Endpoint. B) NAT publico. C) Bastion obrigatorio. D) VPN on-prem para tudo.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
rota pela internet e custo maior.

</details>

## Bloco C: Seguranca

11. Credencial de aplicacao com rotacao automatica.  
A) Secrets Manager. B) Arquivo texto em EC2. C) Variavel fixa em pipeline. D) KMS sozinho.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa D está errada:**
KMS nao faz ciclo de vida de segredo.

</details>

12. Menor privilegio em IAM significa:  
A) Politica ampla para simplificar. B) Permissao minima necessaria por funcao. C) Mesmo role para tudo. D) Sem logs.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** B

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa A está errada:**
amplia superficie de risco.

</details>

13. Necessidade de trilha de auditoria de API calls.  
A) CloudTrail. B) CloudFront. C) EFS. D) Snowball.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
distribuicao, nao auditoria.

</details>

14. Criptografia de dados em repouso gerenciada por chave cliente.  
A) KMS com CMK. B) SG inbound. C) ASG policy. D) IAM group.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa D está errada:**
IAM group nao cifra dados.

</details>

15. Segmentar trafego entre camadas na VPC.  
A) Security Groups e NACLs por funcao. B) Tudo em subnet publica. C) Porta liberada 0.0.0.0/0. D) Um unico SG amplo.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa C está errada:**
exposicao excessiva.

</details>

## Bloco D: Custo

16. Dado raramente acessado, retencao longa.  
A) Classe de arquivamento adequada. B) Standard para tudo. C) EBS io2 para backup frio. D) Replicar sem necessidade.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
custo recorrente desnecessario.

</details>

17. Carga previsivel 24x7 com EC2.  
A) Estrategia de compra com desconto de compromisso. B) Spot para banco critico unico. C) On-demand sem analise. D) Escala manual diaria.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
risco de interrupcao.

</details>

18. Lambda com execucao curta e esporadica para reduzir custo operacional.  
A) Bom encaixe serverless. B) ECS permanente obrigatorio. C) Cluster dedicado fixo. D) Banco como fila.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa C está errada:**
custo fixo alto para carga eventual.

</details>

19. Evitar custo de transferencia indevida para servicos AWS internos.  
A) Endpoints privados quando aplicavel. B) NAT para tudo. C) Tunnel manual. D) S3 publico.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa B está errada:**
rota mais cara para casos internos.

</details>

20. Processo de revisao de custo continuo.  
A) Budgets + alertas + revisao mensal. B) Ver fatura apenas no fim do ano. C) Ignorar tags. D) Sem ownership de gasto.  


<details>
<summary><strong>Ver resposta</strong></summary>

✅ **Resposta correta:** A

**Explicação:**
A alternativa correta atende ao requisito principal sem adicionar complexidade desnecessária.

**Por que a alternativa C está errada:**
sem tags perde rastreabilidade.

</details>



