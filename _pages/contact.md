---
title: "Contact"
permalink: "/contact.html"
---

# CryptoBuzz: Decentralised cryptocurrencies newspaper

The news are published every day automatically, using reddit as a source of information. An algorithm extract information and summarizes the content (using a transformers model) and statically generates the site with Jekyll.

## Decentralization of news

All news can be modified by changing the markdown on Github, make a pull request to update the articles.

----

<form action="https://formspree.io/{{site.email}}" method="POST">    
<p class="mb-4">Please send your message to {{site.name}}. We will reply as soon as possible!</p>
<div class="form-group row">
<div class="col-md-6">
<input class="form-control" type="text" name="name" placeholder="Name*" required>
</div>
<div class="col-md-6">
<input class="form-control" type="email" name="_replyto" placeholder="E-mail Address*" required>
</div>
</div>
<textarea rows="8" class="form-control mb-3" name="message" placeholder="Message*" required></textarea>    
<input class="btn btn-success" type="submit" value="Send">
</form>
