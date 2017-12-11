# invoices

* 1)იუზერის რეგისტრაცია და ლოგინი
* 2)იუაზერის ინვოისის შექმანა, რედატირება, წაშლა, ლისტი
* 3)ინვოისის დეტალების დამატება, რედაქტირება, წაშლა.
* 4)იუზერების ინვოისების სია

routes:
* /user/login (POST)
* /user/signup (POST)
* /user/:id/invoices (query params: page (required), searchText : 'test')

* /invoices/create (POST)
* /invoices/edit (PUT)
* /invoices/delete (DELETE)
* /invoices/list (GET) (query params: page (required), searchText : 'test')

* /invoices/:id/details (GET)
* /invoices/:id/details/:id (GET)
* /invoices/:id/details/:id/edit (PUT)
* /invoices/:id/details/:id/create (POST)
* /invoices/:id/details/:id/delete (DELETE)

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

უნდა გამოიყენოთ:
* ბაზა: mongodb (mongoose orm),
* Promise,
* express.js

