To configure your SAP system to send emails exclusively to a specific domain, follow these steps:

1. **Access SAPconnect Administration (Transaction SCOT):**
   - Log in to your SAP system and enter transaction code `SCOT` to open the SAPconnect administration interface.

2. **Configure the SMTP Node:**
   - In the SCOT interface, locate the existing SMTP node or create a new one by selecting the "Create Node" option.
   - Double-click on the SMTP node to open its settings.

3. **Set Supported Address Types:**
   - Within the SMTP node settings, click on the "Set" button next to "Supported address types" and choose "Internet."

4. **Define the Address Area:**
   - In the "Address area" field, specify the domain to which emails are allowed to be sent.
     - To restrict emails to a single domain, enter the domain in the format `*@yourdomain.com`. This configuration ensures that emails can only be sent to addresses within `yourdomain.com`.
     - If you wish to allow multiple specific domains, list each domain separated by commas, such as `*@domain1.com, *@domain2.com`.

5. **Save and Activate Settings:**
   - After specifying the allowed domain(s), save your changes.
   - Ensure that the SMTP node is active. An inactive node will be grayed out; activate it if necessary.

By implementing these configurations, your SAP system will be restricted to sending emails solely to the specified domain(s). This setup is particularly useful for controlling email communications and preventing unauthorized external email transmissions.
