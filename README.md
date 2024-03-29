# Webhooks
A brief documentation of our webhooks.

## Fields

|     Fieldname     |      Type      |       Response Example       | Possibilities or Description |
| :---------------: | :------------: | :--------------------------: | :--------------------------: |
|     currency      |     string     |             "BRL"            |            BRL, USD          |
|   payment_engine  |     string     |           "pepper"           |         Constant field       |
|     transaction   |     string     |         "PP56489423"         |         Transactions Id      |
|   abandonmentId   |     string     |          "PP213123"          |          Abandonment Id      |
|     client_id     |   string(guid) |  "00000-0000-0000-0000-000"  | To be used in the recovery of an abandoned cart |
| payment_type | string | "Billet" | Checkout, Pix, Billet, Card |
| status | string | "Paid" | Abandonment, Created, WaitingPayment, Paid, Refused, Refunded, Chargeback | 
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
| main_transaction | string | "PP56489423" | The main transaction. Could be the same value of transaction field |
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
| utm_campaign | string | "Campaing Name" | Tracking Parameter |
| utm_source | string | "Source Name" | Tracking Parameter |
| utm_medium | string | "Medium Name" | Tracking Parameter |
| utm_content | string | "Content Name" | Tracking Parameter |
| utm_term | string | "Term Name" | Tracking Parameter |
| src | string | "Source Name" | Tracking Parameter |
| sck | string | "Source Name" | Tracking Parameter |

# Exemplo em JSON:

```javascript
{
  "currency": "BRL",
  "payment_engine": "pepper",
  "transaction": "PP000",
  "abandonmentId": "PP000",
  "client_id": "0000-000-0000",
  "payment_type": "Card",
  "status": "Paid",
  "prod": 000000,
  "prod_name": "Fórmula Javascript",
  "producer_name": "Jake Peralta",
  "producer_document": "123.456.789-00",
  "producer_legal_nature": "Pessoa física",
  "purchase_date": "2023-02-07 18:15:52",
  "confirmation_purchase_date": "2023-02-07 18:16:04",
  "product_support_email": "suporte@email.com",
  "installments_number": 12,
  "original_offer_price": 100,
  "warranty_date": "2023-02-14 18:16:04",
  "order_bump": false,
  "cms_market_place": 5.89,
  "cms_vendor": 94.1,
  "off": 3,
  "price": 100,
  "full_price": 138.28,
  "email": "robert.jr@pepper.com.br",
  "name": "Robert Downey Jr",
  "first_name": "Robert",
  "last_name": "Jr",
  "doc": "987.654.321-10",
  "phone_number": "+551122233344",
  "billet_url": null,
  "billet_barcode": null,
  "pix_URL": "https://pepper.com.br/checkout/obrigado-pix.html?id=000",
  "pix_qrcode": null,
  "utm_campaign": null,
  "utm_source": null,
  "utm_medium": null,
  "utm_content": null,
  "utm_term": null,
  "src": null,
  "sck": null
}
```
