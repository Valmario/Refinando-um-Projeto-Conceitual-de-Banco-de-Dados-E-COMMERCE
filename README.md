# 📦 Projeto Conceitual de Banco de Dados: E-COMMERCE

Este projeto foi desenvolvido como parte do Bootcamp [**Heineken - Inteligência Artificial Aplicada a Dados com Copilot**](https://web.dio.me/track/coding-the-future-heineken-ia-para-analise-de-dados) na plataforma [**DIO**](https://www.dio.me/), com orientação da instrutora **Juliana Mascarenhas**.

---

## 🧩 Descrição do Desafio

> _"Modelamos juntos um contexto reduzido de e-commerce. Agora é a sua vez! Você pode escolher a ferramenta de modelagem para realizar o desafio. Caso opte por uma variação do modelo entidade-relacionamento, como nas ferramentas MySQL Workbench ou DBDesigner, será necessário especificar corretamente as PKs e FKs. Apesar desses conceitos não serem utilizados na modelagem conceitual, foram brevemente explorados. Seu entregável será o esquema conceitual para o cenário de E-commerce."_

---

## 🎯 Objetivo

Refinar o modelo apresentado em aula, incorporando os seguintes requisitos adicionais:

- **Cliente PJ e PF**: Uma conta pode ser de Pessoa Jurídica (PJ) ou Pessoa Física (PF), mas nunca ambas.
- **Pagamento**: O cliente pode ter mais de uma forma de pagamento cadastrada.
- **Entrega**: O pedido deve conter status e código de rastreio.

---

## 🛠️ Ferramentas Utilizadas

- [MySQL Workbench](https://www.mysql.com/products/workbench/)

---

## ✅ Solução Desenvolvida

### 📌 Principais Ajustes no Modelo:

- 🔸 **Cliente**: Foram criadas duas entidades separadas:
  - `PF_PessoaFisica` para armazenar informações de CPF.
  - `PJ_PessoaJuridica` para armazenar informações de CNPJ.
  Ambas se relacionam com a entidade principal `Cliente`.

- 🔸 **Pagamento**: A entidade `Pagamento` foi expandida para contemplar múltiplas formas, como:
  - `Cartao`
  - `Boleto`

- 🔸 **Entrega**: Criada a entidade `Entrega`, com os atributos:
  - `status`
  - `codigoRastreio`
  - `dataPedido`, `dataEnvio`, `dataEntrega`

### 📷 Diagrama do Modelo

![Diagrama ER](https://github.com/Valmario/Refinando-um-Projeto-Conceitual-de-Banco-de-Dados-E-COMMERCE/blob/main/ECOMMERCE/ecommerce_imagem.png)

---

## 📁 Estrutura do Projeto

```
📦 Refinando-um-Projeto-Conceitual-de-Banco-de-Dados-E-COMMERCE
 ┣ 📁 ECOMMERCE
 ┃ ┗ 📄 ecommerce_imagem.png
 ┗ 📄 README.md
```

---

## 👩‍🏫 Instrutora

**Juliana Mascarenhas**  
Especialista em Banco de Dados e Projetos Educacionais de Tecnologia.
