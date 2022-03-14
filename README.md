# Customer_segmentation
# Use Case

- Use Case Summary
- Objective Statement:
  * Get business insight about Revenue per member, Sessions per visitor, Average order value, Traffic, Visit per visitor and Add to cart rate (by country and by gender) per country in the first year of 2021.
  * To increase marketing efficiency by directing effort specifically toward the designated segment in a manner consistent with that segment’s characteristics.

- Methodology / Analytic Technique:
  * Descriptive analysis
  * Graph analysis
  * Segment Analysis

- Business Benefit:
  * Helping Business Development Team to create product differentiation based on the characteristic for each customer.
  * Know how to treat customer with specific criteria.

- Expected Outcome:
  * Know about Revenue per member, Sessions per visitor, Average order value, Traffic, Visit per visitor and Add to cart rate (by country and by gender)
  * Customer segmentation analysis.
  * Recommendation based on customer segmentation.

# Business Understanding

- Retail is the process of selling consumer goods to customers through multiple channels of distribution to earn a profit.
- This case has some business questions using the data:
- Revenue per member
- sessions per visitor
- Average order value
- Traffic
- Visit per visitor
- Add to cart rate (by country and by gender)

# Data Understanding

- Data of Retail Transaction from 01 January 2021 to 31 May 2021
- Data Dictionary:
- (1) Data: Transaction data from a fashion retail company in Canada.
    - orderId: Order (item) code.
    - MemberId: Member code.
    - id_discounted_order: 1 if the order is discounted.
    - Gross_revenue: Revenue of the order.
    - gross_revenue_before_discount	: Revenue before discount.
    - sum_units_sold: Number of nnits sold in the order.
    - sum_units_returned: Number of units returned in the order.
    

- (2) Data: Session data from a fashion retail website.
    - visitId: visiter unique code for each visit.
    - fullVisitorId: full visiter Code.
    - date: the date visitor visit the website.
    - memberId: Member code.
    - is_newsletter_subscriber: if the visitor is a newsletter subscriber.
    - newsletter_gender_communication_preference: gender predictions by newsletter.
    - country_from_ip: visitors come from Canada, US or other countries.
    - platform: visitors browse the website by website or iOS App
    - traffic_channel: affilliate, owned or paid for the traffic 
    - language_visit: lanuages used in the website.
    - orderId: order code if they have bought products.
    - sum_pdp_menswear_views: sum of "menswear" viewed.
    - sum_pdp_womenswear_views: sum of "womenswear" viewed.
    - sum_pdp_everythingelse_views: sum of "everythingelse" viewed.
    - sum_addtocart_menswear:sum of "menswear" added to cart.
    - sum_addtocart_womenswear: sum of "womenswear" added to cart.
    - sum_addtocart_everythingelse: sum of "everythingelse" added to cart.
    - sum_addtowishlist: sum of the products added to wishlist.

# Data Analysis

- Recency Frequency Monetary (RFM)

- RFM analysis allows you to segment customers by the frequency and value of purchases and identify those customers who spend the most money.

- Recency — how long it’s been since a customer bought something from us.
- Frequency — how often a customer buys from us.
- Monetary value — the total value of purchases a customer has made.

# Modeling Data: K-Means Clustering

K-Means clustering algorithm is an unsupervised machine learning algorithm that uses multiple iterations to segment the unlabeled data points into K different clusters in a way such that each data point belongs to only a single group that has similar properties.

# Result

- "Cluster 0" has 23% customers. It belongs to the "Loyal Customers" segment as they Haven’t purchased for some time, but used to purchase frequently (F=2) and spent a lot. (R=3, F=2, M=2)

- "Cluster 1" has 34% customers. It can be interpreted as "Alomost Lost". They purchase recently (R=2). However they do not purchase frequently and do not spent a lot. (R=2, F=3, M=3)

- "Cluster 2" has 23% customers. It can be interpreted as "Lost Cheap Customers". Their last purchase is long ago (R=4), purchased very few (F=4) and spent little (M=4). (R=4, F=4, M=4)

- "Cluster 3" has 19% customers. It belongs to the "Best Customers" segment which we saw earlier as they purchase recently (R=1), frequent buyers (F=1), and spent the most (M=1). (R=1, F=1, M=1)

# recommendations 

- Please see the attachment "one pager executive summary"
