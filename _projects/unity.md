---
layout: project
title: Unity
description: Make Unity Great Again
tagline: Make Unity Great Again
permalink: /showcase/unity/

published-time: 2020-08-19T17:47:06+00:00
last-modified: 2024-01-16T14:56:52+00:00

feature-image: assets/images/projects/unity/unity-feature.jpg
feature-width: 1200
feature-height: 675

showcase-video: https://www.youtube.com/watch?v=o35dfdO8WGQ
showcase-background: assets/images/projects/unity/unity-kingdom.jpg

header-image: assets/images/projects/unity/unity-kingdom.jpg
---

## Going Home

In 2019, I met [Ian Dundore]({{ site.data.linkedin.links.ian-dundore }}), a manager in Professional Services at Unity. I was working at inXile and needed to bring in some additional resources to help get [Wasteland 3]({{ site.url }}/showcase/wasteland-3/) across the finish line. I was on his radar; little did I know. This is where [Francisco Cruz]({{ site.data.linkedin.links.francisco-cruz }}), a friend and colleague from my time at OtherSide, enters the story. Since we crossed paths, Cisco had joined Unity’s M2/Gigaya team and had referred me to his team’s recruiter as a possible hire. Now I was in the system, and thus, Ian’s recruiter was able to strike.

Unity had played such an integral part in my professional life up until that point; having the opportunity to get my foot in the door and work on the impossible task of “making a magical button that converts Unreal projects to Unity” was a pretty easy sell as 2020 was winding down.

## Emerging Technology
Not long after our small, ambitious group started hitting milestones and blowing away executive leadership, Ian’s bet on hiring veteran game developers to create ECT was paying off. Yet, they had other plans for our evolving team at the end of 2021: take our **#gamedev** experience and work with studios to dogfood the engine (yes, we absorbed the legendary Spotlight team).

It was one hell of a ride! Meeting developers, working with them on their games, bringing back fixes, optimizations and features to Unity along the way. Yes, we were what the community would call a dogfooding team.

## Notable Contributions

Our team has done some fantastic work; here are just **some of the things** I have had a hand in landing during the course of working with different studios or on some random tangents that I remember.

- `Object.InstanstiateAsync` – An [optimization](https://docs.unity3d.com/2023.3/Documentation/ScriptReference/Object.InstantiateAsync.html) for spawning many [Objects](https://docs.unity3d.com/ScriptReference/Object.html) (yes [GameObjects](https://docs.unity3d.com/ScriptReference/GameObject.html)!) into a Scene that does not block the main thread. We then combined this work with some work in content streaming to make loading scenes at scale significantly less hitchy!
- `Object.Instantiate(Object,Scene)` – Because spawning directly into a [Scene](https://docs.unity3d.com/ScriptReference/SceneManagement.Scene.html) should be your decision.
- Tracking down and resolving the long-standing **MonoDomain Reload** hang – &#x2713; proud moment.
- The Play/Stop/Pause button change – It just makes more sense that way; MS Paint to the rescue.
- PlayMode Tooltips – Because designers deserve good UX.
- Project folder prefix in the title bar – Because developers can have multiple projects open, it’s a real thing.
- The **2×3 Layout** defaults to the 1-column project view – You’re welcome! This has bothered me since the 2-column **Project Browser** was introduced.
- Creating a retry system for failed licensing requests during batch mode – Because shit happens and your build shouldn’t fail.
- **Unity Style Cop** – An engineering base this size without an automated system of checks on source commits? Preposterous! While not everyone liked the changed workflow, it did promote incredible discussions and developer growth.
- Fixing up the **Package Manager** to understand standard licensing files – This was for [GDX]({{ site.url }}/showcase/gdx/), but it was a problem that needed fixing, I swear.
- Hero textures – Sometimes, you want textures that ignore all mipmap limits placed on them.
- Argument passing to child processes – so everything is cohesive.
- A warning when you change project serialization modes preventing accidental full reimports – which might take hours and make you just want to hard-stop for the day.
- `Debug.developerConsoleEnabled` – Disable the built-in developer console in any build, allowing for your own consoles to shine; or so you can use the fancy one in GDX and its author-time command palette (shameless plug).
- Variable Rate Update Groups in Entities – I loved seeing an entire [YouTube](https://www.youtube.com/watch?v=axUI016yb5U) video about this feature. I had added it because it just made sense for an ECS-based game.
- Finding and fixing leaks in the unleakable rewindable allocator – Never assume developer usage.
- Ability to track changes to externally referenced packages that live under the VCS workspace.
- Many PRs of performance optimizations across all engine segments (Editor, VFX, Rendering, Serialization, UI, Input, Audio, etc.) – Working with studios allowed us to find bottlenecks quickly and build solutions for them.

There are so many things that never shipped which I won’t get into, but you can only imagine the things that we have cooked up and all the things we could have done!

![Unity Credits](/assets/images/projects/unity/unity-credits.jpg)


It’s too bad Unity stopped showing its credits.