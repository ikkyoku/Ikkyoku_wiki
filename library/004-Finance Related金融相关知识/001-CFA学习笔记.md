
# *CFA学习笔记*

## Contents
- [Contents](#contents)
- [Ethical and Professional Standards](#ethical-and-professional-standards)
- [Quantitative Methods](#quantitative-methods)
- [Corporate Finance](#corporate-finance)
- [Fixed Income](#fixed-income)


## Ethical and Professional Standards

## Quantitative Methods

### 1. Time value of money

Nominal risk-free rate = real risk-free rate + expected inflation rate

Required interest rate on a security = nominal risk-free rate + default risk premium + liquidity premium + maturity risk premium

EAR (Effective annual rate) = (1+ stated annual rate/m)^m -1

Continurous compounding:

e^r - 1 = EAR

r = ln(EAR + 1)

Future value (interest) factor: 

(1 + I/Y)^N

### 2. Discounted cash flow applications

HPR (Holding period return)= (ending value + cash flow received)/beginning value + 1

Money-weighted rate of return: IRR of the cash flow

Time-weighted rate of return = [(1+HPR1)*(1+HPR2)...]^1/n-1

It is the geometric mean return.

BDY (Bank discount yield): (D/F)*(360/t)

- D = face value - purchase value
- F = face value
- t= days remaining until maturity

HPY (Holding period yield)=(P1 + D1)/P0 - 1

EAY (Effective annual yield)= (1+HPY)^365/n - 1

**Money market yield (CD equivalent yield): rMM = HPY * (360/t) = 360 * BDY/(360 - t * BDY)**

Bond equivalent yield = 2* semiannual discount rate = [(1+EAY)^0.5-1]*2

### 3. Statistical concepts and market returns


The sharp ratio = (rp-rf)/σp

### 4. Probability concepts

Bayes' formula

### 5. Common probability distributions

Monte carlo simulation

Historical simulation

### 6. Sample amd estimation

Time-series data
Cross-sectional data
Longitudinal data
Panel data

Central limit theorem

Bias:

- Data mining bias
- Sample selection bias
- Survivorship bias
- Look-ahead bias
- Time-period bias


### 7. Hypothesis testing

### 8. Technical analysis



## Corporate Finance

## Fixed Income

### 1. Bond prices, yields, and ratings

#### 1.1 Feature of a fixed-income security

- Issuer of the bond
- Maturity date of the bond
- Par value
- Coupon rate and frequency
- Currency

##### 1.1.1 Issuer of Bond
- Corporations
- Sovereign national governments(U.S. and other countries)
- Nonsorvereign governments(State or city)
- Quasi-government entities(Freddy and Fannie)
- Supranational entities

##### 1.1.2 Bond Maturities
Term to maturity(tenor): the remaining time until maturity

Perpetual bonds: bonds with no maturity date

Money market securities: YTM <=1yr

Capital market securities: YTM >1yr

##### 1.1.3 Par Value

Principle repaid at maturity

- Premium: Price > Par

- At par: Price = Par

- Discount: Price < Par

##### 1.1.4 Coupon Payments

Conventional bond (Plain vanilla): A bond with a fixed coupon rate

Zero-coupon bonds (pure discount bonds): Bonds paying no interests prior to maturity

##### 1.1.5 Currencies
Dual-currency bond: Bond with coupon interest in one currency and principle in another

Currency option bond: Bond with a choice for bondholders to decide which currency tehy want to receive

#### 1.2 Bond indenture

Trust deed(bond indenture契约): legal contract between the bond issuer and bondholders

Covenants(契约): Provisions in the bond indenture

- Negative covenants:restrictions on asset sales, negative pledge of collateral, restrictions on additional borrowings

保护债券持有人，保证债券违约率不提高

- Affirmative covenants: no restrictions on issuer's operating decision

#### 1.3 Issuance and trading of fixed-income securities

Bond Issue country:

Domestic Bonds: Domestic company, currency, market

Foreign Bonds: Foreign company, domestic currency, market

- Panda bonds
- Yankee bonds
- Samurai bonds

Eurobonds: A company, B currency， C market

Global bonds: A company, B currency， C market, trade in D market

- Bearer bond: ownership of bonds by possessing the bonds
- Registered bonds:ownership of bonds is recorded

Legal and regulatory issues in a trust:

- Legal information about the entity
-  Assets pledged for repayment
-  Additional features increasing the repayment probability
-  Covenants including actions to take and prohibited from taking

##### 1.3.1 Issuing Entities

Treasury of the country -> sovereign bonds

Well-known corporation -> corporate bonds

Special purpose entities(in U.S.)/vehicles(in Europe)(called bankruptcy remote vehicles) -> securitized bonds

SPE可以比相同的公司债发行更低的利率，因为SPE持有资产，即使公司破产了也能支付。

##### 1.3.2 Sources of Repayment

Sovereign bonds <- tax receipts of the country

Non sovereign bonds <- general taxes, revenues of projects(airports), special taxes or fees

Corporate bonds <- cash from firm's operations

Securitized bonds <- cash flow from the financial assets by SPE

##### 1.3.3 Collateral and Credit Enhancements

Collateral: assets pledged to support a bond issue

Unsecured bonds: bonds with no collateral

Secured bonds: bonds with collateral

Secured bonds 因为有collateral降低了违约风险，所以收益率降低

破产或者变现资产时，顺序为：Secured bonds, senior unsecured debt, subordinated/junior debt

Secured debt type:

- Equipment trust certificates: backed by equipment like railroad cars and oil drilling rigs
- Collateral trust bonds: backed by financial assets like stocks and bonds

Debenture 在英国和某些国家指有特定资产抵押的债券，在美国和其他国家指无抵押债券

Securitized bond 最常见是MBS，mortgage-backed security

Covered bonds类似于MBS，底层资产存于发行公司报表上（区别于SPE)

Credit enhancement: internal or external

Internal methods:

- overcollateralization
- cash reserve fund 
- excess spread account
- bond division into tranches

External methods:

- surety bonds
- bank guarantees
- letter of credit

#### 1.4 Taxation of Bond Income


Bonds issued by municipal governments in the U.S. exempt from income tax











<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2MTA4MDgzOTldfQ==
-->