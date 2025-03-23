#FROM debian:latest

#RUN apt update && apt install -y tor && rm -rf /var/lib/apt/lists/*

#COPY torrc /etc/tor/torrc

#CMD ["tor"]

FROM python:3.9

# Instalar Tor e dependências
RUN apt update && apt install -y tor && rm -rf /var/lib/apt/lists/*

# Copiar os arquivos do projeto
COPY ./torrc /etc/tor/torrc


# Iniciar o Tor e a aplicação Flask
CMD tor 
