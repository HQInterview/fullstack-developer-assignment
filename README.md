# Fullstack developer assignment

The system you are about to develop is intended to handle bids on hotel auction.

Company RoomsQuickly organizes auction on top hotels luxury rooms once a month. Amount of unique rooms is usually around a few hundred thousands across the globe.

RoomsQuickly has hundred of partners willing to participate and post bids: website, mobile application, off-line auction. CTO of the company managed to agree with all partners to send bids in Thai Baht only. Same time he promises partners to handle high load with excellent performance that’s why he expects the system to be able to scale horizontally.

**Partners should be able to:**

* request list of active auction items (items which are able to accept bids)
* post a bid and get success/failure response back
* request information whether or not the bid is a winner by unique bid_id

**Business rules:**

* Partners bid on unique rooms
* Rooms should be returned in list of auctionable rooms ordered by time remaining for bidding
* Each room has minimal allowed bid
* Bid with higher price wins 
  * If new price is greater than old one by 5%
* Each room is opened for bids for 10 minutes
  * If new bid is received less than 1 minute from the end of room auction then auction time is automatically extend by 1 minute (to prevent bidding in last seconds with anyone else being able to overbid)

## Frontend requirements

Develop a web page which shows active auction items with winning bids. Make the list real time with no page refresh.

Please use React.js for the page.


## Areas we would be evaluating
* Is there documentation?
* Code style
* language/platform features utilization
* project structure (file/folder organization)
* architecture (components, areas of responsibility)
* complexity (easier to understand code is better)
* unit/integration/end2end tests
* resolution for all challenges



