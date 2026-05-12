# Cartoes de Revisao

### Card 01

**Pergunta:** Qual e o primeiro filtro para escolher servicos em um cenario SAA-C03?
**Resposta:** Identificar o requisito dominante do enunciado (resiliencia, desempenho, seguranca ou custo). A escolha do servico deve responder a esse eixo antes dos demais.

### Card 02

**Pergunta:** O que caracteriza uma boa alternativa de prova em arquitetura AWS?
**Resposta:** Solucao gerenciada, com menor complexidade operacional, que atende requisito tecnico e reduz risco de falha.

### Card 03

**Pergunta:** Quando desconfiar de uma alternativa aparentemente completa demais?
**Resposta:** Quando ela adiciona muitos componentes sem necessidade do cenario. Em prova, excesso de arquitetura costuma indicar custo e operacao desnecessarios.

### Card 04

**Pergunta:** Qual sinal indica necessidade de desacoplamento?
**Resposta:** Pico imprevisivel, processamento assincrono ou dependencia forte entre componentes produtores e consumidores.

### Card 05

**Pergunta:** Em seguranca, qual erro recorrente o exame cobra?
**Resposta:** Usar permissao ampla por conveniencia e nao aplicar menor privilegio com escopo especifico por funcao.

### Card 06

**Pergunta:** Como interpretar exigencia de “baixo esforco operacional” no enunciado?
**Resposta:** Priorizar servicos totalmente gerenciados e automacao nativa, evitando manutencao manual de infraestrutura.

### Card 07

**Pergunta:** Como diferenciar alta disponibilidade de recuperacao de desastre?
**Resposta:** Alta disponibilidade trata continuidade local/zonal com failover rapido; DR trata retomada apos eventos de maior impacto, incluindo regiao.

### Card 08

**Pergunta:** Qual tecnica ajuda a eliminar opcoes erradas mais rapido?
**Resposta:** Verificar incompatibilidade direta com requisito: protocolo, latencia, consistencia, custo alvo ou restricao de seguranca.

### Card 09

**Pergunta:** Por que observabilidade aparece em varios dominios do exame?
**Resposta:** Porque operacao confiavel depende de metricas, logs e alarmes para detectar degradacao e agir antes de indisponibilidade ampla.

### Card 10

**Pergunta:** Qual e um bom fechamento de revisao apos este modulo?
**Resposta:** Resolver questoes em tempo controlado e registrar no caderno de erros o motivo da escolha incorreta e a regra de decisao correta.
