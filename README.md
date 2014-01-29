w2p-storefront
==============

A simple web2py/jQuery storefront using Stripe.js


Please refer to Stripe.js documentation to handle purchases properly:

1) Follow this tutorial to get your setPublishableKey ready to talk to stripe (https://stripe.com/docs/tutorials/forms)
-- this is implemented here, and you just need to change line 109 of storefront.html to your public key for Stripe.

2) Next, create the server side call to stripe (https://stripe.com/docs/tutorials/charges)
--not implemented on this project for security constraints with private key but this is project is a great boilerplate to start off

As always feel free to reach out to me if you have any questions.


Features:

Search - Live searching enables of products. Just type keywords and products appear/disappear (no need for form submission)

Shopping Cart - Added Plus and Minus to increase or decrease stock, also kept the universal trash for quick clearing.

Form Validation - All fields must be filled in, all financial information must be correct by Stripe.js (used their validation from their API).

AJAX Post - Posting the payment info to stripe, since stripe doesnt look at user information other than payment information. I pass the token, cart, and shipping details to be handled by server side code. Server side not implemented.

Processing - To allow for the mass demand, we created a simple wait to ensure our server isn't hit like crazy. I really just did this for looks. Also I didn't like the alerts messing up my nice pretty gif. Displaying some debug information under the processing image.

Clear Cart - The most requested feature. Once you submit your payment your cart is cleared and ready for more orders! :) So long as the user doesnt refresh the page, his/her payment information remains in the payment form just in case they wish to place another order. I know this is bad practice, but for testing purposes I left it on. 
