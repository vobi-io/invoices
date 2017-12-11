# invoices

1)იუზერის რეგისტრაცია და ლოგინი
2)იუაზერის ინვოისის შექმანა, რედატირება, წაშლა, ლისტი
3)ინვოისის დეტალების დამატება, რედაქტირება, წაშლა.
4)იუზერების ინვოისების სია

routes:
/user/login
/user/signup
/user/:id:/invoices (query params: page (required), searchText : 'test')

/invoices/create
/invoices/update
/invoices/edit
/invoices/delete
/invoices/list (query params: page (required), searchText : 'test')

/invoices/:id/details
/invoices/:id/details/:id
/invoices/:id/details/:id/edit
/invoices/:id/details/:id/create
/invoices/:id/details/:id/delete

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
desctiption
quantity,
price,
total,
userId,
invoiceId


გამოყენებული უნდა იქნას:
ბაზა: mongodb (mongoose orm),
Promise,
express.js

