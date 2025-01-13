---
layout: "../../layouts/BlogPost.astro"
title: "Learning Astro!"
description: "An example blog post with dynamic components in Astro."
publishDate: "13 Jan 2025"
followMe:
  username: "astro_dev"
  href: "https://twitter.com/astro_dev"
halfTheMeaning: 21
heroImage:
  src: "/assets/blog/learning-astro.jpg"
  alt: "Astronaut floating in space with a glowing keyboard"
setup: |
  import LikeButton from "../../components/LikeButton"
  import FollowMe from "../../components/FollowMe.astro"
  const { followMe, halfTheMeaning, url } = Astro.props;
---

# Welcome to Astro Blog Post!

This is a demonstration of how to integrate components and dynamic properties within an Astro blog post.

## Dynamic Data in Action

<FollowMe username={followMe.username} href={followMe.href} />

Here's a fun calculation: What's the meaning of life? **{halfTheMeaning * 2}**

## Interactive Component

If you like what you see, hit the like button below:

<LikeButton pageUrl={url} client:load />

## Hero Image

![{heroImage.alt}]({heroImage.src})

---

Feel free to tweak this as needed!
