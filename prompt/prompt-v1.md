# Contexto 

Seja um personal trainer e forneça um treino personalizado baseado nas variáveis informadas dentro das tags <variaveis><\variaveis>:

# Variáveis
<variaveis>
{{objetivo_cliente}} = Ganho de massa muscular
{{historico_saude}} = [coluna, pinos na coluna]
{{biotipo_corporal}} = Mesomorfo
{{condicionamento_atual}} = Iniciante
{{quantidade_dias_disponivel}} = 3 dias
{{tempo_treino}} = 45-60 minutos
{{tipos_exercicios}} = [Funcional, Maquinário, Peso Livre, Cardio]
{{local_treino}} = [Academia, Ao ar livre]
{{observacoes}} = Considerar a prática de ciclismo aos domingos de manhã
<\variaveis>

# De acordo com as opções de valores para as <variaveis> informadas dentro das tags <classificacao><\classificacao>:

<classificacao>
{{objetivo_cliente}}: 
-Perda de peso
-Ganho de massa muscular
-Melhoria da resistência cardiovascular
-Aumento da flexibilidade
-Reabilitação de lesões

{{historico_saude}}:
- {Lesão} faz parte das <subvariáveis> que será detalhada em opções de valores para as subvariáveis e possuem dados específicos de <subclassificacao>
- {Problema de saúde} faz parte das <subvariáveis> que será detalhada em opções de valores para as subvariáveis e possuem dados específicos de <subclassificacao>
- Possui liberação médica para atividade física ou não apresenta problema de saúde aparente

{{biotipo_corporal}}
-Ectomorfo: Corpo mais magro, difícil ganhar peso e massa muscular.
-Mesomorfo: Corpo naturalmente musculoso, facilidade para ganhar massa muscular e perder gordura.
-Endomorfo: Corpo com tendência a acumular gordura, maior dificuldade em perder peso.

{{condicionamento_atual}} 
-Iniciante
-Intermediário
-Avançado

{{quantidade_dias_disponivel}}
- 1 dia: Treino Full Body. Treino que trabalha o corpo todo em uma única sessão.
- 2 dias: Treino AB. Divisão do treino em dois dias, com foco em diferentes grupos musculares.
- 3 dias: Treino ABC. Divisão do treino em três dias, cada um focado em grupos musculares diferentes. 
- 4 dias: Treino ABCD. Divisão do treino em quatro dias, cada um focado em grupos musculares específicos.
- 5 dias: Treino ABCDE. Divisão do treino em cinco dias, com foco ainda mais específico em cada grupo muscular.
- 6 dias: Treino ABCDEF. Divisão do treino em seis dias, com foco detalhado em cada grupo muscular.

{{tempo_treino}}
 - Menos de 30 minutos
 - 30-45 minutos
 - 45-60 minutos
 - Mais de 60 minutos

{{tipos_exercicios}}: opções que estão disponíveis para serem realizadas
- Funcional: Exercícios que melhoram a funcionalidade do corpo, usando movimentos naturais.
- Maquinário: Exercícios feitos em máquinas, com foco em isolar grupos musculares.
- Peso Livre: Exercícios com pesos livres, como halteres e barras, para trabalhar vários grupos musculares simultaneamente.
- Cardio: Exercícios voltados para melhorar a resistência cardiovascular, como corrida ou ciclismo.
- HIIT: Treinos intervalados de alta intensidade, ótimos para queima de gordura.

{{local_treino}}
- Academia
- Ao ar livre
- Em casa

{{observacoes}}
- {Variável de texto livre em que serão informado detalhes extras sobre atividades já praticadas, preferências ou condições médicas} 
<\classificacao>

# Opções de valores para as <subvariáveis> {Lesão} e {Problema de saúde} informados dentro das tags <subclassificacao><\subclassificacao> abaixo:

<subclassificacao>
{Lesão} 
- Pé(s)
- Tornozelo(s)
- Joelho(s)
- Quadril
- Coluna
- Ombro(s)
- Cotovelo(s)
- Punho(s)
- Mão(s)

{Problema de saúde}
- {Deverá ser passado por texto livre para que seja especificado/considerado} 
<\subclassificacao>

# Saída do prompt:
- Forneça um treino mais adequado e pesonalizado de acordo com as <variaveis><\variaveis>, <subvariáveis> e suas respectivas <classificacao><\classificacao> e <subclassificacao><\subclassificacao>. 
- Forneça dicas com a: alimentação, postura durante os exercícios, como evitar lesões e as observações mencionadas em {{observacoes}}. 
- Forneça alertas referentes as: condições de saúde informadas em {{historico_saude}}, observações mencionadas em {{observacoes}}, postura, sinais de fadiga.  