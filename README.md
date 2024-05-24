HTML Form:

Added a delivery date picker that validates the selected date to ensure it's a Saturday or Sunday.
Added hidden input fields for SKUs.
Added a script to check the SKU count limits before submitting the form.
Google Apps Script:

doPost function now includes delivery date and SKU count checking.
Added getSKUCounts function to get the current SKU counts for the week.
Modified the sendConfirmationEmail function to include the delivery date and hide items with zero quantity.
SKU Count Check:

Before submitting the form, it checks the current SKU counts to ensure the weekly limit is not exceeded. If it is, it returns an error message.
This setup ensures that the delivery date is validated, SKUs are accounted for, and the order respects the SKU limits for the week.
