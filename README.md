# Neighborhood - Aplicação para Avaliação de Vizinhos

Este repositório contém uma aplicação web chamada Neighborhood, que permite aos usuários avaliarem seus vizinhos e participarem de comunidades locais.

## Funcionalidades

- Avaliação de vizinhos (barulhentos, fumantes, etc.)
- Criação e gestão de comunidades (edifícios, condomínios, ruas)
- Sistema de assinatura premium para recursos avançados
- Interface administrativa com Netlify CMS

## Tecnologias Utilizadas

- Next.js
- Tailwind CSS
- Netlify CMS
- Netlify Identity para autenticação

## Estrutura do Projeto

- `public/admin/` - Configuração do Netlify CMS
- `content/` - Arquivos de conteúdo gerenciados pelo CMS
- `src/app/` - Páginas da aplicação Next.js
- `src/components/` - Componentes reutilizáveis
- `src/lib/` - Utilitários e funções de API

## Instruções de Deploy

### Pré-requisitos

- Conta no GitHub
- Conta no Netlify

### Passos para Deploy

1. Faça fork deste repositório para sua conta GitHub
2. Acesse o Netlify e clique em "New site from Git"
3. Selecione GitHub como provedor e autorize o Netlify
4. Selecione o repositório que você acabou de criar
5. Configure as opções de build:
   - Build command: `npm run build`
   - Publish directory: `.next`
6. Clique em "Deploy site"

### Configuração do Netlify CMS

1. Após o deploy, acesse as configurações do site no Netlify
2. Vá para "Identity" e clique em "Enable Identity"
3. Em "Registration preferences", selecione "Invite only"
4. Em "Services > Git Gateway", clique em "Enable Git Gateway"
5. Convide usuários administradores em "Identity > Invite users"

### Acesso ao CMS

Após a configuração, o CMS estará disponível em:
`https://seu-site.netlify.app/admin/`

## Desenvolvimento Local

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/neighborhood-app.git

# Entre no diretório
cd neighborhood-app

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

Acesse `http://localhost:3000` para ver a aplicação em funcionamento.

## Licença

Este projeto está licenciado sob a licença MIT.
