# -Email-Finder
# 📧 Email Finder (Web Crawler)

Uma ferramenta simples em Python que rastreia uma URL de partida, segue links internos e externos recursivamente, e extrai endereços de e-mail válidos encontrados nas páginas HTML. Útil para coleta de informações (OSINT) e testes de segurança.

## ✨ Funcionalidades

* **Rastreamento Recursivo:** Inicia em uma URL e segue todos os links encontrados que não foram rastreados anteriormente.
* **Extração de E-mails:** Utiliza expressões regulares para identificar e-mails no formato padrão.
* **Controle de Visitas:** Mantém um registro de URLs já rastreadas para evitar loops e repetições desnecessárias.

## ⚙️ Pré-requisitos

Certifique-se de ter o Python instalado. As seguintes bibliotecas são necessárias:

* `requests`
* `beautifulsoup4`

## 📦 Instalação

1.  Clone o repositório:
    ```bash
    git clone [https://github.com/SeuUsuario/SeuRepositorio.git](https://github.com/SeuUsuario/SeuRepositorio.git)
    cd SeuRepositorio
    ```
2.  Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

## 🚀 Uso

Execute o script fornecendo a URL inicial como argumento de linha de comando.

```bash
python email_finder.py <URL_DE_PARTIDA>
# Exemplo: python email_finder.py [http://exemplo.com](http://exemplo.com)
