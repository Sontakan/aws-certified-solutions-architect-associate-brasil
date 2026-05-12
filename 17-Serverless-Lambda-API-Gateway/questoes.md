# Questoes de Revisao

## Questao 1

Uma aplicacao sofre picos repentinos de requisicoes e precisa manter tempo de resposta estavel sem aumentar operacao manual. Qual abordagem e mais adequada?

A) Escalar verticalmente uma instancia unica em horarios fixos.
B) Usar servicos gerenciados com escala automatica orientada por metrica.
C) Criar script manual de aumento de capacidade durante incidente.
D) Migrar toda carga para instancia maior e manter fixa.

**Resposta correta:** B  
**Explicacao:** Escala automatica em servicos gerenciados responde variacao real de demanda e reduz intervencao operacional.  
**Por que A esta errada:** Escala vertical fixa nao acompanha variacao imprevisivel e cria risco de saturacao.

## Questao 2

Um requisito exige reduzir impacto de falha de um componente sem perder mensagens. Qual padrao e mais indicado?

A) Processamento sincrono direto entre todos os servicos.
B) Banco relacional unico como fila de trabalho.
C) Camada de mensageria com retentativa e desacoplamento.
D) Retry no cliente sem persistencia intermediaria.

**Resposta correta:** C  
**Explicacao:** Fila desacopla produtor e consumidor, preserva mensagens e permite retry controlado.  
**Por que D esta errada:** Retry no cliente nao garante durabilidade em falha do produtor ou da rede.

## Questao 3

O enunciado destaca conformidade e protecao de dados sensiveis. Qual combinacao e mais alinhada?

A) Credenciais em texto no codigo e acesso amplo para facilitar deploy.
B) Controle por menor privilegio, criptografia e trilha de auditoria.
C) Ambiente sem logs para reduzir custo.
D) Compartilhar chave entre equipes sem rotacao.

**Resposta correta:** B  
**Explicacao:** Seguranca robusta no exame combina identidade, criptografia e auditabilidade.  
**Por que C esta errada:** Ausencia de logs compromete governanca, rastreabilidade e investigacao.

## Questao 4

Uma arquitetura precisa reduzir custo sem degradar experiencia do usuario. Qual decisao e mais consistente?

A) Escolher sempre classe de armazenamento mais barata.
B) Ajustar servico ao padrao real de acesso e retenção.
C) Desligar monitoramento para economizar.
D) Concentrar tudo em um unico componente para simplificar.

**Resposta correta:** B  
**Explicacao:** Otimizacao de custo depende de perfil de uso, latencia esperada e frequencia de acesso.  
**Por que A esta errada:** Classe mais barata pode aumentar latencia de recuperacao e quebrar requisito funcional.

## Questao 5

Duas opcoes atendem funcionalmente o cenario. Como escolher a melhor no SAA-C03?

A) Preferir a alternativa com mais servicos para mostrar robustez.
B) Escolher a opcao com menor numero de recursos, sem avaliar risco.
C) Comparar trade-offs de operacao, resiliencia e custo total.
D) Selecionar a tecnologia mais nova da AWS por padrao.

**Resposta correta:** C  
**Explicacao:** O exame premia equilibrio tecnico e clareza de trade-off, nao volume de componentes.  
**Por que D esta errada:** Novidade tecnologica nao substitui aderencia ao requisito de negocio.
