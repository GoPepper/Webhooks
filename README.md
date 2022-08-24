# Webhooks
A brief documentation of our webhooks.

## Fields

|  Fieldname   |      Type      |       Response Example       | Possibilities or Description |
| :----------: | :------------: | :-----------------: | :---: |
|   currency   |     string     |      "BRL"      | BRL, USD  |
| payment_engine | string | "pepper" | Constant field |
| transaction | string | "PP56489423" | Transactions Id |
| payment_type | string | "Billet" | Pix, Billet, Card |
| status | string | "Paid" | Created, WaitingPayment, Paid, Refused, Refunded | 
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
