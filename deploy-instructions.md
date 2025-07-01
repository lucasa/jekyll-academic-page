# Instruções de Deploy para GitHub Pages

## Pré-requisitos

1. Conta no GitHub
2. Git instalado localmente

## Passos para Deploy

### 1. Criar Repositório no GitHub

1. Acesse [GitHub](https://github.com) e faça login
2. Clique em "New repository"
3. Nome sugerido: `geyer-academic-page` ou `claudio-geyer-ufrgs`
4. Marque como "Public"
5. NÃO inicialize com README (já temos um)
6. Clique em "Create repository"

### 2. Configurar Git Local

No diretório do projeto, execute:

```bash
git init
git add .
git commit -m "Initial commit - Jekyll academic page"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
git push -u origin main
```

### 3. Configurar GitHub Pages

1. No repositório do GitHub, vá em "Settings"
2. Role até a seção "Pages"
3. Em "Source", selecione "Deploy from a branch"
4. Selecione a branch "main"
5. Selecione a pasta "/ (root)"
6. Clique em "Save"

### 4. Aguardar Deploy

- O GitHub Pages levará alguns minutos para fazer o build
- Você receberá um link como: `https://SEU_USUARIO.github.io/NOME_DO_REPOSITORIO`
- O site será atualizado automaticamente a cada push para a branch main

### 5. Configurar Domínio Personalizado (Opcional)

Se você tiver um domínio próprio:

1. Crie um arquivo `CNAME` na raiz do projeto com o domínio
2. Configure os DNS do domínio para apontar para o GitHub Pages
3. No GitHub, em Settings > Pages, adicione o domínio personalizado

## Atualizações Futuras

Para atualizar o site:

```bash
# Fazer alterações nos arquivos
git add .
git commit -m "Descrição das alterações"
git push origin main
```

O GitHub Pages fará o rebuild automaticamente.

## Estrutura de Arquivos para GitHub Pages

O projeto já está configurado corretamente para GitHub Pages com:

- `_config.yml` - Configuração do Jekyll
- `_layouts/` - Templates de página
- `assets/css/` - Estilos CSS
- Páginas em Markdown na raiz
- `Gemfile` com dependências necessárias

## Troubleshooting

### Erro de Build

Se o build falhar:

1. Verifique os logs em Actions > Pages build and deployment
2. Certifique-se de que o `_config.yml` está correto
3. Verifique se não há erros de sintaxe nos arquivos Markdown

### Site não carrega

1. Verifique se o GitHub Pages está habilitado
2. Aguarde alguns minutos após o primeiro deploy
3. Limpe o cache do navegador

### Estilos não carregam

1. Verifique se o arquivo CSS está no caminho correto
2. Certifique-se de que o layout está referenciando o CSS corretamente

## Customizações Adicionais

Para personalizar ainda mais:

1. Edite `assets/css/style.css` para alterar cores e estilos
2. Modifique `_layouts/default.html` para alterar a estrutura
3. Atualize `_config.yml` para alterar configurações do site
4. Adicione novas páginas criando arquivos `.md` na raiz

