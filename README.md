


RELATÓRIO DE ENTREGA
Entrega referente a alteração do sistema logico do sistema de abastecimento de água
Local: PERINI BUSINESS PARK
Elaborado por: André Araújo dos Santos

INTRODUÇÃO
Este serviço se refere mudança da logica do sistema de abastecimento das cisternas e das caixas de consumo e RTI do parque industrial
O sistema constitui de um CLP Siemens S7-1200 e uma IHM SIMATIC HMI - KTP700 BASIC
Onde controla 5 bombas e 4 válvulas. Também habilita o acionamento de um sistema de abastecimento da cisterna vinda de uma estação de tratamento de agua
Também foi instalado um sistema de acesso remoto para trabalho de atendimento do sistema

COMPONENTES
CLP SIETEMS S7-1200 com cartão de entrada digital e analógico
SIEMENS IHM KTP-700 BASICO
SWITCH INDUSTRIAL WEG LINHA SWU

ESCOPO
Alterado logicas conforme pedido do cliente para que o sistema seja mais bem aproveitado
Entre as mudanças ficaram conforme tabela abaixo
1 ABASTECIMENTO DAS CISTERNAS
1 Prioridade sempre abastecer a cisterna 1
2 Cisterna 1 para de ser abastecida quando nível atingir a 100%
3 Cisterna 1 volta a ser abastecida quando atingir um valor inferior a 80%
4 Cisterna 2 será abastecida quando sistema estiver conforme item 1.2
5 Cisterna 2 para de ser abastecida quando chegar a 100% ou conforme item 1.3
6 Cisterna 2 volta a ser abastecida quando nível atingir 90% e conforme item 1.3
2 CONSUMO DAS CISTERNAS
1 Prioridade e sempre utilizar a cisterna 1 para abastecimentos das caixas (CONSUMO E RTI) exceto conforme item 2.7
2 A cisterna 1 para de abastecer quando atingir o nível inferior a 10%
3 A cisterna 1 para de abastecer conforme itens 3.2 e 3.6
4 A cisterna 1 volta a abastecer conforme item 2.8
5 A cisterna 2 abastece conforme item 2.2
6 A cisterna 2 para de abastecer conforme itens 2.4, 3.2 e 3.6
7 Toda segunda feira da semana o sistema prioriza a cisterna 2 para abastecimentos das caixas (CONSUMO E RTI)
8 A cisterna 2 para de abastecer quando atingir o nível inferior a 10%
3 ABASTECIMENTO DAS CAIXAS (CONSUMO E RTI)
1 A prioridade será sempre abastecer a caixa de consumo
2 A caixa de consumo para de ser abastecida quando atingir nível de 100%
3 A caixa de consumo para de ser abastecida conforme itens 2.2 e 2.8
4 A caixa de consumo só volta a ser abastecida quando atingir o nível inferior a 50%
5 A caixa RTI será abastecida conforme item 3.2 
6 A caixa RTI para de ser abastecida quando atingir o nível de 100% ou conforme itens 3.4, 2.2 e 2.8
7 A caixa RTI volta ser abastecida quando atingir o nível inferior a 95%
4 ACIONAMENTOS DAS BOMBAS
1 O sistema funciona com alternância de acionamento de bombas
2 A alternância funciona no intervalo entre o desligamento de uma bomba e o próximo acionamento
3 A bomba de consumo 1 e bomba de consumo 2 se alternam conforme item 4.2
4 Caso uma das bombas de consumo entrar em falha a bomba reserva de consumo entra no revezamento
5 As bombas RTI e bomba reserva RTI se alternam conforme item 4.2
6 O acionamento das bombas sege a regra conforme a guia 3 - ABASTECIMENTO DAS CAIXAS (CONSUMO E RTI)
7 A bomba de ETE será habilitada quando os níveis das cisternas 1 ou 2 estiverem abaixo de 95%
8 A bomba da ETE será desabilitada quando as cisternas 1 e 2 atingirem nível de 100%

A lógica terá em sua constituição um sistema manual para necessidade de fazer alguma função manualmente
Também há todos os dispositivos segurança habilitados na logica como, botão de emergência, falha de sobrecarga e falha dos inversores
Em relação a IHM foi feito alterações do projeto para adequar ao novo sistema
Estas mudanças foram na maioria em tags dos eventos
Devido a problemas na IHM do sistema houve a necessidade da troca da mesma
Também foi instalado um switch industrial para acesso por VPN ao CLP e IHM
Para esta mudança foi necessário troca os endereços do CLP e IHM

ENTREGA
A entrega do serviço foi realizada inloco, com o startup do sistema e simulações
Disponibilizado o arquivo atualizado
Todo arquivo utilizado neste serviço está disponível para todos os envolvidos no serviço no repositório do link abaixo
https://github.com/AeG-automacao/perini-business-park.git
