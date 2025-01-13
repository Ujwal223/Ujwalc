---
layout: "../../layouts/BlogPost.astro"
title: "Test!"
description: "Ts"
publishDate: "12 Sep 2021"
followMe:
  username: "bholmesdev"
  href: "https://twitter.com/bholmesdev"
halfTheMeaning: 21
heroImage:
  src: "/assets/blog/introducing-astro.jpg"
  alt: "Space shuttle leaving curved trail in the sky"
setup: |
  import LikeButton from "../../components/LikeButton"
  import FollowMe from "../../components/FollowMe.astro"
  const { followMe, halfTheMeaning, url } = Astro.props;
---

<FollowMe username={followMe.username} href={followMe.href} />

Access all exported properties with JSX expressions. For example, let's find the meaning of life: **{halfTheMeaning * 2}**

If this seems cool, consider giving my post a like with this Preact component: <LikeButton pageUrl={url} client:load />
