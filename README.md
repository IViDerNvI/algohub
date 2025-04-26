# AlgoHub

## Getting Started

### Clone the Repository

To get started, clone the repository:

```bash
git clone https://github.com/ividernvi/algohub.git
cd algohub
```

### Generate SSL Certificate and Key

To enable HTTPS, you can generate a self-signed SSL certificate and key using OpenSSL:

```bash
cd conf/cert
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout private.key
 -out public.crt
```

This will create two files:

- `private.key`: The private key.
- `public.crt`: The self-signed certificate.

Place these files in a secure location and configure your application to use them.

### Run with Docker Compose

Ensure you have Docker and Docker Compose installed. Then, run the following command:

```bash
cd algohub
docker-compose up -d
```

This will build and start the application in a containerized environment.
