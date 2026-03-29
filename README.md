# 🚔 Sistema de Escalas - 15º BPM/PMPB

Sistema integrado de gestão de escalas da Polícia Militar da Paraíba - 15º Batalhão.

## 📋 Sobre o Sistema

Este aplicativo integra dois sistemas de escalas em uma única plataforma:

### 1. 📋 Escala CPU (Coordenador do Policiamento da Unidade)
- **Tipo:** Escala mensal
- **Funcionalidades:**
  - Cadastro e gerenciamento de militares
  - Geração automática de escala mensal
  - Destaque para fins de semana (sexta, sábado, domingo)
  - Classificação: Ordinário (preto) e Extra (vermelho)
  - Exportação em PDF e PNG formato A4
  - Sistema de notificações por militar
  - Tema claro/escuro
  - Persistência de dados (localStorage)

### 2. 🎯 Escala NUFAP-15 (Núcleo de Formação e Aperfeiçoamento Profissional)
- **Tipo:** Escala semanal
- **Funcionalidades:**
  - Gerenciamento de turnos (manhã/tarde)
  - Múltiplos militares por turno
  - Observações por dia
  - Exportação em PDF e PNG
  - Layout oficial PMPB
  - Persistência de dados

## 🚀 Instalação

### Como PWA (Progressive Web App)

1. **Acesse o sistema** em um navegador moderno (Chrome, Edge, Safari)
2. **Clique em "Instalar"** ou "Adicionar à tela inicial" quando solicitado
3. **Ou manualmente:**
   - Chrome/Edge: Menu → Instalar aplicativo
   - Safari: Compartilhar → Adicionar à Tela de Início

### Requisitos

- Navegador moderno com suporte a JavaScript
- Conexão com internet (para primeiro carregamento)
- Funciona offline após instalação

## 📁 Estrutura de Arquivos

```
sistema-escalas-integrado/
├── index.html          # Página inicial (hub)
├── cpu.html            # Sistema Escala CPU
├── nufap.html          # Sistema Escala NUFAP-15
├── manifest.json       # Configuração PWA
├── sw.js              # Service Worker (offline)
├── icons/             # Ícones do aplicativo
│   ├── icon-72x72.png
│   ├── icon-96x96.png
│   ├── icon-128x128.png
│   ├── icon-144x144.png
│   ├── icon-152x152.png
│   ├── icon-192x192.png
│   ├── icon-384x384.png
│   ├── icon-512x512.png
│   ├── icon-cpu.png
│   └── icon-nufap.png
└── README.md          # Este arquivo
```

## 🎯 Como Usar

### Página Inicial (Hub)

Ao abrir o aplicativo, você verá dois cards:
- **📋 Escala CPU** - Acesse o sistema de escala mensal
- **🎯 Escala NUFAP-15** - Acesse o sistema de escala semanal

Clique no card desejado para acessar o respectivo sistema.

### Escala CPU

1. **Selecione mês e ano** nos controles superiores
2. **Cadastre militares** na seção "Gerenciar Militares"
3. **Atribua escalas** clicando nos campos de cada dia
4. **Marque como Extra** quando necessário (nome fica vermelho)
5. **Exporte** em PDF ou PNG usando os botões superiores

### Escala NUFAP-15

1. **Edite os dados** no painel esquerdo:
   - Título e período
   - Nomes e graduações dos militares
   - Escala de turnos (manhã/tarde)
   - Observações por dia
2. **Clique em "Prévia"** para visualizar
3. **Exporte** em PDF ou PNG

## 💾 Persistência de Dados

Todos os dados são salvos automaticamente no **localStorage** do navegador:
- Lista de militares
- Escalas configuradas
- Preferências de tema
- Notificações ativas

⚠️ **Importante:** Os dados são salvos localmente no dispositivo. Para backup, exporte os arquivos PDF/PNG.

## 🔔 Notificações

No sistema CPU, você pode ativar notificações para militares específicos:
1. Clique no ícone de sino (🔔) ao lado do nome do militar
2. O sistema notificará um dia antes da escala (quando permitido pelo navegador)

## 🎨 Temas

O sistema CPU suporta tema claro e escuro:
- Clique no botão 🌓 no canto superior direito para alternar

## 📱 Compatibilidade

- ✅ Chrome/Edge (desktop e mobile)
- ✅ Safari (iOS)
- ✅ Firefox
- ✅ Samsung Internet

## 🔒 Segurança

- Todos os dados ficam armazenados localmente no dispositivo
- Nenhuma informação é enviada para servidores externos
- Funciona 100% offline após instalação

## 🛠️ Tecnologias

- HTML5
- CSS3 (com variáveis CSS)
- JavaScript (ES6+)
- Service Workers (PWA)
- LocalStorage API
- html2canvas (exportação de imagens)
- jsPDF (exportação de PDF)

## 📞 Suporte

Para suporte técnico ou sugestões, entre em contato com a equipe de TI do 15º BPM.

---

**Polícia Militar da Paraíba**  
**15º Batalhão de Polícia Militar**  
*Sistema de Gestão de Escalas - 2026*
