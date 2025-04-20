# BlockBase_FEC
From Solidity feature and javascript i choose following feature:-

_Solidity-_
4.Get label of the last expense
Fetches the description of the most recently added expense.

_JavaScript-_
3.Show last expense label
Fetches and shows the description of the most recent expense added.

Used a bit similar feature to implement at both ends efficiently (at backend as well as frontend)
# Description 1 (solidity):
I added the getLastExpenseLabel function right after the existing function  getAmountPaid. This function will simply return the label of the last expense added, 
which can be obtained using the expenseCount variable.The expenseCount variable already tracks the number of expenses, so I used expenseCount - 1 to fetch the
last expense ,since arrays in Solidity are zero-indexed.
# Description 2 (java script):
"const lastExpense = expenses.length > 0 ? expenses[expenses.length - 1] : null;"
I added this logic to display the most recent (last) expense by accessing the last item in the expenses array.
Then,a helper function called calculateTotals was created to compute the total amount paid, total amount owed, and the number of participants involved 
