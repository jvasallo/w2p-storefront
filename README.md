w2p-storefront
==============

A simple web2py/jQuery storefront using Stripe.js


Please refer to Stripe.js documentation to handle purchases properly:

1) Follow this tutorial to get your setPublishableKey ready to talk to stripe (https://stripe.com/docs/tutorials/forms)
-- this is implemented here, and you just need to change line 109 of storefront.html to your public key for Stripe.

2) Next, create the server side call to stripe (https://stripe.com/docs/tutorials/charges)
--not implemented on this project for security constraints with private key but this is project is a great boilerplate to start off

As always feel free to reach out to me if you have any questions.
