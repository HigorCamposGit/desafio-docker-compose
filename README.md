# 🐳 Desafio Prático: Conteinerização de Aplicação Web com Docker Compose

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-D22128?style=for-the-badge&logo=Apache&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

Projeto prático desenvolvido para demonstrar a criação, configuração e execução de um servidor web **Apache HTTP Server (`httpd`)** conteinerizado com **Docker Compose**, utilizando mapeamento de volumes locais, personalização de layout em escuro e boas práticas de controle de versão.

---

## 📌 Visão Geral do Projeto

O objetivo deste desafio foi provisionar um ambiente web leve e isolado utilizando Docker, garantindo que alterações no código-fonte local (`HTML/CSS`) fossem refletidas instantaneamente no servidor em tempo de execução através do uso de **Volumes Mapeados**.

### Key Features & Implementações:
- **Servidor Web Isolado:** Imagem oficial do Apache HTTP Server (`httpd:latest`) configurada via Docker Compose.
- **Volume Bind Mount:** Mapeamento do diretório local `./website` para o diretório padrão de hospedagem do Apache (`/usr/local/apache2/htdocs/`).
- **Interface Responsiva:** Aplicação web estática customizada com tema escuro moderno e ícones Font Awesome.
- **Otimização de Build & Versionamento:** Arquivos `.gitignore` e `.dockerignore` configurados para evitar o envio de arquivos desnecessários tanto para a imagem do container quanto para o repositório remoto.

---

## 🛠️ Estrutura do Repositório

```text
desafio-docker-compose/
├── website/
│   ├── index.html        # Estrutura principal da página web
│   └── style.css         # Estilização externa em tema escuro
├── compose.yml           # Orquestração do container Docker
├── .gitignore            # Arquivos ignorados pelo Git
└── README.md             # Documentação do projeto
