# Day 1: Create an EC2 Key Pair

---

## English

Created an RSA key pair in AWS (us-east-1) for use in future EC2 instance access.

```bash
aws ec2 create-key-pair --region us-east-1 --key-name nautilus-kp --key-type rsa

# Validate
aws ec2 describe-key-pairs \
  --region us-east-1 \
  --key-names nautilus-kp
```

> Key pairs are required to SSH into EC2 instances. The private key is only available at creation time — store it securely.

---

## Español

Creé un key pair de tipo RSA en AWS (us-east-1) para usar en futuros accesos a instancias EC2.

```bash
aws ec2 create-key-pair --region us-east-1 --key-name nautilus-kp --key-type rsa

# Validar
aws ec2 describe-key-pairs \
  --region us-east-1 \
  --key-names nautilus-kp
```

> Los key pairs son necesarios para conectarse por SSH a instancias EC2. La clave privada solo está disponible al momento de la creación — guardarla en un lugar seguro.

---

## Português

Criei um key pair do tipo RSA na AWS (us-east-1) para uso em futuros acessos a instâncias EC2.

```bash
aws ec2 create-key-pair --region us-east-1 --key-name nautilus-kp --key-type rsa

# Validar
aws ec2 describe-key-pairs \
  --region us-east-1 \
  --key-names nautilus-kp
```

> Key pairs são necessários para conectar via SSH em instâncias EC2. A chave privada só está disponível no momento da criação — guarde-a em local seguro.
