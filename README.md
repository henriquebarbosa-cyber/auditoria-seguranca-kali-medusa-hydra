# 🔐 Auditoria de Segurança: Testes de Autenticação com Kali Linux, Medusa e Hydra

![Kali Linux](https://img.shields.io/badge/Kali_Linux-Security-blue)
![Medusa](https://img.shields.io/badge/Medusa-Auditoria-orange)
![Hydra](https://img.shields.io/badge/THC_Hydra-Authentication-red)
![VirtualBox](https://img.shields.io/badge/VirtualBox-Lab-blue)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

## 📌 Sobre o Projeto

Este projeto foi desenvolvido como parte do desafio prático da **Digital Innovation One (DIO)**, com o objetivo de estudar técnicas de auditoria de segurança e identificar vulnerabilidades relacionadas à autenticação de usuários.

A proposta consiste na utilização do Kali Linux em conjunto com ferramentas especializadas em testes de autenticação, como **Medusa** e **THC Hydra**, em ambientes virtuais vulneráveis e controlados.

Durante o desenvolvimento, foram explorados conceitos de ataques de força bruta, automação de tentativas de autenticação, password spraying e análise de mecanismos de proteção.

O projeto também aborda medidas de prevenção e mitigação, demonstrando a importância de políticas de segurança para proteger serviços, aplicações e credenciais.

## 🎯 Objetivos do Projeto

- Compreender o funcionamento dos ataques de força bruta.
- Conhecer e utilizar as ferramentas Medusa e THC Hydra.
- Estudar vulnerabilidades relacionadas à autenticação.
- Realizar simulações controladas em serviços FTP, SMB e aplicações Web.
- Compreender o conceito de password spraying.
- Analisar os riscos associados ao uso de senhas fracas.
- Identificar mecanismos de proteção contra tentativas automatizadas.
- Documentar os procedimentos, ferramentas e resultados.
- Propor medidas de mitigação para melhorar a segurança dos sistemas.

## 🛠️ Ferramentas e Tecnologias

| Ferramenta | Descrição |
|---|---|
| Kali Linux | Sistema operacional voltado para testes de segurança e pentest. |
| Medusa | Ferramenta utilizada para auditoria automatizada de autenticação. |
| THC Hydra | Ferramenta utilizada para testes de autenticação em diferentes serviços. |
| Metasploitable 2 | Máquina virtual intencionalmente vulnerável para estudos de segurança. |
| DVWA | Aplicação Web vulnerável utilizada para treinamento. |
| VirtualBox | Software de virtualização para criação do laboratório. |
| GitHub | Plataforma utilizada para documentação e compartilhamento do projeto. |

## 🖥️ Arquitetura do Laboratório

O ambiente de testes utiliza máquinas virtuais configuradas em uma rede isolada, permitindo executar atividades de auditoria sem comprometer sistemas externos.

### Máquinas virtuais

**Kali Linux**
- Sistema utilizado para executar as ferramentas de auditoria.
- Ambiente para análise e realização dos testes.

**Metasploitable 2**
- Máquina virtual intencionalmente vulnerável.
- Utilizada para estudar serviços de rede e vulnerabilidades.

**DVWA (Damn Vulnerable Web Application)**
- Aplicação Web vulnerável para fins educacionais.
- Utilizada para estudar falhas de autenticação e segurança de aplicações.

### Configuração de rede

- Virtualizador: Oracle VirtualBox.
- Tipo de rede: Host-Only.
- Comunicação restrita ao laboratório.
- Ambiente destinado exclusivamente a testes autorizados.

## 🔍 Cenários de Auditoria

### 1. Testes de autenticação em FTP

Estudo de vulnerabilidades relacionadas à autenticação no serviço FTP.

Foi utilizada a ferramenta Medusa para realizar testes controlados de autenticação com credenciais de laboratório.

**Objetivos:**
- Compreender o funcionamento de tentativas automatizadas.
- Identificar riscos relacionados a senhas fracas.
- Observar a resposta do serviço às tentativas de autenticação.
- Verificar o estabelecimento de conexão após a autenticação.

### 2. Testes em aplicação Web (DVWA)

Estudo de mecanismos de autenticação em aplicações Web por meio do ambiente DVWA.

Foi utilizada a ferramenta THC Hydra no cenário de teste.

**Objetivos:**
- Compreender os riscos de formulários de login vulneráveis.
- Estudar a automação de tentativas de autenticação.
- Analisar mecanismos de proteção contra ataques automatizados.
- Observar os resultados da autenticação no ambiente controlado.

### 3. Testes de autenticação em SMB

Estudo de autenticação no serviço SMB em ambiente controlado.

Foi utilizada a ferramenta Medusa para realizar testes de autenticação no serviço.

**Objetivos:**
- Compreender os riscos relacionados ao uso de senhas comuns.
- Observar o comportamento do serviço durante os testes.
- Verificar o estabelecimento de conexão com a máquina.
- Estudar a importância de políticas adequadas de autenticação.

## ⚙️ Ferramentas de Auditoria: Medusa e Hydra

### Medusa

A Medusa é uma ferramenta de código aberto utilizada em auditorias de autenticação.

Permite realizar testes automatizados em diferentes serviços, auxiliando na identificação de credenciais vulneráveis em ambientes autorizados.

### THC Hydra

A THC Hydra é uma ferramenta de auditoria de autenticação que permite testar diferentes protocolos e serviços.

É utilizada em avaliações de segurança para identificar riscos relacionados a credenciais fracas e mecanismos inadequados de autenticação.

### Comparativo entre as ferramentas

| Característica | Medusa | THC Hydra |
|---|---|---|
| Testes automatizados | Sim | Sim |
| Auditoria de autenticação | Sim | Sim |
| Suporte a múltiplos serviços | Sim | Sim |
| Uso em ambientes de laboratório | Sim | Sim |
| Finalidade educacional | Sim | Sim |

As duas ferramentas são importantes no contexto de auditoria de segurança e permitem compreender diferentes abordagens para avaliação de mecanismos de autenticação.

## 📸 Evidências do Laboratório

A seguir estão os registros das atividades realizadas durante os testes no ambiente controlado, demonstrando o uso das ferramentas Medusa e Hydra e as conexões com os serviços FTP e SMB.

### 1. Conexão FTP

![Conexão FTP](images/conex%C3%A7%C3%A3o-ftp.PNG)

Registro da conexão FTP estabelecida com a máquina de laboratório.

### 2. Aplicação DVWA

![Página de login DVWA](images/DVWA.PNG)

Acesso à página de login da aplicação vulnerável DVWA.

### 3. Teste com Hydra na DVWA

![Execução Hydra DVWA](images/hydra-dvwa.PNG)

Registro da execução do Hydra no ambiente DVWA, no qual foram identificadas as credenciais `admin` e `password`.

### 4. Testes com Medusa no FTP

![Medusa FTP](images/medusa-ftp.PNG)

Utilização da ferramenta Medusa para testar credenciais de acesso ao serviço FTP.

![Medusa FTP ataque](images/medusa-ftp-ataque.PNG)

Registro adicional da execução do teste com Medusa contra o serviço FTP.

### 5. Testes com Medusa no SMB

![Medusa SMB](images/medusa-smb.PNG)

Execução do Medusa para testar credenciais de acesso ao serviço SMB.

### 6. Conexão SMB

![Conexão SMB](images/smb-conexc%C3%A3o.PNG)

Registro da conexão estabelecida com a máquina por meio do serviço SMB.

**Observação:** Todos os testes foram realizados em ambiente de laboratório controlado, com finalidade educacional.

## 📊 Resultados e Análise

Durante a execução das atividades no laboratório, foram realizados testes de autenticação nos serviços FTP, SMB e na aplicação Web DVWA.

Os registros obtidos demonstram os seguintes resultados:

### FTP
- Utilização da ferramenta Medusa para testes de autenticação.
- Identificação de credenciais aceitas pelo serviço no ambiente de laboratório.
- Estabelecimento de conexão FTP após a autenticação.

### DVWA
- Acesso à página de autenticação da aplicação.
- Utilização da ferramenta THC Hydra no cenário de teste.
- Identificação das credenciais `admin` e `password` no ambiente utilizado.

### SMB
- Utilização da ferramenta Medusa para testes de autenticação.
- Registro das tentativas realizadas no serviço SMB.
- Estabelecimento de conexão com a máquina por meio do serviço SMB.

### Análise geral

As atividades demonstraram como credenciais fracas podem representar riscos à segurança dos serviços e aplicações.

Os testes também permitiram conhecer as funcionalidades das ferramentas Medusa e THC Hydra e compreender a importância de mecanismos de proteção, como políticas de senhas fortes, limitação de tentativas de autenticação e monitoramento de logs.

## 🛡️ Medidas de Mitigação e Prevenção

Para reduzir os riscos relacionados a ataques de força bruta e password spraying, são recomendadas as seguintes medidas:

### 1. Políticas de senhas
- Utilizar senhas fortes e exclusivas.
- Evitar senhas comuns e previsíveis.
- Implementar políticas adequadas de proteção de credenciais.

### 2. Autenticação
- Implementar autenticação multifator (MFA).
- Adotar mecanismos seguros de autenticação.
- Restringir tentativas consecutivas de login.

### 3. Monitoramento
- Monitorar logs de autenticação.
- Identificar padrões incomuns de acesso.
- Configurar alertas para tentativas suspeitas.

### 4. Segurança de rede
- Desabilitar serviços desnecessários.
- Restringir o acesso aos serviços por firewall.
- Utilizar protocolos seguros de comunicação.

### 5. Segurança em aplicações Web
- Implementar limitação de tentativas de login.
- Utilizar mecanismos contra automação abusiva.
- Implementar controles de sessão e autenticação.
- Monitorar tentativas suspeitas de acesso.

## 📚 Aprendizados Adquiridos

O desenvolvimento deste projeto proporcionou uma experiência prática sobre auditoria de segurança e avaliação de mecanismos de autenticação.

A utilização das ferramentas Medusa e THC Hydra permitiu compreender como tentativas automatizadas podem identificar credenciais vulneráveis.

Também reforçou a importância de ambientes controlados para estudos de segurança, da documentação técnica e da aplicação de medidas preventivas.

Além disso, o projeto contribuiu para o desenvolvimento de conhecimentos em Linux, redes, segurança da informação e análise de vulnerabilidades.

## 🎓 Conclusão

A realização deste projeto proporcionou uma experiência prática sobre auditoria de segurança e avaliação de mecanismos de autenticação.

Por meio do Kali Linux, Medusa e THC Hydra, foi possível conhecer ferramentas utilizadas em testes de autenticação e observar seus resultados em um ambiente virtual controlado.

As atividades com FTP, SMB e DVWA reforçaram a importância da utilização de senhas fortes, mecanismos de proteção contra tentativas automatizadas e monitoramento dos serviços.

O projeto contribuiu para ampliar meus conhecimentos em Linux, redes de computadores, segurança da informação e práticas de cibersegurança.

A experiência também reforçou a importância de realizar testes somente em ambientes próprios e autorizados.

## ⚠️ Aviso de Segurança

Este projeto possui finalidade exclusivamente educacional.

Todas as atividades de auditoria devem ser realizadas em ambientes próprios, virtuais, isolados e devidamente autorizados.

Não utilize as ferramentas apresentadas contra sistemas, redes ou serviços de terceiros sem autorização expressa.

## 📁 Estrutura do Repositório

```text
auditoria-seguranca-kali-medusa-hydra/
│
├── README.md
│
├── images/
│   ├── conexção-ftp.PNG
│   ├── DVWA.PNG
│   ├── hydra-dvwa.PNG
│   ├── medusa-ftp.PNG
│   ├── medusa-ftp-ataque.PNG
│   ├── medusa-smb.PNG
│   └── smb-conexcão.PNG
│
├── wordlists/
│   ├── users.txt
│   └── passwords.txt
│
└── docs/
    └── mitigacoes.md
```

## 🔗 Referências e Documentação

- [Kali Linux](https://www.kali.org/)
- [Medusa](https://github.com/jmk-foofus/medusa)
- [THC Hydra](https://github.com/vanhauser-thc/thc-hydra)
- [Metasploitable 2](https://sourceforge.net/projects/metasploitable/)
- [DVWA](https://github.com/digininja/DVWA)
- [Oracle VirtualBox](https://www.virtualbox.org/)

## 👨‍💻 Autor

Projeto desenvolvido como parte do desafio de cibersegurança da Digital Innovation One (DIO).

**Tema:** Auditoria de Segurança com Kali Linux, Medusa e THC Hydra.

**Área de estudo:** Cibersegurança | Pentest | Segurança da Informação | Auditoria de Autenticação.
