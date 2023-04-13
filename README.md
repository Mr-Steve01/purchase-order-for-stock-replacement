# purchase-order-for-stock-replacement
This problem requires some kind of input. You are free to implement any mechanism for feeding
input into your solution (for example, using hard coded data within a unit test). You should
provide sufficient evidence that your solution is complete, by indicating that it works correctly
against the supplied test data at least.
Problem
Your shop sells goods that you can buy from different suppliers. The selling price of each article is
fixed, but you should be able to buy that article from one supplier instead of another depending on
purchase price and discounts.
The discount percentage a supplier could offer can be related to the total order value, to the
ordered quantity or could be limited to a particular date/season.
When you need to order an article, you choose an item and the quantity you want to buy; the
system should find which suppliers do sell that article (check if enough quantity is available in
stock) and calculate the total purchase order amount applying the discounts (if available). The
result list should suggest the best supplier highlighting the cheapest one.
Also display the minimum days that each supplier needs to ship your order; this way you can
choose that a faster supplier is still better than a cheaper one.
EXAMPLE 1

Input:
12x Philips monitor 17”
● Supplier 1 has 8pcs in stock at 120€ each, and offers 5% discount for purchases of
minimum 1000€. Min. days to ship order is 5
● Supplier 2 has 15pcs in stock at 128€ each, and offers a 3% discount if you order >5pcs and
5% discount if you order >10pcs. Min. days to ship order is 7
● Supplier 3 has 23pcs in stock at 129€ each, and offers a discount of 5% for orders over
1000€. It also offers an additional discount of 2% for orders placed in september.. Min. days
to ship order is 4

Output:
● Supplier 1 is not prompted because it does not have enough stock quantity available.
● Supplier 2 can fulfill the request for 1’459.20€.
● Supplier 3 can fulfill the request for 1’441.19€; this is the cheapest one so it should be
highlighted
EXAMPLE 2

Input:
12x Philips monitor 17”
order date is november 2021
Output:
This time, Supplier 3 can fulfill the request for 1’470,60€ and so Supplier 2 should be highlighted as
it is the cheapest one; it should be highlighted even if Supplier 3 is faster (4 days instead of 7), as
you still decide where to buy
