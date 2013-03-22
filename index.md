---
layout: default
title: The Summer of Drones
---

<h2 id="about">The Summer of Drones</h2>

The Summer of Drones is an epic series of up to 34
[Nodecopter](http://nodecopter.com/) community events to take place in North
America and Europe from June to September 2013.

Our goal is to highlight the non-military potential of
[UAVs](http://en.wikipedia.org/wiki/Unmanned_aerial_vehicle), bring together
people from different programming communities, and learn some interesting new
stuff while having fun with flying robots.

Have a look at some videos from the first Nodecopter event that was held in
Berlin on Oct 5th, 2012 to get an idea for what to expect:

<iframe width="345" height="194" src="http://www.youtube.com/embed/gucpgJEJ5b4" frameborder="0"></iframe>
<iframe width="345" height="194" src="http://www.youtube.com/embed/t13jGeBAWrA" frameborder="0"></iframe>

A lot more Nodecopter videos can be found with this [YouTube Search](http://www.youtube.com/results?search_query=nodecopter).

<h2 id="attend">Attend an Event</h2>

You know JavaScript, Ruby, Python, Java, Objective C, C++, C#, Perl, Go, Clojure,
or Scale? Heck, even Bash will do.

As long as your language of choice can do networking, you should consider
attending an event close to you. There is also no need for previous robotics
experience as long as you are passionate and curious!

We are going to announce the first dates and cities very soon, so make sure
to get notified:

<form class="form-search" action="http://nodecopter.createsend.com/t/j/s/irhtuj/" method="post" id="subForm">
  <input class="email" placeholder="email@example.com" type="text" name="cm-irhtuj-irhtuj" id="irhtuj-irhtuj">
  <input class="btn" type="submit" value="Keep me posted">
</form>

<h2 id="organize">Organize an Event</h2>

The Summer of Drones is a community project, this means anybody who is
passionate about flying robots and their local community can bring an event to
their city!

We'll take care of the drones, you take care of the rest.

Sounds interesting? Head over to the [Organizer Page](/organize.html) to find
out more!

<h2 id="sponsor">Sponsor</h2>

The summer of drones will see some of the best and most passionate web and
mobile developers come together to push the boundaries of their tools further
than ever before, and we want you there as a sponsor!

[Contact us for details!](mailto:sponsor@nodecopter.com)

<h2 id="blog">Blog</h2>

<section class="content">
  <ul class="listing">
    {% for post in site.posts %}
<li>
  <span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="{{ post.url }}">{{ post.title }}</a>
</li>
    {% endfor %}
  </ul>
</section>
