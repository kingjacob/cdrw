# CDRW

## Setup






## Process: 
1. “CD Buyer” deposits 100 DAI into a “Bank” for 1y.
2. If the "Bank" has a 1y rate for 5% th “Bank”  The bank effectively deposits 5 DAI worth of cDAI into an “escrow account”. The interest will be released to the “CD Buyer” at the end of the 1y.
If the “CD Buyer” wants to redeem their CD before the 1y is up, they will have to forfeit a portion of the interest earned. 
For example, if the CD Buyer wants to redeem his CD after 6m, he would normally be due 102.5 DAI, but might receive only 101.5 DAI instead, paying a 1 DAI penalty. 
This penalty can be set as a % of accrued interest. In the example above, a penalty of 13% of the 2.5 DAI of accrued interest is assessed (1 DAI/2.5 DAI = 40%). 
“Bank” deposits the 105 DAI into Compound to earn variable interest. 
“Bank” collects the difference between the variable interest it earns from Compound and the fixed interest that it pays to the “CD Buyer”. 
“Bank” makes money if the amount of interest it pays the CD Buyer is less than the amount of interest it earns from Compound on 105 DAI. 

## How to build this technically?
ERC721 to represent to CD. 
Build the “Bank” contract
Build the interface for the CD Buyer to buy a CD from the Bank

## What happens if there’s not enough money in the bank to support more interest?
Stop issuing CDs until more funds are deposited into the DAO that governs the bank. 

## What determines the rates you get? 
Currently multiple "banks" will submit rates via an onchain oracle


## How to interact with CDRW
1. Web interface
2. ENS Domain (deposit.eth) https://manager.ens.domains/name/deposit.eth



## Components of a CD



