# Ficha de Requisitos — Aula 02

## Análise e Projeto de Sistemas

**Unidade:** II — Introdução à Análise e Projeto de Sistemas
**Atividade:** Transformação do levantamento do sistema em requisitos funcionais e não funcionais
**Sistema:** Sistema de Gerenciamento de Academia
**Versão:** 1.0

---

# 1. Identificação do Sistema

| Campo                             | Preenchimento                                                                     |
| --------------------------------- | --------------------------------------------------------------------------------- |
| **Nome do sistema**               | Sistema de Gerenciamento de Academia                                              |
| **Objetivo**                      | Gerenciar o cadastro de alunos, planos, aulas, reservas e pagamentos da academia. |
| **Público-alvo**                  | Alunos, professores, funcionários e administradores.                              |
| **Responsável pelo levantamento** | Grupo de estudantes                                                               |
| **Versão**                        | 1.0                                                                               |

---

# 2. Requisitos Funcionais

> Requisitos funcionais descrevem **funcionalidades ou serviços que o sistema deve oferecer**.

## RF01 — Cadastrar aluno

| Campo                      | Descrição                                                                                                                                                           |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF01                                                                                                                                                                |
| **Descrição**              | O sistema deve permitir que funcionários cadastrem novos alunos na academia.                                                                                        |
| **Prioridade**             | Alta                                                                                                                                                                |
| **Critérios de aceitação** | 1. Deve permitir informar nome, CPF, e-mail e telefone. 2. Deve impedir o cadastro sem nome e CPF. 3. Deve informar ao funcionário quando o cadastro for concluído. |
| **Exemplo**                | O funcionário informa os dados de um novo aluno e seleciona **Cadastrar**. O sistema valida as informações e registra o aluno.                                      |

---

## RF02 — Consultar planos

| Campo                      | Descrição                                                                                                                                                                  |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF02                                                                                                                                                                       |
| **Descrição**              | O sistema deve permitir consultar os planos disponíveis na academia.                                                                                                       |
| **Prioridade**             | Média                                                                                                                                                                      |
| **Critérios de aceitação** | 1. Deve apresentar os planos disponíveis. 2. Deve informar o nome, valor e período de cada plano. 3. Deve indicar quando um plano não estiver disponível para contratação. |
| **Exemplo**                | O aluno acessa a área de planos e consulta as opções disponíveis, verificando o valor e a duração de cada plano.                                                           |

---

## RF03 — Reservar aula

| Campo                      | Descrição                                                                                                                                                                                                                                                               |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF03                                                                                                                                                                                                                                                                    |
| **Descrição**              | O sistema deve permitir que alunos realizem reservas em aulas disponíveis.                                                                                                                                                                                              |
| **Prioridade**             | Alta                                                                                                                                                                                                                                                                    |
| **Critérios de aceitação** | 1. Deve verificar se o aluno está cadastrado. 2. Deve verificar se o aluno possui um plano ativo. 3. Deve verificar se existem vagas disponíveis. 4. Deve registrar a reserva após a confirmação. 5. Deve informar ao aluno quando a reserva for realizada com sucesso. |
| **Exemplo**                | O aluno acessa a lista de aulas, seleciona uma aula de musculação funcional às 18h e confirma a reserva. O sistema verifica a disponibilidade e registra o agendamento.                                                                                                 |

---

## RF04 — Cancelar reserva

| Campo                      | Descrição                                                                                                                                                                                                             |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF04                                                                                                                                                                                                                  |
| **Descrição**              | O sistema deve permitir que o aluno cancele uma reserva de aula realizada anteriormente.                                                                                                                              |
| **Prioridade**             | Alta                                                                                                                                                                                                                  |
| **Critérios de aceitação** | 1. Deve apresentar as reservas realizadas pelo aluno. 2. Deve permitir selecionar uma reserva para cancelamento. 3. Deve solicitar a confirmação do cancelamento. 4. Deve liberar a vaga da aula após o cancelamento. |
| **Exemplo**                | O aluno acessa suas reservas, seleciona uma aula para a qual não poderá comparecer e confirma o cancelamento. O sistema cancela a reserva e libera a vaga.                                                            |

---

## RF05 — Cadastrar e editar aulas

| Campo                      | Descrição                                                                                                                                                                                                                                                       |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF05                                                                                                                                                                                                                                                            |
| **Descrição**              | O sistema deve permitir que funcionários cadastrem e editem as aulas oferecidas pela academia.                                                                                                                                                                  |
| **Prioridade**             | Alta                                                                                                                                                                                                                                                            |
| **Critérios de aceitação** | 1. Deve permitir informar nome da aula, professor, data, horário e quantidade de vagas. 2. Deve impedir o cadastro sem as informações obrigatórias. 3. Deve permitir alterar os dados de uma aula cadastrada. 4. Deve informar quando a operação for concluída. |
| **Exemplo**                | O funcionário cadastra uma aula de musculação funcional para segunda-feira às 18h, define o professor responsável e informa o limite de 20 alunos.                                                                                                              |

---

## RF06 — Cadastrar e editar planos

| Campo                      | Descrição                                                                                                                                                                                                                |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Identificação**          | RF06                                                                                                                                                                                                                     |
| **Descrição**              | O sistema deve permitir que funcionários cadastrem e editem os planos oferecidos pela academia.                                                                                                                          |
| **Prioridade**             | Média                                                                                                                                                                                                                    |
| **Critérios de aceitação** | 1. Deve permitir informar nome, valor e duração do plano. 2. Deve impedir o cadastro sem nome e valor. 3. Deve permitir editar os dados de um plano existente. 4. Deve apresentar confirmação após o cadastro ou edição. |
| **Exemplo**                | O funcionário cadastra o plano **Mensal**, define o valor e a duração de 30 dias. Posteriormente, poderá alterar o valor do plano.                                                                                       |

---

## RF07 — Consultar pagamentos

| Campo                      | Descrição                                                                                                                                                                                                                                        |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Identificação**          | RF07                                                                                                                                                                                                                                             |
| **Descrição**              | O sistema deve permitir consultar a situação dos pagamentos dos alunos.                                                                                                                                                                          |
| **Prioridade**             | Alta                                                                                                                                                                                                                                             |
| **Critérios de aceitação** | 1. Deve permitir consultar os pagamentos vinculados ao aluno. 2. Deve informar pagamentos realizados e pendentes. 3. Deve indicar quando houver pagamento em atraso. 4. Funcionários autorizados devem poder consultar os pagamentos dos alunos. |
| **Exemplo**                | O funcionário consulta o cadastro de um aluno e verifica que a mensalidade do mês atual está pendente.                                                                                                                                           |

---

## RF08 — Consultar dados e reservas

| Campo                      | Descrição                                                                                                                                                                                 |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF08                                                                                                                                                                                      |
| **Descrição**              | O sistema deve permitir que o aluno consulte seus dados cadastrais e suas reservas de aulas.                                                                                              |
| **Prioridade**             | Média                                                                                                                                                                                     |
| **Critérios de aceitação** | 1. O aluno deve visualizar seus dados cadastrados. 2. Deve apresentar as reservas atuais e futuras. 3. Deve permitir visualizar informações como nome da aula, professor, data e horário. |
| **Exemplo**                | O aluno acessa seu perfil e consulta seus dados e a lista de aulas que possui reservadas para a semana.                                                                                   |

---

# 3. Requisitos Não Funcionais

> Requisitos não funcionais descrevem **características, restrições e condições de qualidade** que o sistema deve atender.

## RNF01 — Segurança

| Campo                      | Descrição                                                                                                                                                                                                                                                        |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RNF01                                                                                                                                                                                                                                                            |
| **Descrição**              | O sistema deve controlar o acesso às funcionalidades de acordo com o perfil do usuário.                                                                                                                                                                          |
| **Prioridade**             | Alta                                                                                                                                                                                                                                                             |
| **Critérios de aceitação** | 1. Os usuários devem realizar autenticação antes de acessar funções restritas. 2. Funcionalidades administrativas devem estar disponíveis somente para funcionários e administradores autorizados. 3. O aluno não deve conseguir acessar dados de outros alunos. |
| **Exemplo**                | Um aluno acessa o sistema, mas não consegue acessar a tela de cadastro e edição de planos, que é restrita aos funcionários autorizados.                                                                                                                          |

---

## RNF02 — Desempenho

| Campo                      | Descrição                                                                                           |
| -------------------------- | --------------------------------------------------------------------------------------------------- |
| **Identificação**          | RNF02                                                                                               |
| **Descrição**              | O sistema deve apresentar respostas em tempo adequado durante o uso normal.                         |
| **Prioridade**             | Média                                                                                               |
| **Critérios de aceitação** | Em condições normais de operação, consultas simples devem apresentar o resultado em até 3 segundos. |
| **Exemplo**                | Ao consultar as aulas disponíveis, o sistema deve apresentar os resultados em até 3 segundos.       |

---

## RNF03 — Usabilidade

| Campo                      | Descrição                                                                                                                                                                                                                  |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RNF03                                                                                                                                                                                                                      |
| **Descrição**              | A interface deve apresentar informações e comandos de forma clara, simples e consistente.                                                                                                                                  |
| **Prioridade**             | Alta                                                                                                                                                                                                                       |
| **Critérios de aceitação** | 1. Os campos devem possuir rótulos claros. 2. As mensagens de erro devem orientar o usuário. 3. As principais ações devem ser facilmente identificáveis. 4. O processo de reserva de aula deve ser simples de compreender. |
| **Exemplo**                | Ao tentar reservar uma aula lotada, o sistema apresenta uma mensagem informando que não existem vagas disponíveis.                                                                                                         |

---

## RNF04 — Disponibilidade

| Campo                      | Descrição                                                                                                                                                                                 |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RNF04                                                                                                                                                                                     |
| **Descrição**              | O sistema deve estar disponível durante o horário de funcionamento da academia.                                                                                                           |
| **Prioridade**             | Alta                                                                                                                                                                                      |
| **Critérios de aceitação** | 1. O sistema deve permanecer acessível durante o horário de funcionamento da academia. 2. Manutenções programadas devem ser realizadas previamente e comunicadas aos usuários.            |
| **Exemplo**                | Durante o horário de funcionamento, alunos e funcionários conseguem acessar o sistema para realizar reservas e consultar informações, exceto durante manutenções previamente programadas. |

---

# 4. Modelo para preenchimento pelos estudantes

## Requisito Funcional

| Campo                      | Resposta do grupo                                                                                                                                                   |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RF01                                                                                                                                                                |
| **Descrição**              | O sistema deve permitir que funcionários cadastrem novos alunos na academia.                                                                                        |
| **Prioridade**             | Alta                                                                                                                                                                |
| **Critérios de aceitação** | 1. Deve permitir informar nome, CPF, e-mail e telefone. 2. Deve impedir o cadastro sem nome e CPF. 3. Deve informar ao funcionário quando o cadastro for concluído. |
| **Exemplo**                | O funcionário informa os dados de um novo aluno e seleciona **Cadastrar**. O sistema valida as informações e registra o aluno.                                      |

## Requisito Não Funcional

| Campo                      | Resposta do grupo                                                                                                                                                                                                                                                |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Identificação**          | RNF01                                                                                                                                                                                                                                                            |
| **Descrição**              | O sistema deve controlar o acesso às funcionalidades de acordo com o perfil do usuário.                                                                                                                                                                          |
| **Prioridade**             | Alta                                                                                                                                                                                                                                                             |
| **Critérios de aceitação** | 1. Os usuários devem realizar autenticação antes de acessar funções restritas. 2. Funcionalidades administrativas devem estar disponíveis somente para funcionários e administradores autorizados. 3. O aluno não deve conseguir acessar dados de outros alunos. |
| **Exemplo**                | Um aluno acessa o sistema, mas não consegue acessar a tela de cadastro e edição de planos, que é restrita aos funcionários autorizados.                                                                                                                          |

---

# 5. Orientações para elaboração

Para cada requisito, o grupo deve verificar:

* **Identificação:** possui código único?
* **Descrição:** está claro o que o sistema deve fazer ou qual característica deve apresentar?
* **Prioridade:** é essencial, importante ou pode ser implementado posteriormente?
* **Critérios de aceitação:** é possível verificar objetivamente se o requisito foi atendido?
* **Exemplo:** existe uma situação concreta que demonstra o requisito?

## Regra prática

Um bom requisito deve ser:

**Claro + específico + verificável + relevante**

---

# 6. Integrantes do grupo

* Pedro Henrique Silva Monteiro
* Pedro Borges Prudente Machado
* Yago Alves de Carvalho
* Robson Otávio Queiroz Castro
* Igor Jesus da Silva Tolentino
* Luiz Daniel da Costa Bastos

---

# 7. Entregável da atividade

O grupo desenvolveu a especificação dos requisitos para um **Sistema de Gerenciamento de Academia**, contemplando:

* Identificação do sistema;
* 8 requisitos funcionais;
* 4 requisitos não funcionais;
* Prioridade de cada requisito;
* Critérios de aceitação;
* Exemplos de utilização;
* Identificação dos integrantes do grupo.

## Próxima etapa

Os requisitos produzidos nesta ficha servirão como base para a identificação e especificação dos **casos de uso** do Sistema de Gerenciamento de Academia.
