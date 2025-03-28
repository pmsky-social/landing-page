---
layout: '../../layouts/Blogpost.astro'
title: 'The App is Live!'
pubDate: 2025-02-23
description: 'Announcing the launch of the PMsky platform'
author: '@drewmca.dev'
# image:
#     url: 'https://docs.astro.build/assets/rose.webp'
#     alt: 'The Astro logo on a dark background with a pink glow.'
tags: ["launch", "pmsky.social", "peer moderation", "bsky", "atproto"]
---
## We're live!
The main voting platform for pmsky is now live, at [app.pmsky.social](https://app.pmsky.social)!

The source code is also available on the organization's GitHub [here](https://github.com/pmsky-social/app).  We'd love any feedback you have, and you can submit them as GitHub issues, emails, Bluesky DMs, or the form linked in the docs [here](https://docs.pmsky.social/getting-started/provide-feedback).

### Check out the app!  
You can currently propose a label, of which there are [three allowed](https://github.com/pmsky-social/app/blob/cba37c716d5dc99527f23cf3627b2918d91873fa/src/routes/proposals.ts#L7): `wholesome`, `helpful`, and `banger`.  In the future, you'll also be able to help decide which additional labels can be proposed on posts via a "meta-proposal" to allow a new label.  

So far, the only meta-proposal enabled is whitelisting users.  This means you're able to invite other users by proposing they be whitelisted, and then upvoting that proposal.  

Logging into the app is restricted to "whitelisted" users ([code](https://github.com/pmsky-social/app/blob/cba37c716d5dc99527f23cf3627b2918d91873fa/src/routes/login.ts#L69)).  A user is whitelisted if the proposal to whitelist them has a positive score (i.e. more upvotes than downvotes) ([code](https://github.com/pmsky-social/app/blob/cba37c716d5dc99527f23cf3627b2918d91873fa/src/db/repos/allowedUsersRepository.ts#L9)).  

If you aren't on the whitelist yet, you can request access [here](https://docs.pmsky.social/getting-started/request-access), or you can ask an existing user to propose whitelisting you!

### Next steps
There are a few steps to take next.  I'd like to build a simple labeler to publish the labels you're currently able to propose and vote on, as well as one that publishes a label indicating that the post is getting attention over on pmsky.  The ability to propose more labels is also on the horizon, plus a whole host of usability bits to develop.  

What's being released right now is the bare minimum, but I would love to have folks trying it out, giving feedback on usability bugs (are there things that don't work, or don't work how you'd expect them to?) as well as any thoughts around how this might be useful to you and your communities, and how you see this being used to improve your experience on Bluesky.

Thank you for reading; I'll see you in the atmosphere!

<a class="homelink" href="/"><i>back to home</i></a>