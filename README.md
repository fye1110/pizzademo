## BUILD AND RUN

```bash
  npm i
```
```bash
  npm run start
```
```bash
  npm run test
```

## UI DESIGN:
- Identify the customer
- Input product
- Output price based on the additional pricing rule

## PRICING DESIGN:
#### The idea is that each customer can add multiple pricing rules, so one order can apply multiple rules
#### Pricing logic should be calculated in the Backend and will be called through an API with a payload of (customer, items, payment type, etc.)
#### In the scope of an assessment, pricing logic is implemented at the Front end, and one special customer only has one pricing rule
- Currently, there are two types of pricing rules, which are GET_MORE and DROP
- GET_MORE means the customer receives more product when they pay for a quantity of product
- DROP means the customer can have a special price on a product

#### Main business logic is located in /hook/usePricing.ts