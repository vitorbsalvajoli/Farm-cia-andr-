# Farmácia do André - Sistema Completo

Sistema completo de e-commerce para farmácia com 3 portais separados.

## 🌐 Sites (GitHub Pages)

### 1. Site do Cliente
**URL:** `https://vitorbsalvajoli.github.io/Farm-cia-andr-/site-cliente/`

- Catálogo de produtos
- Carrinho de compras
- Checkout com entrega
- Login/registro de clientes
- Acompanhamento de pedidos

### 2. Site da Farmácia (Monitoramento)
**URL:** `https://vitorbsalvajoli.github.io/Farm-cia-andr-/site-farmacia/`

- Gestão de pedidos em tempo real
- Atualização de status
- Controle de abertura/fechamento da loja
- Login de farmacêuticos
- Notificações sonoras

### 3. Site do Administrador
**URL:** `https://vitorbsalvajoli.github.io/Farm-cia-andr-/site-admin/`

- Dashboard completo
- Logs de todas as atividades
- Estatísticas de farmacêuticos
- Gráfico de vendas (7 dias)
- Lista de pedidos recentes

## 🔐 Credenciais de Teste

### Farmacêuticos:
| Código | Nome | Senha |
|--------|------|-------|
| FAR001 | Dr. André | 123456 |
| FAR002 | Dra. Maria | 123456 |
| FAR003 | Dr. João | 123456 |
| ADMIN | Administrador | admin123 |

## 📁 Estrutura do Projeto

```
Farm-cia-andr-/
├── site-cliente/          # Site dos clientes (GitHub Pages)
│   ├── index.html
│   ├── auth.html
│   ├── script.js
│   └── styles.css
├── site-farmacia/         # Site da farmácia (GitHub Pages)
│   ├── monitoramento.html
│   ├── script.js
│   └── styles.css
├── site-admin/            # Site do admin (GitHub Pages)
│   ├── admin.html
│   ├── script.js
│   └── styles.css
├── .github/workflows/     # Deploy automático
│   ├── deploy-site-cliente.yml
│   ├── deploy-site-farmacia.yml
│   └── deploy-site-admin.yml
├── index.html             # Arquivos originais (desenvolvimento)
├── auth.html
├── monitoramento.html
├── admin.html
├── script.js
├── styles.css
└── README.md
```

## 🚀 Deploy Automático

Os sites são deployados automaticamente ao fazer push para a branch `main`:

1. **Site do Cliente**: Deploy quando há mudanças em `site-cliente/`
2. **Site da Farmácia**: Deploy quando há mudanças em `site-farmacia/`
3. **Site do Admin**: Deploy quando há mudanças em `site-admin/`

## ⚙️ Como Funciona

### Fluxo do Cliente:
1. Acessa o site e faz login/registro
2. Adiciona produtos ao carrinho
3. Finaliza compra com endereço de entrega
4. Acompanha status do pedido

### Fluxo da Farmácia:
1. Farmacêutico faz login no monitoramento
2. Recebe notificações de novos pedidos
3. Atualiza status (Pendente → Preparando → Pronto → Saiu → Entregue)
4. Cada ação é registrada com código do farmacêutico

### Fluxo do Administrador:
1. Acessa dashboard completo
2. Vê todas as atividades em tempo real
3. Acompanha performance de cada farmacêutico
4. Visualiza relatório de vendas

## ⚠️ Limitações (localStorage)

Este sistema usa `localStorage` para armazenamento de dados, o que significa:
- ✅ Funciona completamente no navegador
- ✅ Não requer backend para demonstração
- ❌ Dados não são compartilhados entre dispositivos
- ❌ Cada usuário vê apenas seus próprios dados

Para produção real, é necessário implementar um backend com banco de dados.

## 📞 Contato da Farmácia

- **Endereço:** Av. Nove de Julho, 1381 - José Bonifácio - SP
- **Telefone:** (17) 3245-2992
- **Instagram:** @farmaciadoandre

---

Desenvolvido para Acc.2026