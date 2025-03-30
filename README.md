# 📬 Sistema de Notificações em Swift

Este projeto é um sistema simples de notificações em Swift que permite o envio de mensagens por Email, SMS e Push Notification, com escolha de prioridade e tipo de mensagem. Ele roda no terminal e organiza as notificações para envio conforme sua prioridade.

## 🚀 Funcionalidades

- Suporte a múltiplos canais de notificação (Email, SMS, Push)
- Interface interativa via terminal (CLI)
- Escolha de tipo de mensagem (Alerta, Promoção, Lembrete)
- Escolha de prioridade (Alta, Média, Baixa)
- Envio das notificações agrupadas por prioridade

## 🛠️ Tecnologias

- Swift (puro)
- Entrada e saída via readLine() e print()

## 📦 Estrutura do Projeto

- Notificavel – protocolo que define o que uma notificação deve implementar.
- Email, SMS, PushNotification – structs que representam os diferentes canais.
- Mensagem – struct que representa a mensagem a ser enviada.
- Prioridade e TipoMensagem – enums para organizar o tipo de mensagem e sua urgência.
- Funções auxiliares para escolha de tipo e prioridade e agrupamento de notificações.

## 🧪 Como Usar

1. Compile o projeto em um ambiente com suporte a Swift (como Xcode ou terminal com swiftc).
2. Execute o arquivo.
3. Use o menu para:
   - Adicionar notificações
   - Escolher tipo e prioridade
   - Enviar todas as notificações agrupadas

## 📸 Exemplo de Saída

Menu:
1 - Adicionar Email
2 - Adicionar SMS
3 - Adicionar Push Notification
4 - Enviar Notificações
0 - Sair

══════════════════════════════════════════════════════
Enviando notificações com prioridade Alta:
[SMS] Enviando SMS de [Alerta] para (99) 99999-9999: Sistema fora do ar. [Prioridade: Alta]
══════════════════════════════════════════════════════

## 🤓 Decisões de Design

- Uso de protocolo para permitir polimorfismo.
- Enumerações para evitar valores inválidos.
- Separação de lógica por funções auxiliares.
- Interface simples e acessível via terminal.

