---
layout: "../../layouts/BlogPost.astro"
title: "Hel of possibilities!"
description: "Tas"
publishDate: "12 Sep 2021"
followMe:
  username: "bholmesdev"
  href: "https://twitter.com/bholmesdev"
halfTheMeaning: 21
heroImage:
  src: "/assets/blog/introducing-astro.jpg"
  alt: "Space shuttle leaving curved trail in the sky"

---

<FollowMe username={frontmatter.followMe.username} href={frontmatter.followMe.href} />

Access all exported properties with JSX expressions. For example, let's find the meaning of life: **{frontmatter.halfTheMeaning * 2}**

If this seems cool, consider giving my post a like with this Preact component: <LikeButton pageUrl={frontmatter.url} client:load />


