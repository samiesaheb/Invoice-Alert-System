# Invoice Alert System

A Python program to send an alert if a Proforma Invoice (PI) has not been received within 30 days of the order date.

## Features

- Extracts necessary information from an Excel file.
- Checks if the Proforma Invoice has been received within 30 days.
- Sends an email alert to the order coordinator if the invoice is overdue.

## Setup and Usage

1. Clone the repository:
   ```
   git clone https://github.com/your-username/Invoice-Alert-System.git
   ```

2. Install the required dependencies:
   ```
   pip install pandas openpyxl smtplib ssl
   ```

3. Add your Gmail account's app password and email addresses to the `config.json` file.

4. Run the program:
   ```
   jupyter notebook invoice_alert_system.ipynb
   ```

## Configuration

The configuration file `config.json` contains the following settings:

```json
{
  "sender_email": "your_email@gmail.com",
  "app_password": "abcdefghijklmnop",
  "receiver_email": "order_coordinator@example.com"
}
