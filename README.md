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
