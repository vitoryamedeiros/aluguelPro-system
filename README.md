# Sistema de Aluguel de Mesas e Cadeiras

Este projeto consiste em um sistema simples e eficiente para gerenciamento de aluguel de mesas e cadeiras, com uma área administrativa e uma página pública para clientes.

## 📂 Estrutura de Arquivos

- `index.html`: **Painel Administrativo**. Onde o proprietário gerencia o estoque, define preços e registra pedidos.
- `cliente.html`: **Página do Cliente**. Onde os clientes podem ver os produtos, calcular preços e fazer pedidos via WhatsApp.
- `README.md`: Este arquivo de instruções.

## 🚀 Como Usar

### 1. Configuração Inicial (Admin)
1. Abra o arquivo `index.html` no seu navegador.
2. Clique no botão **"⚙️ Configurações"** no topo da página.
3. Defina:
   - Preço da Mesa e da Cadeira.
   - Seu número de WhatsApp (apenas números, com DDD).
   - Sua chave PIX.
   - Mensagem de boas-vindas (opcional).
4. Clique em **"Salvar Configurações"**.

### 2. Para os Clientes
1. Envie o arquivo `cliente.html` para seus clientes ou hospede-o em um servidor.
2. O cliente acessa a página, escolhe a quantidade de mesas/cadeiras.
3. Preenche os dados (Data, Endereço, etc.).
4. O sistema calcula o total automaticamente.
5. Ao clicar em **"Finalizar Pedido"**, o cliente vê a chave PIX e um botão para enviar o pedido já formatado para o seu WhatsApp.

### 3. Recebendo Pedidos
1. Você receberá uma mensagem no WhatsApp com todos os detalhes do pedido.
2. No Painel Administrativo (`index.html`), clique em **"📥 Importar WhatsApp"**.
3. Cole a mensagem recebida e clique em **"Processar Texto"**.
4. O formulário será preenchido automaticamente.
5. Clique em **"✓ Registrar Aluguel"** para salvar.

## 📱 Funcionalidades
- **Totalmente Responsivo**: Funciona em celulares e computadores.
- **Sem Servidor**: Todos os dados ficam salvos no seu navegador (localStorage).
- **Integração WhatsApp**: Fluxo simplificado para fechar negócios.
- **Controle de Estoque**: Saiba quantas mesas/cadeiras estão disponíveis em tempo real.

## ⚠️ Importante
Como o sistema não usa banco de dados online, os dados do Painel Administrativo ficam salvos **apenas no navegador onde você usa o sistema**. Se trocar de computador ou limpar o cache, os dados podem ser perdidos. Recomenda-se fazer backups manuais se necessário.
