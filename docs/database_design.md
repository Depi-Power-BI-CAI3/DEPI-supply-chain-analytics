# Database Design

## Current Data Sources
- `supply_chain_data.csv` (see `/docs/data_dictionary.csv`)

## Conceptual Model (Entities)
- Product, Supplier, Order/Shipment, Carrier, Location, Inspection/Quality, Inventory Snapshot

## Proposed Star Schema
**Fact tables:**
- `fact_orders` (order_id, product_id, supplier_id, order_qty, unit_price, manufacturing_cost, shipping_cost, ship_date, delivery_date, carrier_id)

- `fact_inventory` (snapshot_date, product_id, stock_level, units_sold)

**Dimensions:**
- `dim_product` (product_id, product_type, category, brand)
- `dim_supplier` (supplier_id, name, location, lead_time)
- `dim_carrier` (carrier_id, name, transport_mode)
- `dim_date` (date_key, day, month, quarter, year)
- `dim_location` (location_id, country, city, region)

> Add an ERD diagram image export here and list PK/FK constraints.

## Data Modeling Notes
- Create calculated measures for: margin per unit, revenue by category, lead time (delivery_date − ship_date), defect rate.
