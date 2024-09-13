# gnr-qbo-test
Playing with Intuit API with the goal of integrating HTML forms for client

#### Client requests a major update to the basic functionality of their customer-facing site to include:
* Ability to input their own info (name, contact numbers, emails, address, etc)
* Ability to choose which type of product they'll be buying (drop-down menu)
* Integration into at least one mapping API in order to estimate shipping charges
* Integration into client's QuickBooks Online for the express purpose of creating an invoice directly from the webpage.

#### Actions continue to ripple for client:
* QBO is preferred vendor for tax tables
* QBO can be triggered to automatically send customers their invoices once been created within QBO after triggering API
* QBO will then include online payment options within email/hosted on their own servers

##### Further questions that need to be answered:
* What happens when the customer already exists? The HTML form seems useful for new customers, but without some sort of login or caching, it may gum up the works and create multiple copies of a customer or incorrectly pull data from an unrelated, but matched customer.
* Determine whether QBO API requires sequential calls to first create a customer, and then next create an invoice.
* Depending on the above, and also upon the workflow for the geo-mapping API, we may need a small server to manage things.
* How does the client account for the virtual inventory of their products?


#### Notes for debugging/improving overall site
* Add a favicon
* Hamburger menu doesn't work on mobile
* Strip unecessary code from prior build's hosting
