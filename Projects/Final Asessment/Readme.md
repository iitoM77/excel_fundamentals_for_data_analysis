#Final Assessment Task

all calculations done in Upload sheet
- In Column B create a TransactionReference that contains MERCHANT, SETTLEMENT DATE and MERCHANT REFERENCE from the BPAY Bank File Sheet
- in Column C extract the last 5 from BPAY Ref (column A) and modify BPAY Ref to remove the extra spaces so Column C is correct
- in column D extract the digit month from the corresponding paiddate in the BPAY sheet
- in column E convert the paiddate in BPAY sheet to a valid excel date
- in Column F get the payment amount from the BPAY sheet. Apply functions to remove the unwanted ("AU") and convert to a number
- edit Amount and Cust_Ref named ranges to in all the necessary data in the SYS DATA i.e. F2:F7624 (Amount) & C2:C7624
- create named ranges for all the other columns in the SYS DATA sheet. in the Upload sheet, calculate the total Amount (for SYS DATA) in T10, copy down the formula to T11 to calculate the total arrears_amt
- turn A1:Q69 into a table, turn on total row and add sum total in the balance column
- in Column H, use the Customer Reference to lookup the invoice date associated with fee_amt transactions for that customer from the SYS DATA sheet
- in column I, Use the data in columns E and H to calculate how many days there were between when the invoice was issued and when it was paid
- in column K identify the customers that paid early i.e. paid before date in column J. return Y if they paid early or leave it blank
- in column L calculate how many working days (excluding weekends) early payments were made. only customers who paid early should be included, others should have 0.
- in column M calculate customers that are eligible for discounts i.e. those that paid 5 working days or more before the due date (exclude weekends)
- in column N calculate the discount amount for eligible customers only. using the lookup table S2:T5
- in column O return the Discount offered for eligible customers and 0 for all others  
