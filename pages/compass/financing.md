<%
this.layout = 'default';
this.title = 'Financing';
%>


<h2 id="financing"><a href="#financing">Financing</a></h2>

<h3 id="finding-sponsors"><a href="#finding-sponsors">Finding sponsors</a></h3>

If you can find enough sponsors to cover all your costs, that would be truly awesome. From our experience it is best to contact local tech companies for this. Many are more than willing to help out with such an awesome event - you just need to contact them.

Most of the time they will even send a few people to the event as well, which in turn helps you get the required amount of attendees.

Unfortunately sponsors do not get to keep the drones after the events this time. Instead we are thinking about donating them to [CoderDojo](http://coderdojo.com) to help raise the next generation of software developers.

However, you can offer your sponsors different things they get in return - like banners, naming the venue's Wifi connection, sponsoring the food, etc. If you need help finding sponsors, you can always drop us a line at [core@nodecopter.com](core@nodecopter.com).


<h3 id="selling-tickets"><a href="#selling-tickets">Selling tickets</a></h3>

If you can't find enough sponsors to cover all your costs, then that's not a problem at all. You can sell tickets instead. A good ticket price would be between 20 and 30 USD. After all we want to make this less expensive, but more epic for the attendees.

<%
var people = 40;
var ticketPrice = 30;
var currency = 'USD';
var total = ticketPrice * people;
%>

With <%= people %> showing up at the event and a ticket price of <%= ticketPrice + ' ' + currency %>, you can raise <%= total + ' ' + currency %>, which should be between 30% and 50% of what you need to raise.

You are free to sell tickets however you like. We recommend using services like [Eventbrite](http://www.eventbrite.com/) to make selling tickets a breeze and to receive the money upfront.

<h3 id="ways-for-money"><a href="#ways-for-money">Other ways to raise money</a></h3>

If you can't or don't want to raise money via sponsors or selling tickets, that's fine. This is your event and you are free to raise money for it in whichever way you like.

However, in order to ensure that everything is in sync with the spirit of and the idea behind the "Summer of Drones", please drop us a line at [core@nodecopter.com](core@nodecopter.com) before you execute your fundraising idea.
