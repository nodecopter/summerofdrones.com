<%
this.layout = 'default';
this.title = 'Budget';
%>

<h2 id="budget"><a href="#budget">Budget</a></h2>

There are essentially only three big items that you need to budget for:

* [Venue](#venue) (0 - 5000 USD)
* [Drinks and lunch](#drinks-and-lunch) (25 - 50 USD / person)
* [Shipping](#shipping) (~300 USD)

Additionally you should add an extra ~15% to your budget for overhead:

* Unexpected problems
* Power splitters
* Extra drinks for visitors in the evening
* etc.

If you want a quick estimate, check our [example budget](#example).

<h3 id="venue"><a href="#venue">Venue</a></h3>

Ideally you can find a local company to provide a [nice venue](/compass/venue)
for free.

If you cannot find a free venue, you should:

* Look at many different venues and compare prices
* Be prepared to spend between 0 USD and 5000 USD
* Try to get a discount for doing something amazing

Some venues may also like the idea of people taking photos & videos of their
venue from positions & angles that are only reachable with the drones.

<h3 id="drinks-and-lunch"><a href="#drinks-and-lunch">Drinks and lunch</a></h3>

To let people focus on programming the drones, you should provide drinks
(water, soft drinks, maybe beer in the evening) and lunch. You can do this in one of two ways:

* Buy food & drinks from the venue: This will most likely be more expensive,
  but it easier to coordinate and some venues will require it.
* **Recommended:** Buy drinks & order delivery food yourself: This is
  cheaper and more flexible, but requires a little more work.

<h3 id="shipping"><a href="#shipping">Shipping</a></h3>

We require you to ship your drone set (20 drones) to the organizer of the even that takes place <strong>two weeks after your event</strong>. You can calculate this to be around 10 - 15 USD per drone, so around 300 USD altogether.


<h3 id="example"><a href="#example-budget">Example Budget</a></h3>

<%
var people = 40;
var drones = 20;
var shippingPricePerDrone = 15;
var venueCost = 2000;
var visitors = people * 0.4;

var currency = 'USD';
var items = [
  {
    name: 'Lunch',
    amount: people,
    price: 15
  },
  {
    name: 'Drinks',
    amount: people + visitors,
    price: 15,
    comment: people + ' attendees plus ' + visitors + ' visitors'
  },
  {
    name: 'Shipping',
    amount: drones,
    price: shippingPricePerDrone,
    comment: 'for 20 drones'
  },
  {
    name: 'Venue',
    amount: 1,
    price: venueCost
  },
];

var total = 0;
%>

Here is an example calculation for an event with <%= people %> people:

<%-
items.map(function(item) {
  var subTotal = item.amount * item.price;
  total += subTotal;
  var line =
    '* **' + item.name + ':** ' + item.amount + ' x ' + item.price + ' ' +
    currency + ' = **' + subTotal + ' ' + currency + '**';

  if (item.comment) {
    line += ' (' +  item.comment + ')';
  }

  return line;
}).join('\n')
%>
<%
var overhead = total * 0.15;
%>

**Total:** <%= total + ' ' + currency %> (hard costs) + <%= overhead + ' ' +
currency %> (15% overhead) = **<%= (total + overhead) + ' ' + currency %>**

This is just an example, but **3500 USD - 5000 USD** is a reasonable ball
bark for most "Summer of Drones" events.

But don't be scared, on the [finacing page](/compass/financing) you will find some advice on how you can pull this off.
