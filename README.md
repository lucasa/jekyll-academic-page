# Página Acadêmica do Professor Cláudio Geyer

Este é um projeto Jekyll para GitHub Pages que replica a página acadêmica do Professor Cláudio Geyer do Instituto de Informática da UFRGS.

## Sobre o Projeto

O site foi desenvolvido usando o tema [Alembic](https://github.com/daviddarnes/alembic) como base, com personalizações para refletir o design e conteúdo da página original do professor.

## Características

- **Design responsivo** baseado no tema Alembic
- **Cores personalizadas** inspiradas na identidade visual da UFRGS
- **Navegação intuitiva** com seções organizadas
- **Conteúdo acadêmico** completo incluindo pesquisa, ensino e contato
- **Compatível com GitHub Pages**

## Estrutura do Site

- **Home** (`/`) - Página principal com biografia resumida
- **Sobre** (`/about/`) - Informações detalhadas sobre formação e experiência
- **Pesquisa** (`/research/`) - Áreas de pesquisa e projetos atuais
- **Ensino** (`/teaching/`) - Disciplinas e orientações
- **Contato** (`/contact/`) - Informações de contato e links

## Tecnologias Utilizadas

- Jekyll 4.3.2
- Tema Alembic (remote theme)
- Sass/SCSS para estilos personalizados
- Markdown para conteúdo
- GitHub Pages para hospedagem

## Como Usar

### Pré-requisitos

- Ruby (versão 2.7 ou superior)
- Bundler
- Git

### Instalação Local

1. Clone o repositório:
   ```bash
   git clone [URL_DO_REPOSITORIO]
   cd geyer-academic-page
   ```

2. Instale as dependências:
   ```bash
   bundle install
   ```

3. Execute o servidor local:
   ```bash
   bundle exec jekyll serve
   ```

4. Acesse `http://localhost:4000` no seu navegador

### Deploy no GitHub Pages

1. Faça fork ou clone este repositório
2. Configure o GitHub Pages nas configurações do repositório
3. Selecione a branch `main` como fonte
4. O site será automaticamente construído e publicado

## Personalização

### Configuração

Edite o arquivo `_config.yml` para personalizar:

- Título e descrição do site
- Informações de contato
- Links de navegação
- Configurações de SEO

### Estilos

Os estilos personalizados estão em `assets/styles.scss`. Você pode modificar:

- Cores do tema
- Tipografia
- Layout e espaçamento
- Responsividade

### Conteúdo

As páginas estão em arquivos Markdown na raiz do projeto:

- `index.md` - Página inicial
- `about.md` - Sobre
- `research.md` - Pesquisa
- `teaching.md` - Ensino
- `contact.md` - Contato

## Estrutura de Arquivos

```
geyer-academic-page/
├── _config.yml          # Configuração do Jekyll
├── Gemfile              # Dependências Ruby
├── README.md            # Este arquivo
├── index.md             # Página inicial
├── about.md             # Página sobre
├── research.md          # Página de pesquisa
├── teaching.md          # Página de ensino
├── contact.md           # Página de contato
└── assets/
    └── styles.scss      # Estilos personalizados
```

## Contribuição

Para contribuir com melhorias:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Contato

Para dúvidas sobre o projeto, entre em contato através dos canais disponíveis na página de contato do site.

---

*Baseado no tema Alembic por David Darnes*

