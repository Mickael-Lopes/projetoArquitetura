# Casos de Uso Detalhado #

## Gerenciar paciente ##

Objetivo: Permitir que o ator cadastre, visualize, edite e inative os dados cadastrais de um paciente no sistema;

Ator primário: Secretária/Assistente e Psicologa;

Pré-Condição: Ator deve estar autenticado no sistema (CU06) e ter permissão de acesso ao módulo de pacientes;

Pós-Condição: Um novo paciente é registrado ou os dados de um paciente existente são atualizados na base de dados, em conformidade com a LGPD;

## Gerenciar agenda ##

Objetivo: Permite que o ator consiga agendar, reagendar e cancelar consultas no sistema

Ator primário: Secretária/Assistente e Psicologa;

Pré-Condição: O paciente deve estar cadastrado no sistema;

Pós-Condição: Consulta registrada na agenda;

## Gerenciar prontuário ##

Objetivo: O ator registra a consulta com o paciente, acompanha a evolução e consegue fazer atualizações conrfome necessário;

Ator principal: Psicóloga;

Pré-condição: Paciente devidamente cadastrado e psicóloga autenticada;

Pós-condição: Prontuário atualizado com segurança;

## Autenticação e controle de acesso ##

Objetivo: O sistema deve ser seguro e permitir um acesso limpo e sem dificuldades;

Ator primário: todos os usuários;

Pré-condição: Conta de usuário criada;

Pós-condição: Acesso permitido conforme as permissões do usuário;

## Enviar lembretes/avisos ##

Objetivo: Notificar pacientes sobre consultas agendadas e/ou pagamentos;

Ator primário: Sistema (automático);

Pré-condição: Consulta agendada e paciente com telefone de contato válido;

Pós-condição:Paciente notificado;

## Gerenciar pagamentos ##

Objetivo: Registrar status e valores de pagamento;

Ator primário: Secretária/Assistente e Psicologa;

Pré-condição: Consulta realizada e registrada;

Pós-condição: Pagamento atualizado e registrado;