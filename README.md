# 🐳 Docker Web Application

Uma aplicação web moderna e responsiva rodando em container Apache HTTP Server usando Docker Compose.

## 📋 Sobre o Projeto

Este projeto demonstra como criar e executar uma aplicação web completa usando Docker e Docker Compose. A aplicação inclui uma interface moderna desenvolvida com HTML5, CSS3 e JavaScript, rodando em um servidor Apache containerizado.

## 🚀 Tecnologias Utilizadas

- **Docker** - Containerização da aplicação
- **Docker Compose** - Orquestração de containers
- **Apache HTTP Server** - Servidor web (httpd:2.4-alpine)
- **HTML5** - Estrutura da aplicação
- **CSS3** - Estilização moderna e responsiva
- **JavaScript** - Funcionalidades interativas
- **Font Awesome** - Ícones
- **Google Fonts** - Tipografia (Inter)

## 🎯 Funcionalidades

### ✨ Interface Moderna
- Design responsivo e mobile-first
- Animações suaves e transições
- Tema moderno com gradientes
- Navegação suave entre seções

### 🔧 Recursos Interativos
- **Contador Dinâmico** - Incrementar/decrementar valores
- **Gerador de Cores** - Cores aleatórias com código hexadecimal
- **Status do Container** - Tempo online em tempo real
- **Formulário de Contato** - Com validação e persistência local

### 🎮 Easter Eggs
- Konami Code para efeitos especiais
- Sistema de notificações
- Console interativo com comandos

## 📁 Estrutura do Projeto

```
docker/
├── docker-compose.yml          # Configuração do Docker Compose
├── README.md                   # Documentação do projeto
└── src/                        # Código fonte da aplicação
    ├── index.html             # Página principal
    ├── css/
    │   └── style.css          # Estilos da aplicação
    └── js/
        └── script.js          # Scripts JavaScript
```

## 🛠️ Como Executar

### Pré-requisitos
- Docker instalado
- Docker Compose instalado

### Passos para execução

1. **Clone ou baixe o projeto**
   ```bash
   git clone <seu-repositorio>
   cd docker
   ```

2. **Execute com Docker Compose**
   ```bash
   docker-compose up -d
   ```

3. **Acesse a aplicação**
   - Abra seu navegador
   - Vá para: `http://localhost:8080`

4. **Para parar a aplicação**
   ```bash
   docker-compose down
   ```

## 🐳 Configuração Docker

### docker-compose.yml
O arquivo de configuração define:
- **Serviço**: apache-web
- **Imagem**: httpd:2.4-alpine (Apache HTTP Server)
- **Porta**: 8080 (host) → 80 (container)
- **Volume**: ./src mapeado para /usr/local/apache2/htdocs
- **Restart**: unless-stopped

### Benefícios da Containerização
- ✅ Ambiente isolado e consistente
- ✅ Fácil deployment e portabilidade
- ✅ Baixo overhead (Alpine Linux)
- ✅ Escalabilidade simplificada

## 🎨 Recursos da Interface

### Design System
- **Cores Primárias**: #007acc (azul), #00d4ff (accent)
- **Tipografia**: Inter (Google Fonts)
- **Espaçamento**: Sistema baseado em rem
- **Responsividade**: Mobile-first approach

### Componentes
- Header fixo com navegação suave
- Hero section com animações
- Cards informativos
- Formulários estilizados
- Footer com links úteis

## 📱 Responsividade

A aplicação é totalmente responsiva com breakpoints:
- **Desktop**: > 768px
- **Tablet**: 768px - 480px
- **Mobile**: < 480px

## 🔧 Funcionalidades JavaScript

### Principais Recursos
- Navegação suave entre seções
- Contador interativo com animações
- Gerador de cores aleatórias
- Timer de uptime do container
- Sistema de notificações
- Persistência no localStorage
- Easter eggs e interações especiais

### Comandos do Console
Execute no console do navegador:
- `debugInfo()` - Informações de debug
- `mostrarInfo()` - Detalhes da aplicação
- `gerarCor()` - Nova cor aleatória
- `incrementar()` / `decrementar()` - Controle do contador

## 🚀 Possíveis Expansões

### Backend
- **Node.js**: Express.js server
- **Python**: Flask ou Django
- **PHP**: Apache + PHP-FPM
- **Go**: Gin web framework

### Banco de Dados
- MySQL/PostgreSQL para persistência
- Redis para cache
- MongoDB para dados não-relacionais

### DevOps
- CI/CD com GitHub Actions
- Deploy automatizado
- Monitoramento com Prometheus
- Logs centralizados

## 📚 Documentação Adicional

### Links Úteis
- [Docker Documentation](https://docs.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Apache HTTP Server](https://httpd.apache.org/docs/)

### Comandos Docker Úteis
```bash
# Ver containers rodando
docker ps

# Ver logs do container
docker logs minha-aplicacao-web

# Executar comando no container
docker exec -it minha-aplicacao-web sh

# Rebuild após mudanças
docker-compose up --build
```

## 🤝 Contribuindo

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto é para fins educacionais e está disponível sob a licença MIT.

## 📞 Contato

Desenvolvido com ❤️ para aprendizado de Docker e desenvolvimento web.

---

🐳 **Happy Coding with Docker!** 🚀
