---
title: Post View Counter Info
description: "What's this weird request my browser makes when I read stuff?"
permalink: /blog/postviewcounter
hidden: true
---

`viewcounter.trobinson.me` is used to count the views of each blog post. When you scroll a certain amount into the post, the view counter is incremented for whichever post you were reading. When the post loads, it also makes a request to this subdomain in order to show the current view count.

To discourage spam and illegitimate views being added, there's a short ratelimit implemented that works based on IP address. Don't worry, I knock off the last octet (last few digits), so there's no way I can identify you, the posts you visit or anything else.

---

**To Devs:**  
Found a security issue with my awful PHP? I want to know! Please click contact in the menu and get in touch.