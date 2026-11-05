# Warehouse tools

Small Python utilities for warehouse order and shipping workflows.

Run the tests with `python3 -m unittest discover -s tests -v`.

## Shipping

`shipping_quote(weight_kg, zone)` returns a standard delivery quote. Zones are
`local` and `regional`; weights must be positive. Quotes use a $4 local or
$8 regional base rate plus $1.50 per kilogram, rounded to two decimal places. The command-line entry point
prints a quote for an order.
