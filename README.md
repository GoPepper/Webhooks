# Webhooks
A brief documentation of our webhooks.

## Fields

|     Fieldname     |      Type      |       Response Example       | Possibilities or Description |
| :---------------: | :------------: | :--------------------------: | :--------------------------: |
|     currency      |     string     |             "BRL"            |            BRL, USD          |
| payment_engine | string | "pepper" | Constant field |
| transaction | string | "PP56489423" | Transactions Id |
| payment_type | string | "Billet" | Pix, Billet, Card |
| status | string | "Paid" | Created, WaitingPayment, Paid, Refused, Refunded, Chargeback | 
| prod | int32 | 10000 | Product Id |
| prod_name | string | "Maratona Javascript em 30 dias" | Product name |
| producer_name | string | "Escola de curso online LTDA" | Producer name |
| producer_document | string | "12.3456.789/0001-10" | Producer document number |
| producer_legal_nature | string | "Pessoa Jurídica | Pessoa física, Pessoa Jurídica |
| purchase_date | string | "2022-08-24 15:10:59" | Purchase date |
| confirmation_purchase_date | string | "2022-08-24 15:10:59" | Approved date |
| product_support_email | string | "suporte@javascript.com" | Product Support Email |
| installments_number | int32 | 12 | Number of transaction installments |
| original_offer_price | float | 29.90 | Price before taxes |
| warranty_date | string | "2022-08-24 15:10:59" | Warranty deadline |
| order_bump | bool | false | If product is orderbump |
| cms_market_place | float | 3.21 | Platform tax amount |
| cms_vendor | float | 24.31 | Producer amount |
| off | int32 | 10232 | Offer Id |
| price | float | 29.90 | Offer price before taxes |
| full_price | float | 34.90 | Price paid by client |
| email | string | "user@gopepper.com.br" | Client email |
| name | string | "João Maria" | Client full name |
| first_name | string | "João" | Client first name |
| last_name | string | "Maria" | Client last name |
| doc | string | "111.222.333-45" | Client document number |
| phone_number | string | "+5511970503010" | Client phone number |
| billet_url | string | "https://pepper.com.br/example" | Billet payment page |
| billet_barcode | string | "00000 11111 22222 333333" | Billet Barcode |
| pix_URL | string | "https://pepper.com.br/example" | Pix payment page |
| pix_qrcode | string | "0002010100006820014br.example" | Pix QRCode |


# Transação

A transação contém informações relacionadas a um pagamento realizado por um cliente.

## Campos da Transação

### currency

- Tipo: string
- Descrição: A moeda utilizada na transação. Exemplo: "BRL".

### payment_engine

- Tipo: string
- Descrição: O nome da plataforma que processou o pagamento. Exemplo: "pepper".

### transaction

- Tipo: string
- Descrição: O identificador único da transação. Exemplo: "PP126".

### payment_type

- Tipo: string
- Descrição: O tipo de pagamento utilizado na transação. Exemplo: "Card".

### status

- Tipo: string
- Descrição: O status atual da transação. Exemplo: "Paid".

### prod

- Tipo: int
- Descrição: O identificador único do produto adquirido na transação. Exemplo: 10002.

### prod_name

- Tipo: string
- Descrição: O nome do produto adquirido na transação. Exemplo: "LALALA 2a".

### producer_name

- Tipo: string
- Descrição: O nome completo do produtor do produto adquirido na transação. Exemplo: "Alexandre Flores John".

### producer_document

- Tipo: string
- Descrição: O documento do produtor do produto adquirido na transação. Exemplo: "023.832.780-92".

### producer_legal_nature

- Tipo: string
- Descrição: A natureza jurídica do produtor do produto adquirido na transação. Exemplo: "Pessoa física".

### purchase_date

- Tipo: string
- Descrição: A data e hora da compra na transação. Exemplo: "2023-02-07 18:15:52".

### confirmation_purchase_date

- Tipo: string
- Descrição: A data e hora da confirmação da compra na transação. Exemplo: "2023-02-07 18:16:04".

### product_support_email

- Tipo: string
- Descrição: O email de suporte ao produto adquirido na transação. Exemplo: "askamskm@gmail.com".

### installments_number

- Tipo: int
- Descrição: O número de parcelas da transação
