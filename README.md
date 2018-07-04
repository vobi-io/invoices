# invoices

* 1)იუზერის რეგისტრაცია და ლოგინი
* 2)იუაზერის ინვოისის შექმანა, რედატირება, წაშლა, ლისტი
* 3)ინვოისის დეტალების დამატება, რედაქტირება, წაშლა.
* 4)იუზერების ინვოისების სია

Mutation:
* login
* signup
* createInvoice
* editInvoice
* deleteInvoice
* createInvoiceDetails
* editInvoiceDetails
* deleteInvoiceDetails

Query:
* getInvoices (pagination, searchText: 'test')
* getInvoiceById
* getInvoicesByUserId
* getInvoiceDetailsByInvoiceId

```
user:
id
username,
email,
created,
activated


Invoice fields:
name,
date,
created,
modified,
userId,
description,
contactName,
address

Invoice details fields:
id,
name,
description,
quantity,
price,
total,
userId,
invoiceId
```

Please use:

backend:
* Database: mongodb (mongoose orm),
* Promise async await
* Node (express.js)
* grapqhl https://www.graphql.com/

Front: 
* react.js
* appollo client https://www.apollographql.com/client/
* bootrap
