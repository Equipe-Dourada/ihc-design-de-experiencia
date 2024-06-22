## Artefatos: 
### Personas Cenários e Casos de Uso do STP (Sistema de Transferência de Pacientes)

_

| Requisitos Funcionais |
| ------------- |
| RF01: Como médico(a) regulador(a), desejo visualizar, adicionar e remover informações, alterar parâmetros e fazer modificações diversas no prontuário online do paciente antes e durante a transferência.
RF02: Como médico(a) regulador(a), desejo especificar o meio de transporte da transferência do paciente: ambulância terrestre, helicóptero ou avião.
RF03: Como médico(a) regulador(a), desejo selecionar uma unidade hospitalar de destino listada no sistema, de acordo com as necessidades do paciente, para receber a transferência.
RF04: Como médico(a) regulador(a), desejo visualizar uma lista de unidades hospitalares disponíveis para receber transferências, com os meios de contato disponíveis e as informações sobre o pessoal responsável pela recepção.
RF05: Como médico(a) regulador(a), desejo cadastrar o horário de saída do paciente, selecionar a unidade de destino e receber do sistema o horário previsto de chegada.
RF06: Como médico(a), desejo poder realizar solicitações de transferência de pacientes.
RF07: Como médico(a), desejo poder especificar a classificação da transferência a ser realizada, seja ela primária, secundária ou terciária.
RF08: Como médico(a), desejo poder listar todas as drogas administradas no paciente e escrever detalhes de sua utilização no documento de transferência.
RF09: Como médico(a), desejo poder anexar ao documento de transferência do paciente uma lista de verificação dos procedimentos de acondicionamento previamente preparada.
RF10: Como médico(a) da unidade de origem, desejo estabelecer procedimentos a serem seguidos pelos profissionais da unidade de destino e anexá-los ao documento de transferência do paciente.|

## Identificadores e Tabela de Casos de Uso

* UC01: Coordenação de Transferências
* UC02: Logística de Transferência
* UC03: Integração no Sistema de Saúde
* UC04: Comunicação

## Tabela de Casos de Uso:

| ID  | Nome do Caso de Uso | Descrição | Atores Envolvidos | Necessidades Gerais | RF |
| ------------- |--------------| ------------- | ----------- | -------------- | ----- |
|UC01 | Coordenação de Transferências | Coordenação de uma transferência urgente de um paciente em estado crítico. | Dr. Pedro Costa (Médico Regulador), Dr. Lúcia Santos (Médica de Origem), Dr. Augusto Oliveira(Médico de Destino) | Tipos de Dados, Logística de Equipamento, Classificação, Preparação, Equipamentos, Documentação | RF01, RF02, RF03, RF04, RF05, RF06, RF07, RF08, RF09, RF10 |
|UC02 | Logística de Transferência | Planejamento e execução de uma transferência programada para tratamento não urgente.| Dr. Lúcia Santos (Médica de Origem), Dr. Pedro Costa(Médico Regulador), Dr. Augusto Oliveira (Médico de Destino) |Tipos de Dados, Logística de Equipamento, Classificação, Preparação, Equipamentos, Documentação| RF01, RF02, RF03, RF04, RF05, RF06, RF07, RF08, RF09, RF10|
|UC03| Integração no Sistema de Saúde|Integração do software de transferências com os sistemas de saúde existentes.|Dr. Augusto Oliveira(Médico de Destino), Luís Torres (Coordenador de TI)|Tipos de Dados, Logística de Equipamento, Classificação,|Preparação, Equipamentos, Documentação, Segurança de Dados|RF01, RF06|
|UC04|Comunicação |Comunicação e atualização de familiares sobre o status da transferência do paciente.|Mariana|Rodrigues(Parente do Paciente), Dr. Pedro Costa (Médico Regulador)|Tipos de Dados, Logística de Equipamento,|Preparação, Equipamentos, Documentação, Segurança de Dados|RF01, RF05, RF06|


|ID → Identificador  | UC → Caso de Uso| RF → Requisito Funcional|
| ---- | ---- | ---- |

## Personas

1. → Dr. Pedro Costa (Médico Regulador)

    * Idade: 52 anos
    * Experiência: 28 anos na área médica, com especialização em medicina de emergência
    * Objetivos: Garantir a eficiência e segurança nas transferências de pacientes, coordenar com diferentes unidades hospitalares e equipes de transporte
    * Desafios: Lidar com a falta de prática em transferências, assegurar a comunicação entre todas as partes envolvidas, e gerenciar transferências em situações de alta pressão

2. → Dr. Lúcia Santos (Médica de Origem)
    * Idade: 45 anos
    * Experiência: 20 anos na área médica, com especialização em clínica médica
    * Objetivos: Preparar e estabilizar pacientes para transferências, garantir que toda a documentação e informações estejam corretas e completas
    * Desafios: Coordenar a logística de transferências, assegurar que os pacientes sejam transferidos com segurança e que todas as necessidades médicas sejam atendidas

3. → Dr. Augusto Oliveira (Médico de Destino)
    * Idade: 60 anos
    * Experiência: 33 anos na área médica, com especialização em cirurgia e administração hospitalar
    * Objetivos: Receber pacientes transferidos e garantir que sejam atendidos prontamente, coordenar com a equipe médica para preparar os recursos necessários para a chegada dos pacientes
    * Desafios: Integrar sistemas de saúde para facilitar transferências, garantir que todas as informações do paciente sejam recebidas corretamente e de forma completa

4. → Mariana Rodrigues(Parente do Paciente)
    * Idade: 35 anos
    * Profissão: Professora
    * Objetivos: Receber informações e atualizações sobre o estado e localização do filho durante a transferência, assegurar que seu filho esteja sendo bem cuidado durante o processo
    * Desafios: Lidar com a ansiedade e a falta de informações durante a transferência, comunicar-se efetivamente com a equipe médica para obter atualizações


## Cenários 

#### Cenário 1: Coordenação de Transferências
   * Atores Envolvidos: Dr. Pedro Costa, Dr. Lúcia Santos, Dr. Augusto Oliveira
   * Contexto: O paciente João Silva sofreu um infarto e precisa ser transferido imediatamente do Hospital A para o Hospital B, que possui uma UTI cardiológica disponível.
   * Ações:
        * Dr. Lúcia solicita a transferência urgente no software.
        * Dr. Pedro revisa e aprova a solicitação, seleciona o transporte adequado, e define a unidade de destino.
        * Dr. Pedro cadastra o horário de saída e recebe a estimativa do horário de chegada.
        * Dr. Lúcia prepara o paciente para a transferência.
        * João Silva é transferido com segurança para o Hospital B, onde Dr. Augusto está preparado para recebê-lo.

#### Cenário 2: Logística de Transferência 
* Atores Envolvidos: Dr. Lúcia Santos, Dr. Pedro Oliveira, Dr. Augusto Almeida
* Contexto: A paciente Mariana Rodrigues precisa de uma cirurgia ortopédica eletiva e será transferida na próxima semana para outro hospital.
* Ações:
    * Dr. Lúcia agenda a transferência no software, especificando os detalhes necessários.
    * Dr. Pedro revisa a solicitação, seleciona o transporte e a unidade de destino.
    * Dr. Pedro cadastra o horário de saída e a estimativa de chegada.
    * Dr. Lúcia prepara a paciente e organiza a logística da transferência.
    Mariana Rodrigues é transferida com sucesso para o hospital de destino, onde Dr. Augusto a aguarda para a cirurgia.

#### Cenário 3: Integração no Sistema de Saúde
* Atores Envolvidos: Dr. Augusto Almeida, Luís Torres
* Contexto: O hospital de Dr. Augusto está integrando o novo software de transferência com o sistema de saúde existente.
* Ações:
    * Dr. Augusto e 	Luís configuram a integração do software.
    * Luís configura APIs e protocolos de segurança.
    * Dr. Augusto e Luís realizam testes para garantir a sincronização correta dos dados.
    * Resolução de problemas de compatibilidade.
    * Sistema é integrado com sucesso, permitindo a sincronização em tempo real dos dados dos pacientes.

#### Cenário 4: Comunicação 
* Atores Envolvidos: Mariana Rodrigues, Dr. Pedro Oliveira
* Contexto: O filho de Mariana está sendo transferido para outro hospital e ela deseja receber atualizações sobre o status da transferência.
* Ações:
    * Mariana fornece suas informações de contato para receber atualizações.
    * Dr. Pedro registra as informações de contato no sistema.
    * O sistema envia notificações automáticas a Mariana durante a transferência.
    * Mariana recebe atualizações sobre o status e a localização do filho em tempo real.
    * Mariana é mantida informada, reduzindo sua ansiedade e melhorando a comunicação com a equipe médica.
