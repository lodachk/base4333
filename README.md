# base4333
Wallet Inflow vs Outflow Tracker
inflow = outflow = 0

for tx in block.transactions:
    if tx["to"] == wallet:
        inflow += tx["value"]
    if tx["from"] == wallet:
        outflow += tx["value"]

print("In:", inflow, "Out:", outflow)
