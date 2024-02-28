---
title: Xero Integration
description: Streamline your catering business's financial processes by connecting Puree to Xero. This guide walks you through the setup and use of integrating Puree with Xero.
---

Xero is cloud-based accounting software platform used by individuals as well as small and medium sized businesses.

{% include callout.html text="We hope this guide helps you make the most out of Puree's Xero integration. If you have any questions or need further assistance, don't hesitate to reach out." %}

## How we work together

Puree.app integrates with Xero to provide a seamless solution between order management and order accounting.
Quotes or orders created in Puree can be synced with Xero.

## How Puree + Xero works

### Generate tax invoices for your customers

When you connect to Xero, you will have the option to link orders to Xero. This will create an invoice in Xero, with
a summary of the various item categories rolled up into line items.

Invoices can be linked to existing customers you have setup in Xero, or Puree gives the option of creating new customer
records directly in Xero.

## Before you begin

{% include callout.html text="These instructions assume that you have a Xero subscription. If you haven't signed up
with Xero yet, you can sign up for a free trial." %}

In your Xero chart of accounts you need to have an account setup to receive Sales at a minimum.

## Setting up Xero synchronisation in Puree

1. Click on the "Menu" slider in the top right corner.
1. Click "Integrations"
1. Click "Connect to Xero". This will direct you to log into your Xero account and authorise access to Puree. You'll be
   redirected back to Puree when you're finished.
1. Setup your Puree settings:
    - map categories of items to the appropriate account from your Xero organisation's chart of accounts:
      - Menu
      - Beverages
      - Equipment
      - Miscellaneous
      - Staff
      - Delivery
      - Venues (if you have the venues add-on enabled)
    - Select "auto sync" with Xero if you want changes to orders to be
      automatically sent to Xero
    - Choose the default number of days before a Xero invoice is due
1. Click "save" to complete your Xero integration setup.

## Linking orders with Xero

To start linking orders with Xero, navigate to the Quotes index page. If you
have setup your Xero integration, you will now see an invoicing section, with
"Link to Xero" buttons for each quote.

1. Click the "Link to Xero" button for quotes you want to send to Xero.
1. You can either create a new contact in Xero, or select an existing Xero contact.
    - The list of Xero contacts is regularly updated with your contacts from Xero.
1. Select the date you want the Xero invoice to be due. It will default to the order date
   plus the configured number of days before the invoice is due.
1. Click save, and you will receive a message notifying that the sync was successful, along
   with a link if you want to immediately view the invoice in Xero.

{% include callout.html text="Note that Xero invoices will use your default tax settings based on the Tax Information in the Account Details page. For example, if you have configured sales tax 'GST' at 15.0%, that will flow through to the Xero invoice." %}

## Background syncing

{% include callout.html text="To enable background syncing select 'auto sync with Xero' on the Xero settings page. If this option is not enabled, changes to orders have to be manually synced via the 're-sync to Xero' button." %}

Once an order is linked with Xero, any subsequent changes within Puree will automatically
be synced to Xero. Note that this is a one-way sync only. Changes made in Xero will not be reflected in Puree.

### Error Handling

There are various scenarios that could cause an invoice to fail to sync to Xero. For example:
- The contact associated with the invoice has been archived
- The associated invoice was deleted or archived in Xero
- There was a network error or outage at the time the sync was attempted.

In these cases, Puree will notify you of the relevant error to allow action to be taken.

#### Background errors

If the invoice was initially successfully created in Xero, but a subsequent update fails,
you will be notified via two mechanisms:
- A notification that the order update failed.
- By viewing the details of the failure on the integration sync history page.

The Integration sync history page shows a log of synced records, along with errors for any
that failed. Once you have rectified any errors, you can use the "retry" function to attempt
to sync the order with Xero again.

Examples of corrective action might be:
- Restoring an archived contact
- Restoring a deleted or archived invoice
- Simply retrying an order that failed due to network issues.

## Connection Refresh

After a period of time you may need to refresh your connection with Xero. In this case Puree
will notify you via two mechanisms:
- A notification that the connection with Xero is broken
- When viewing the integrations page, the Xero connection will show as needing to be
  refreshed.

Clicking the "Re-authenticate with Xero" button will allow you to go through the Xero
authentication flow again, restoring the connection.

Attempting to push any data to Xero with the connection broken will result in redirection
to the integrations page, with a notice indicating the connection needs to be restored.

For further assistance, please contact Puree support.

## Watch Our Tutorial on the Venue feature in Puree

<!-- Loom Video Below -->
{% include video_embed.html id="b75d20e2df0d48c29a3f97198bda441d" %}
<br>
