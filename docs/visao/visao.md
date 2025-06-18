# Documento de visão

### Histórico da Revisão 

|  Data  | Versão | Descrição | Autores |
|:-------|:-------|:----------|:------|
| 17/06/2025 |  **`1.00`** | Versão Inicial  | Marcos Alexandre, João Roberto, Lucas Tales |

### 1. Projeto: **`Sistema de Agendamento CNAT MAKER`**

### 2. Descrição do problema 
| Item | Descrição |
|:------------------|:-----|
| **_O problema_** | A ausência de um sistema dedicado para gerenciar os serviços do laboratório e facilitar as solicitações por parte dos usuários.|
| **_afetando_** | Pessoas que necessitam dos serviços oferecidos pelo laboratório, como bolsistas e voluntários responsáveis pelo gerenciamento dessas demandas.|
| **_cujo impacto é_**| Dificuldade tanto na solicitação quanto no controle dos serviços, gerando dificuldades na prestação dos atendimentos. |
| **_Uma boa solução seria_** | Uma plataforma que centralize e simplifique o processo de solicitação e gestão dos serviços prestados pelo laboratório.|

### 3. Descrição dos usuários
| Item | Descrição |
|:------------------|:-----|
| **_Publico_** | Pessoas que desejam solicitar os serviços oferecidos pelo laboratório, como estudantes, professores ou membros da comunidade. |
| **_Bolsista/Voluntario_** | Colaboradores responsáveis por gerenciar os processos relacionados à prestação dos serviços, incluindo o controle das solicitações e o acompanhamento das demandas. |

**Ambiente de trabalho**
| Item | Descrição |
|:------------------|:-----|
| **_Publico_** | Poderá acessar o sistema a partir de qualquer dispositivo com conexão à internet, por meio de um navegador web compatível. |
| **_Bolsista/Voluntario_** | Também poderão acessar o sistema remotamente, utilizando qualquer dispositivo conectado à internet, por meio de um navegador web. |

**Responsabilidade**
| Item | Descrição |
|:------------------|:-----|
| **_Bolsista/Voluntario_** |  São responsáveis por atender às solicitações geradas pelo público, bem como por gerenciar os processos necessários para a execução e finalização dos serviços. |
| **_Publico_** | Deve preencher corretamente os dados ao criar uma solicitação de serviço, além de acompanhar o andamento e negociar eventuais ajustes até a conclusão do atendimento.  |

### 4. Descrição do ambiente dos usuários
A plataforma em questão é uma aplicação web que conecta dois perfis de usuários: o Público, que possui uma demanda específica, e o Bolsista, que oferece serviços por meio do laboratório. Todas as interações no sistema, como o cadastro de demandas e o envio de propostas, são realizadas diretamente pelos próprios usuários.

Considerando essa dinâmica, é fundamental que a plataforma esteja disponível de forma contínua, permitindo a realização de postagens e o envio de propostas a qualquer momento. Portanto, o sistema deve ser capaz de operar ininterruptamente, 24 horas por dia, 7 dias por semana, incluindo feriados, garantindo alta disponibilidade e acessibilidade para todos os usuários.

**_A interação com o sistema pode ter diversas variações devido a localidade e sinal de internet do usuário, fato que pode restringir a navegação e o acesso ao sistema._**

### 5. Principais necessidades dos usuários
**Necessidades do Público (Solicitante)**
As pessoas interessadas em contratar um serviço do laboratório frequentemente enfrentam obstáculos para formalizar suas solicitações. Muitas vezes, não há um canal claro ou estruturado para encaminhar demandas, o que gera insegurança e retrabalho.
Além disso, há uma falta de clareza quanto à disponibilidade de materiais e insumos que o laboratório possui, o que dificulta o planejamento por parte do solicitante e pode gerar expectativas desalinhadas. Outro ponto importante é a necessidade de compreender o que pode ser oferecido ao laboratório como contrapartida pelo serviço — seja em forma de materiais, dados, colaboração ou outra forma de retribuição acordada.
O solicitante também busca acompanhamento contínuo do andamento do pedido, incluindo prazos estimados, etapas já realizadas e eventuais pendências. A transparência no processo é fundamental para manter a confiança e garantir que o serviço atenda às suas expectativas.

**Necessidades do Bolsista (Executor)**
Do lado do bolsista responsável por executar e despachar os pedidos, existem dificuldades operacionais e de comunicação que impactam diretamente a eficiência do processo. Entre os principais desafios estão: listar de forma organizada os serviços solicitados, manter atualizações regulares sobre o progresso do trabalho e esclarecer de maneira objetiva quais materiais serão utilizados e o que é esperado do solicitante como contrapartida. 
A ausência de uma ferramenta centralizada para registrar e acompanhar essas informações pode levar à perda de dados, atrasos na entrega dos serviços e falhas na comunicação entre as partes. Assim, há uma necessidade evidente de um sistema que possibilite ao bolsista gerenciar facilmente as demandas, registrar o andamento das etapas e informar, com clareza, os requisitos e recursos necessários para a execução do serviço.

### 6.	Alternativas concorrentes
Devido à natureza específica da plataforma — voltada para a gestão de solicitações e execução de serviços em um contexto laboratorial envolvendo bolsistas e o público interessado —, **não há atualmente soluções concorrentes diretas** que atendam a esse mesmo conjunto de necessidades de forma integrada. 

### 7.	Visão geral do produto
O Sistema CNATMAKER é a nova plataforma digital a ser desenvolvida para o laboratório CNATMAKER. Seu objetivo é oferecer um ambiente acessível via navegadores web modernos, com uma interface intuitiva, de fácil uso e com boa usabilidade, visando reduzir o tempo de execução das tarefas e facilitar a experiência dos usuários.

A plataforma se propõe a servir como um elo entre dois perfis de usuários: o Público, que busca solicitar serviços oferecidos pelo laboratório, e os Bolsistas, que são responsáveis pela organização, acompanhamento e execução dessas demandas.

O sistema irá atuar como um facilitador no processo de solicitação, execução e monitoramento dos serviços prestados, proporcionando comunicação ágil, objetiva e centralizada entre as partes envolvidas. Além disso, pretende oferecer recursos que tragam mais transparência, rastreabilidade e controle sobre o andamento das solicitações, beneficiando tanto os solicitantes quanto os bolsistas responsáveis.

### 8. Requisitos Funcionais
| Código | Nome                                | Descrição                                                                                                  |
| :----: | :---------------------------------- | :--------------------------------------------------------------------------------------------------------- |
|  RF001 | Autenticação                        | Permitir que o usuário faça login na plataforma para acessar funcionalidades conforme seu perfil.          |
|  RF002 | Gerenciar solicitações de serviço   | Permitir o cadastro, visualização, edição e exclusão de solicitações de serviços feitas pelo público.      |
|  RF003 | Gerenciar solicitações de visita    | Permitir o cadastro, visualização, edição e exclusão de solicitações de visitas feitas pelo público.       |
|  RF004 | Fazer solicitação serviço   | Permitir o cadastro de uma solicitação de serviço.      |
|  RF005 | Fazer solicitações de visita    | Permitir o cadastro de uma solicitação de visita.       |
|  RF006 | Gerenciar andamento de solicitações | Permitir que os bolsistas atualizem e acompanhem o status e o progresso de cada solicitação.               |
|  RF007 | Gerenciar perfíl                  | Permitir a edição de dados cadastrais, exclusão e controle de permissões dos usuários conforme seu perfil. |
| RF008  | Gerenciar material    | Permitir ao bolsista o cadastro, atualização e exclusão de materiais utilizados nos apoios.|


### 9. Requisitos não-funcionais
| Cod. | Nome | Descrição | Categoria | Classificação |
| :---: | :---: | :--- | :---: | :---: |
| RNF01 | Autorizações | Somente usuários logados poderão acessar os recursos da plataforma. | Segurança | Obrigatório |
| RNF02 | Ferramentas | O sistema deve ser desenvolvido utilizando o banco de dados MySql e a linguagem python por meio do framework django. | Implementação | Preferível |
| RNF03 | Tempo de resposta | O tempo de resposta do sistema não deve ultrapassar 5 segundos. | Performance | Obrigatório |
| RNF04 | Ambiente de execução | O sistema deve ser executado na web através de um navegador. | Interoperabilidade | Obrigatório |
