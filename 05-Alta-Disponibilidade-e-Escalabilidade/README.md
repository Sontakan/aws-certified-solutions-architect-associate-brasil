# Alta Disponibilidade e Escalabilidade

Este módulo apresenta os conceitos essenciais de **Alta Disponibilidade e Escalabilidade** no contexto de arquitetura AWS para SAA-C03. O foco é apoiar decisões de design com clareza, priorizando disponibilidade, segurança, eficiência de custo e simplicidade operacional.

## O que dominar neste módulo

- Papel do serviço na arquitetura de referência.
- Decisões de projeto que aparecem com frequência em cenários de prova.
- Integrações mais comuns com serviços adjacentes.
- Limites práticos, riscos recorrentes e mitigação básica.

## Intuição de Arquitetura

Ao modelar uma solução com Alta Disponibilidade e Escalabilidade, avalie primeiro o requisito crítico do sistema: latência, resiliência, conformidade ou elasticidade. Em seguida, escolha o padrão mínimo que atende ao objetivo sem aumentar complexidade desnecessária. Em cenários de exame, respostas fortes costumam equilibrar três fatores: desacoplamento entre componentes, observabilidade para operação contínua e proteção de dados em repouso e em trânsito.

Também é importante diferenciar decisões de curto prazo (entrega rápida com baixa sobrecarga operacional) de decisões de escala (governança, automação e padronização). Para cargas variáveis, prefira mecanismos gerenciados e políticas automáticas de ajuste. Para cargas previsíveis, otimize capacidade e custos com estratégias de dimensionamento e armazenamento adequadas.

## Padrões que mais caem

- Arquitetura altamente disponível com falha isolada por componente.
- Camadas desacopladas para absorção de picos e retry controlado.
- Segurança por menor privilégio e segmentação de acesso.
- Observabilidade com métricas, logs e alarmes orientados a ação.

## Roteiro de revisão rápida

1. Leia o cheatsheet.md antes de resolver questões.
2. Use flashcards.md para reforço de termos-chave.
3. Execute o lab.md para fixar fluxo e integração.
4. Retorne às questões e valide evolução no domínio.

---

## Estudos complementares

Para revisar fundamentos de cloud e servicos essenciais da AWS, vale combinar esta etapa com a trilha Cloud Practitioner:
https://github.com/Thiago-code-lab/aws-certified-cloud-practitioner-brasil

Como extensao opcional, a trilha AI Practitioner conecta arquitetura com IA generativa e Bedrock:
https://github.com/Thiago-code-lab/aws-certified-ai-practitioner-brasil

