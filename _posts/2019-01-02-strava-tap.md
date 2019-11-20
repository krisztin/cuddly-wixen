---
layout: post
img: https://res.cloudinary.com/du2vvjrb5/image/upload/v1574253223/krisztin/thumb-stravarec_hmuyff.png
title: 'Strava tap dance'
date: 2017-08-01 11:15:06 +0100
tags: [Strava, rant, app, a11y]
excerpt: '4 screens, 3 taps and more than 10 seconds from opening the app to the start of recording. Is that bad? Yes, yes it is.'
---

Let me paint you a picture here, a context of use if you will: I’m sitting on my bike, ready for an epic ride. But wait, _a ride does not happen if it’s not on Strava_. It’s kind of a tree falling in the woods thing amongst us cyclists. So I whip my phone out, all ready to roll I start what I not so affectionately call:

## “The Strava tap dance”

### Tap 0 - Opening the App

Not a premium member? Get ready to be prompted to sign up for a free trial that needs to be tapped close before you get to the opening screen below.

### Tap 1 - Tap the plus button

{% include imgout.html class="img--mobile" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574173906/krisztin/strava-step1_yxbyrt.png' alt="" caption="Record button? No?" %}

I would expect a quick record button on the opening screen somewhere close to the bottom right. Yes, you may want to record different kinds of activities; I'd Imagine there is a sizable cross-section of people using Strava and people tracking multiple sports/activities. In my case however, I only do cycling and my account is set up so that that is the default activity. **So why can't I just start recording my [insert default activity] with one tap?**

{% include imgout.html class="img--small" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574177742/krisztin/strava-step1t2_1_ekhbfl.png' alt="" caption="Bingo! Or is it?" %}

### Tap 2 - Tap the record button

{% include imgout.html class="img--small" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574178128/krisztin/strava-rec_pplwwz.png' alt="button with label: record activity" caption="Tap #2" %}

This is where the problem usually starts (unlike the recording of my ride). **Once you press the Record Activity button the next screen takes a bit to load**, by this time my brain immediately jumped to the conclusion that that’s it, we are recording and ready to go. Unfortunately, the load time is just slow enough that I have now locked the phone and put it away.

<small>My phone is a few years old and wasn’t high end even when I’ve bought it. It’s perfectly acceptable for everyday use, though.</small>

{% include imgout.html class="img--mobile" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574173906/krisztin/strava-step3_tdkcoh.png' alt="" caption="Screen #3 loads way too slow" %}

Not to mention this screen gets even more confusing. Notice the small recording icon in the notification bar?

{% include imgout.html class="img--small" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574173906/krisztin/strava-step3ab_t8uxgn.png' alt="" caption="Start? Stop? Which is it then?" %}

This clearly contradicts the button on the screen: one says **START** the other **STOP**. It really shouldn't be up there just yet.

### Tap 3 - Final tap to start

Once you've tapped START you get the final recording screen. Tired already? I am.

{% include imgout.html class="img--mobile" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574173906/krisztin/strava-step4_qgohx2.png' alt="" caption="The finish line" %}

#### Cold context

I am one of those insane people who ride when it’s cold outside. My winter gloves are as “screen-friendly” as they can be, which means 1 tap often becomes 5 before it finally registers, hence the more steps the more taps until I’ve had enough of wildly fingering my phone and rip off my gloves. The end result: frozen hand, recording started, doing some additional gymnastics to put the glove back on which is an artform in sub-zero temperatures.

#### Accessibility note

It takes at least 10 seconds from tapping on the app to recording. In comparison, it takes less than 5s to start Spotify, find my favourite playlist and hit play. And yes, optimising an app’s loading time is part of accessibility: not everyone has the latest phones and superfast 4G connections.

## How to cut down on taps?

My solution would be using the _default activity_ setting you can choose for your account. By introducing a _Quick Record_ button that immediately starts recording your default activity. In case you do want to switch you can do so by

{% include imgout.html class="img--small" url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574243936/krisztin/strava-stepbtnchange_uozrox.png' alt="" caption="Turn 3 taps to 1" %}

### User flow

With _default activity_ set.

{% include imgout.html url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574243868/krisztin/strava-flowold_co1fa6.png' alt="" caption='Old "flow"' %}

To record your _default activity_:

- 3 taps

{% include imgout.html url='https://res.cloudinary.com/du2vvjrb5/image/upload/v1574243907/krisztin/strava-flownew_zsm1hb.png' alt="" caption='New flow' %}

To record your _default activity_:

- 1 tap

From a **technical perspective**, I recognise this would introduce the question of when to acquire the GPS co-ordinates which in the current flow happens on the _Record Activity_ screen. I have recently watched a video on introducing Machine Learning into UX which in this context would be for the app to learn when the user usually records activities and if the app is switched on around those times then it would automatically fetch GPS data on load.
