# Desafio Módulo Docker - StackX

Este repositório contém as soluções para o desafio do módulo Docker, separadas em duas atividades distintas. Cada atividade foi projetada para explorar conceitos de contêineres e boas práticas no uso do Docker.

## Estrutura do Repositório

```
desafio-modulo-docker-stackx/
├── README.md         # Este arquivo, documentação geral
├── atv1/             # Diretório da Atividade 1
│   ├── Dockerfile    # Dockerfile para empacotar a aplicação
│   ├── index.html    # Página HTML simples para exibição
│   └── README.md     # Documentação específica da Atividade 1
├── atv2/             # Diretório da Atividade 2
│   ├── docker-compose.yml # Configuração da stack Wiki.js + Postgres
│   ├── .env              # Variáveis de ambiente
│   └── README.md         # Documentação específica da Atividade 2
```

---

## Atividade 1: Empacotando uma Aplicação com Nginx

Nesta atividade, o objetivo foi criar uma imagem Docker personalizada para servir uma aplicação frontend simples com Nginx. A aplicação consiste em um arquivo `index.html` que exibe uma mensagem de boas-vindas.

### Destaques:
- Baseado na imagem oficial do Nginx com menor tamanho (alpine).
- Variável de ambiente `APP_VERSION` configurada.
- Instalação de ferramentas extras: `curl`, `htop` e `wget`.
- Porta de comunicação exposta: `80/TCP`.

Mais detalhes podem ser encontrados no arquivo [README da Atividade 1](./atv1/README.md).

---

## Atividade 2: Plataforma Wiki.js com Banco de Dados Postgres

Nesta atividade, foi configurada uma stack utilizando **Docker Compose** para implementar a plataforma Wiki.js com persistência em um banco de dados Postgres. A stack inclui dois containers:
- **Postgres**: Banco de dados para armazenamento de dados da Wiki.
- **Wiki.js**: Plataforma de documentação.

### Destaques:
- Configuração completa com variáveis de ambiente para credenciais.
- Persistência de dados utilizando volumes Docker.
- Comunicação em rede entre os serviços via Docker Compose.
- A aplicação é acessível na porta `3000`.

Mais detalhes podem ser encontrados no arquivo [README da Atividade 2](./atv2/README.md).

---

## Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/desafio-modulo-docker-stackx.git
   ```
2. Navegue até o diretório da atividade que deseja executar:
   ```bash
   cd atv1 # ou cd atv2
   ```
3. Siga as instruções específicas no README de cada atividade para construir e executar os containers.

---

## Licença
Este projeto é apenas para fins educacionais e não possui licença específica.

---

Se você tiver dúvidas ou sugestões, fique à vontade para abrir uma *issue* ou entrar em contato!
