# 🧠 Especificação de Objetivos e Requisitos

**EOR – Sistema Psicoplanner**
**Versão 1.0**

## 1. Introdução

Este documento apresenta a **Especificação de Objetivos e Requisitos (EOR)** do sistema **Psicoplanner**, um software destinado à **gestão de consultórios psicológicos e clínicas de psicoterapia**.
O objetivo é registrar e organizar os **requisitos funcionais e não funcionais**, bem como os **objetivos e benefícios esperados** com a utilização do sistema.

### 1.1 Objetivos

Definir os **objetivos e requisitos** que orientarão o **desenvolvimento, manutenção e evolução** do sistema Psicoplanner, garantindo que as funcionalidades estejam **alinhadas às necessidades dos profissionais da psicologia**.

### 1.2 Público-Alvo

Este documento é voltado a **desenvolvedores, analistas de sistemas, gerentes de projeto** e demais envolvidos no ciclo de vida do software, bem como a **psicólogos e gestores** interessados em compreender suas capacidades.

### 1.3 Organização do Documento

O documento segue a estrutura tradicional de uma **Especificação de Objetivos e Requisitos**, contendo seções de introdução, **descrição do problema**, **casos de uso**, **requisitos funcionais e não funcionais**, **requisitos futuros** e **referências**.


## 2. Descrição do Problema e do Sistema

### 2.1 Identificação e Missão do Sistema

O **Psicoplanner** é um **sistema online de gestão** voltado a psicólogos, criado com a missão de **organizar, automatizar e integrar processos clínicos e administrativos**, oferecendo **maior eficiência e segurança** nas rotinas de atendimento.

### 2.2 Domínio do Problema e Contexto de Aplicação

O domínio do problema abrange a **dificuldade de gestão de pacientes, finanças e documentos clínicos** em consultórios psicológicos.
O sistema atua como uma **solução digital integrada** para **otimizar o trabalho** e **reduzir falhas humanas**.

### 2.3 Objetivos e Benefícios Esperados do Sistema

* Automatizar agendamentos e lembretes de consultas;
* Reduzir faltas e atrasos através de notificações automáticas;
* Centralizar prontuários e informações clínicas de forma segura;
* Facilitar a gestão financeira e geração de relatórios;
* Promover a conformidade com o CFP e a LGPD.

### 2.4 Características Essenciais do Sistema

O sistema deve:

* Ser acessível via navegador e dispositivos móveis;
* Possuir interface intuitiva e amigável;
* Garantir segurança e privacidade de dados;
* Permitir integrações com serviços externos;
* Oferecer suporte técnico contínuo.

### 2.5 Descrição dos Interessados do Sistema

| Interessado         | Função no Sistema                                              |
| ------------------- | -------------------------------------------------------------- |
| **Psicólogos**      | Gerenciam atendimentos, pacientes e finanças.                  |
| **Secretárias**     | Auxiliam na marcação de consultas e comunicação com pacientes. |
| **Pacientes**       | Recebem lembretes e acessam atendimentos online.               |
| **Suporte Técnico** | Responsável por manutenção e atendimento ao cliente.           |

### 2.6 Diagnóstico da Situação Atual

Atualmente, muitos profissionais ainda utilizam **métodos manuais** ou **ferramentas genéricas** que não atendem às necessidades específicas da psicologia.
O **Psicoplanner** substitui essas soluções fragmentadas por uma **plataforma completa e integrada**.

## 3. Casos de Uso

### 3.1 Atores

1. Psicólogo
2. Secretária
3. Paciente
4. Sistema de Pagamentos
5. Plataforma de Videochamada

### 3.2 Lista de Casos de Uso

| Código    | Caso de Uso                  | Atores                |
| --------- | ---------------------------- | --------------------- |
| **CSU01** | Agendar Consulta             | Psicólogo, Secretária |
| **CSU02** | Enviar Lembretes Automáticos | Sistema               |
| **CSU03** | Realizar Atendimento Online  | Psicólogo, Paciente   |
| **CSU04** | Registrar Pagamento          | Psicólogo             |
| **CSU05** | Gerar Relatórios             | Psicólogo             |


## 4. Requisitos e Restrições Funcionais (RFUN)

| Código   | Descrição                                               |
| -------- | ------------------------------------------------------- |
| **RF01** | Gerenciar agenda de atendimentos.                       |
| **RF02** | Enviar lembretes automáticos de consultas e pagamentos. |
| **RF03** | Realizar atendimentos online com segurança.             |
| **RF04** | Criar e armazenar prontuários eletrônicos.              |
| **RF05** | Controlar pagamentos e gerar relatórios financeiros.    |
| **RF06** | Sincronizar com calendários externos.                   |
| **RF07** | Notificar o usuário sobre o dia de trabalho.            |
| **RF08** | Permitir múltiplos usuários e perfis de acesso.         |
| **RF09** | Disponibilizar suporte técnico.                         |


## 5. Requisitos e Restrições Não Funcionais

| Código    | Descrição                                                          |
| --------- | ------------------------------------------------------------------ |
| **RNF01** | O sistema deve garantir sigilo e proteção de dados conforme LGPD.  |
| **RNF02** | Deve estar disponível 24h por dia.                                 |
| **RNF03** | A interface deve ser responsiva e intuitiva.                       |
| **RNF04** | O tempo de resposta não deve ultrapassar 3 segundos.               |
| **RNF05** | O sistema deve realizar backup automático diário.                  |
| **RNF06** | Deve permitir escalabilidade conforme o número de usuários cresce. |
| **RNF07** | Compatível com navegadores modernos.                               |
| **RNF08** | Deve registrar logs de operações.                                  |
| **RNF09** | Suporte à manutenção sem perda de dados.                           |


## 6. Requisitos Futuros (RFUT)

| Código     | Descrição                                        |
| ---------- | ------------------------------------------------ |
| **RFUT01** | Integração com emissão de nota fiscal.           |
| **RFUT02** | Módulo de feedback e satisfação dos pacientes.   |
| **RFUT03** | Relatórios personalizados de desempenho clínico. |


## 7. Referências Cruzadas Complementares

| Requisito Funcional | Caso de Uso Relacionado |
| ------------------- | ----------------------- |
| **RF01**            | CSU01                   |
| **RF02**            | CSU02                   |
| **RF03**            | CSU03                   |
| **RF04**            | CSU04                   |
| **RF05**            | CSU05                   |

## 8. Bibliografia

* [Site oficial Psicoplanner](https://www.psicoplanner.com.br)
* **Conselho Federal de Psicologia** – Resoluções sobre prontuário eletrônico.
* **Lei Geral de Proteção de Dados (LGPD)** – Lei nº 13.709/2018.
