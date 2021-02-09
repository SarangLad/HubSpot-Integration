# HubSpot-Integration
HubSpot API implementations


# Install Packages
- npm i request and npm i request promise
- Create "index.js"
- node index.js
- npm install express --save
- npm install axios


# HubSpot Link

Create a product
https://legacydocs.hubspot.com/docs/methods/products/create-product

Create Contact
https://legacydocs.hubspot.com/docs/methods/contacts/create_contact

Create Deals
https://legacydocs.hubspot.com/docs/methods/deals/create_deal

Associate CRM objects
https://legacydocs.hubspot.com/docs/methods/crm-associations/associate-objects

Get line_item_id for a specific product
https://community.hubspot.com/t5/APIs-Integrations/Get-line-item-id-for-a-specific-product/m-p/350073


# Step to map product with deald using line item

1. Create Product in HS library using Create a Product . Save the object ID returned from HubSpot at your end.
2. Create a deal and save the deal id at your end
3. Run line items api using Create Line Item . The hs_product_id here is the object id from 1st step. Save the line item object id returned in 202 response.
4. Run Associate CRM objects to associate line items and deals. Use 20 as definition ID to associate line item to deal.
