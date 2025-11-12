# Modelo C4 #

## Visão C1: Contexto ##

**Descrição geral**: O *Sistema da Clínica de Psicologia* é uma aplicação web que permite gerenciar pacienttes, consultas, prontuários e pagamentos, automatizando processos administrativos e clínicos. Ele interage com diferentes tipos de usuários e serviços externos, garantindo segurança e conformidade com a LGPD.

**Sistema principal**: Sistema de Clínica de Psicologia

**Atores externos**

*Psicóloga:* Cadastra pacientes, acessa protuários, gerencia consultas e pagamentos.

*Secretária:* Agenda consultas, cadastra pacientes, confirma pagamentos, atualiza cadastros e envia comunicados.

*Paciente:* Recebe notificações da clínica, confirma consultas, realiza pagamento e acessa prontuário.

**Fluxo de interação**

1. A secretária, Psicóloga e o Paciente acessam o sistema via navegador.
2. O psicólogo consulta e atualiza dados dos pacientes e prontuários.
3. O sistema envia lembretes e confirmações para pacientes via serviços de mensagens.
4. A secretária verifica e atualiza pagamentos pendentes.
----------------------------------------------------------------------------------
## Visão C2: Containers

A visão C2 representa a arquitetura de containers do sistema, mostrando os principais componentes de software, bancos de dados e serviços externos que interagem entre si.


### **Descrição Geral**

O **Sistema da Clínica de Psicologia** é composto por diversos containers que trabalham em conjunto para gerenciar pacientes, consultas, prontuários e pagamentos.
Cada container tem responsabilidades bem definidas e comunica-se via **API REST**.


### **Containers Principais**

| Container                   | Tipo                              | Responsabilidade                                                                                         |
| --------------------------- | --------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Frontend Web**            | Aplicação Web (Angular) | Interface gráfica para psicólogos, secretárias e pacientes. Exibe agendamentos, cadastros e prontuários. |
| **Backend API**             | Servidor (C# .NET Core) | Processa regras de negócio, autenticação, controle de acesso e comunicação com serviços externos.        |
| **Banco de Dados**          | PostgreSQL                | Armazena informações de pacientes, consultas, pagamentos e prontuários.                                  |
| **Serviço de Notificações** | Microserviço / API externa        | Envia lembretes automáticos e confirmações por WhatsApp e e-mail.                                        |
| **Serviço de Autenticação** | Módulo interno          | Garante login seguro e controle de permissões (Psicólogo, Secretária, Administrador).                    |
| **Google Calendar API**     | Serviço Externo                   | Sincroniza os compromissos e horários do psicólogo.                                                      |
| **Armazenamento em Nuvem**  | Serviço Externo                   | Guarda backups e documentos anexados (opcional).                                                         |


### **Fluxo de Comunicação**

1. O **usuário** acessa o **Frontend Web** via navegador.
2. O **Frontend** envia requisições HTTP para o **Backend API**.
3. O **Backend** valida o acesso com o **Serviço de Autenticação**.
4. Dados são gravados e lidos do **Banco de Dados**.
5. O **Serviço de Notificações** envia lembretes automáticos.
6. O **Backend** sincroniza os agendamentos com o **Google Calendar API**.
7. Backups e anexos são armazenados na **Nuvem**.


### **Resumo**

> O diagrama C2 mostra que o sistema é modular, seguro e escalável.
> A divisão em containers permite **facilidade de manutenção**, **integração com serviços externos** e **boa experiência para usuários da clínica**.