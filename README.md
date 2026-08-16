# 🖥️ Lab de Redes: Configuração e Segurança Básica (Cisco Packet Tracer)

![Cisco](https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Packet Tracer](https://img.shields.io/badge/Packet_Tracer-000000?style=for-the-badge&logo=cisco&logoColor=white)

## 📖 Sobre o Projeto
Este repositório contém a resolução de um laboratório prático de Redes de Computadores desenvolvido no **Cisco Packet Tracer**. 
O objetivo principal deste projeto foi aplicar na prática conceitos fundamentais de infraestrutura, roteamento, e segurança básica em equipamentos Cisco (Cisco IOS), simulando um ambiente real do dia a dia de um profissional de redes.

## 🎯 Tarefas Realizadas
O laboratório foi construído para solucionar os seguintes desafios propostos:
1. Configurar o endereço IP nas interfaces.
2. Garantir que os roteadores consigam pingar entre si.
3. Configurar a senha de acesso privilegiado do roteador.
4. Criptografar as senhas configuradas em texto claro.
5. Configurar uma senha criptografada nativamente (secret).
6. Configurar e liberar o acesso remoto via protocolo Telnet (VTY).
7. Testar a conectividade e o acesso remoto corretamente.
8. Configurar uma senha de proteção para a porta de Console.

## 🛠️ Comandos Utilizados (Cisco IOS)
Abaixo estão os principais comandos utilizados para a resolução do laboratório, divididos por categoria:

### Navegação e Verificação
```text
- enable                        # Entrar no modo privilegiado
- configure terminal (conf t)   # Entrar no modo de configuração global
- exit                          # Sair do modo atual
- show ip interface brief       # Visão geral das interfaces e IPs
- show running-config           # Verificar as configurações atuais em execução
```

### Configuração de Interfaces e Comunicação
```text
- hostname [Nome]               # Renomear o equipamento
- interface gigabitEthernet 0/0/0 # Acessar a interface de rede
- ip address [IP] [Mascara]     # Atribuir um endereço IPv4
- no shutdown                   # Ligar (ativar) a interface
- ping [IP]                     # Testar conectividade (ICMP)
```

### Segurança e Acesso Remoto
```text
- enable password [senha]       # Criar senha para o modo privilegiado
- service password-encryption   # Criptografar senhas de texto claro
- enable secret [senha]         # Criar senha forte criptografada
- line console 0                # Acessar configurações da porta física de console
- line vty 0 4                  # Acessar configurações de portas virtuais (Telnet/SSH)
- password [senha]              # Definir senha para a linha (console/vty)
- login                         # Exigir autenticação no acesso
- telnet [IP]                   # Acessar outro equipamento remotamente
```

### Persistência de Dados
```text
- copy running-config startup-config # Salvar as configurações na NVRAM
```

<img width="1439" height="849" alt="Captura de tela 2026-08-15 223940" src="https://github.com/user-attachments/assets/63c911ca-b9f9-4f4f-aa6b-6af8185b7ffd" />


## 🚀 Como testar este laboratório
1. Certifique-se de ter o **Cisco Packet Tracer** instalado em sua máquina.
2. Faça o clone deste repositório ou baixe o arquivo `.pkt`.
3. Abra o arquivo no Packet Tracer.
4. Utilize as senhas configuradas (`cisco` e `cisco123`) para explorar as configurações através da aba CLI dos roteadores.

