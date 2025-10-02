## Lista de Requisitos – Geral

Esta lista combina os requisitos do escopo, da análise do sistema análogo e das necessidades de negócio, divididos em Funcionais e Não Funcionais.

# Requisitos Funcionais (RF)

●	RF01 - Gerenciar Pacientes:
○	O sistema deve permitir cadastrar, visualizar, editar e inativar pacientes.
○	Os dados cadastrais devem incluir nome completo, CPF, data de nascimento, contato (telefone, e-mail) e endereço.
○	O sistema deve solicitar e registrar o consentimento do paciente para o tratamento de seus dados (LGPD).

●	RF02 - Gerenciar Agenda:
○	O sistema deve exibir a agenda do psicólogo em formato diário, semanal e mensal.
○	O sistema deve permitir agendar, reagendar e cancelar consultas, associando-as a um paciente.
○	O sistema deve permitir bloquear horários para compromissos pessoais.

●	RF03 - Gerenciar Prontuário Eletrônico:
○	O sistema deve permitir que o psicólogo crie e edite registros de evolução para cada sessão de um paciente.
○	Os registros devem ser datados e ter acesso restrito ao psicólogo responsável.

●	RF04 - Gerenciar Pagamentos:
○	O sistema deve permitir registrar o status de pagamento de cada sessão (ex: Pendente, Pago, Cancelado).
○	O sistema deve permitir a geração de recibos simples.

●	RF05 - Enviar Lembretes e Avisos:
○	O sistema deve enviar lembretes de consulta automaticamente 24 horas antes da sessão.
○	O sistema deve enviar avisos de pagamentos pendentes.

●	RF06 - Autenticação e Controle de Acesso:
○	O sistema deve exigir autenticação (login e senha) para acesso.
○	O sistema deve suportar diferentes perfis de usuário (ex: Administrador/Psicólogo, Secretário(a)) com permissões distintas.
Requisitos Não Funcionais (RNF)

●	RNF01 - Segurança: O sistema deve criptografar dados sensíveis em repouso (banco de dados) e em trânsito (HTTPS). O acesso aos prontuários deve ser restrito e auditável.

●	RNF02 - Usabilidade: A interface deve ser limpa, intuitiva e fácil de usar, minimizando a curva de aprendizado.

●	RNF03 - Desempenho: As páginas principais (agenda, lista de pacientes) devem carregar em menos de 3 segundos.

●	RNF04 - Disponibilidade: O sistema deve estar disponível 99.5% do tempo.

●	RNF05 - Responsividade: O sistema deve ser acessível e funcional em navegadores de desktops, tablets e smartphones.

●	RNF06 - Conformidade: O sistema deve seguir todas as diretrizes da Lei Geral de Proteção de Dados (LGPD) no tratamento de dados pessoais.

