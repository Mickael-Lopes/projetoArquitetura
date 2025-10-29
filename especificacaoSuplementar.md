# 🧠 Especificação Suplementar do Sistema Psicoplanner

## 1. Introdução

### 1.1 Propósito

Este documento descreve os requisitos suplementares do **Sistema Psicoplanner**, complementando o documento de **Especificação de Objetivos e Requisitos (EOR)**.
Ele segue o modelo **IEEE 830/RUP**, detalhando aspectos técnicos, operacionais e de qualidade que não estão diretamente cobertos pelos casos de uso.

### 1.2 Escopo

O **Psicoplanner** é um sistema **web (SaaS)** voltado à gestão de consultórios psicológicos e clínicas, integrando funções de **agenda**, **prontuário eletrônico**, **controle financeiro**, **videochamadas** e **automação de notificações**.

### 1.3 Definições e Abreviações

* **EOR** – Especificação de Objetivos e Requisitos
* **LGPD** – Lei Geral de Proteção de Dados (Lei nº 13.709/2018)
* **CFP** – Conselho Federal de Psicologia
* **SaaS** – Software as a Service
* **UI** – Interface do Usuário

### 1.4 Referências

* EOR - Sistema Psicoplanner
* IEEE Std 830-1998 – *Recommended Practice for Software Requirements Specifications*
* LGPD – Lei nº 13.709/2018
* Resoluções do CFP sobre prontuário eletrônico e ética profissional

### 1.5 Visão Geral do Documento

Este documento aborda os **requisitos suplementares** que regem a **operação, segurança, desempenho, usabilidade e manutenção** do sistema Psicoplanner, estruturados em conformidade com o modelo **IEEE 830/RUP**.

## 2. Descrição Geral

### 2.1 Perspectiva do Produto

O **Psicoplanner** é um sistema **SaaS** hospedado em nuvem, acessível via navegador e dispositivos móveis, oferecendo uma **solução integrada de gestão** para psicólogos e clínicas.
Ele interage com serviços externos, como **Google Calendar** e **APIs de mensagens**.

### 2.2 Funções do Produto

* Agendamento de consultas e lembretes automáticos
* Prontuário eletrônico e registros clínicos
* Controle financeiro e relatórios
* Videochamadas integradas
* Gestão de múltiplos usuários e planos
* Suporte técnico e armazenamento em nuvem seguro

### 2.3 Características dos Usuários

O público-alvo inclui **psicólogos autônomos**, **clínicas de psicologia** e **assistentes administrativos**.
O sistema deve atender usuários com **conhecimentos básicos de informática** e oferecer **interface intuitiva e responsiva**.

### 2.4 Restrições Gerais

* O sistema deve operar em ambiente web seguro.
* Requer conexão estável à internet.
* Deve cumprir as normas do CFP e a LGPD.
* Deve funcionar em navegadores atualizados.

### 2.5 Suposições e Dependências

* O servidor de hospedagem deve garantir **disponibilidade 24/7**.
* As **APIs de terceiros** (WhatsApp, Google Calendar) devem permanecer operacionais.
* O usuário deve possuir **dispositivos compatíveis** (PC, tablet ou smartphone).

## 3. Requisitos Suplementares

### 3.1 Usabilidade

O sistema deve possuir **interface simples, responsiva e intuitiva**, com **cores neutras** e **estrutura ergonômica**.
Os textos devem ser claros e os ícones representativos.
O tempo de aprendizado para novos usuários **não deve ultrapassar 30 minutos**.

### 3.2 Confiabilidade

* Disponibilidade mínima de **99% mensal**.
* **Falhas críticas** devem ser recuperadas em até **2 horas**.
* **Backups automáticos diários** devem assegurar a integridade das informações clínicas e administrativas.

### 3.3 Desempenho

* **Tempo máximo de resposta:** 3 segundos por transação.
* **Suporte mínimo:** 1.000 usuários simultâneos.
* **Tolerância:** até 5% de lentidão em horários de pico.
* **Operação eficiente** com conexão mínima de 1 Mbps.

### 3.4 Suporte e Manutenibilidade

* Atualizações devem ocorrer **sem interrupção de serviço**, utilizando **deploy contínuo**.
* **Suporte técnico** disponível em horário comercial via chat ou e-mail.
* Toda alteração deve ser **documentada em logs de versão**.

### 3.5 Segurança

* Autenticação obrigatória com **credenciais individuais**.
* **Criptografia AES-256** para dados sensíveis.
* **Controle de acesso** baseado em perfis de usuário.
* **Logs** de todas as ações críticas.
* Conformidade com a **LGPD** e políticas de sigilo do **CFP**.

### 3.6 Compatibilidade e Portabilidade

* Compatível com **Chrome**, **Firefox**, **Edge** e **Safari**.
* Compatível com **Windows**, **macOS**, **Android** e **iOS**.
* Deve permitir **migração de dados** e integração com **APIs RESTful externas**.

### 3.7 Padrões e Requisitos Legais

O **Psicoplanner** deve seguir as **normas do CFP** relacionadas à **segurança e confidencialidade de dados psicológicos**.
Todos os dados pessoais devem ser tratados conforme a **LGPD**, com **consentimento informado dos pacientes**.

### 3.8 Restrições de Design e Implementação

* Utilizar **arquitetura em camadas** (front-end, back-end e banco de dados).
* **Front-end:** React, HTML5, CSS3, JavaScript.
* **Back-end:** API REST com banco de dados relacional.

## 4. Apêndice

Este documento complementa o **EOR do Sistema Psicoplanner** e deve ser utilizado como **referência técnica** durante o **desenvolvimento e manutenção** do sistema.