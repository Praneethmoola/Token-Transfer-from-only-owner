# Token-Transfer-from-only-owner
One Person in Charge:
# The person who creates (deploys) the contract is the owner.
#  Only the owner can move (transfer) tokens to others. Keeps Track of Tokens:
 There’s a record (called balances) that shows how many tokens each person has. Initially, all the tokens belong to the owner.
# Sending Tokens:
 The owner can send tokens to someone else using the transfer function.Before sending, it checks,
 Does the owner have enough tokens?
If yes:
o The tokens are subtracted from the owner’s balance and added to the
recipient’s balance.
o A "transfer log" is created to keep a record of the transaction.
#  Recording Transfers:
Each time tokens are sent, a "receipt" (called an event) is logged, which shows:
o Who sent the tokens.
o Who received them.
o How many tokens were sent
