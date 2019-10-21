---
title: "Contact"
permalink: "/contact.html"
---

<form action="https://formspree.io/{{site.email}}" method="POST">    
<p class="mb-4">Hi, I am Tarun from Bengaluru, the Silicon valley of East. Apart from a thrilling job as Product manager, I am into DSLR photography, creative arts, psychology, tech ecosystem & boxing. 

If you are interested in any of this or just feeling bored in Bengaluru's amazing weather, feel free to <span><a target="_blank" href=" {{site.authors.tarun.linkedin}} " class="btn btn-outline-success btn-sm btn-round ml-1">Connect</a></span> or send a message below to {{site.name}}.</p>
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

