---
title: How I Turned Our Old Tablet Into a Math-Only Tablet (No YouTube, No Games)
slug: math-only-ai-tablet-for-kids
date: 2026-11-06
draft: false
description: Turn a spare Android tablet into a free, math-only study station
  for kids up to 11 using Google AI Studio and Fully Kiosk Browser.
image: /img/math-only-tablet-for-kids.jpg
image_alt: A boy solving a fraction problem on an Android tablet while a
  friendly robot tutor sits beside him.
author: Mr Wnow
tags:
  - EdTech
  - AI
  - Parenting
  - Android
  - Tutorial
categories:
  - AI
  - Mathematics
  - Technology
  - Learning Tips
sources:
  - name: Own experience with Google AI Studio and Fully Kiosk Browser. Gemini assist
---
I gave my kid our old tablet last month. Big mistake.
Within five minutes he was on YouTube. Then a game. Then he was asking the AI about Minecraft.
So I set out to build a tablet that does one thing: math. For kids up to 11 years old. It took me two tries. The first time, I locked myself out. The second time, it worked.
Here is what finally worked. A parent does the setup. Your kid just uses it.
### What it does, in simple words
Your kid opens the tablet and sees one teacher. Only math.
• He asks: "What is 3/4 + 1/8?" The teacher helps him step by step.
• He asks: "Tell me about Minecraft." The teacher says: "Nope, math only."
If he tries to leave, the tablet brings him straight back, like a boomerang. And best of all, it costs nothing.
### Before you start
Use YOUR Google account, not your kid's. Google requires account holders to be 18 or older to access AI Studio. Your kid never logs in.
What you need:
• Your computer
• Your Google password
• An old Android tablet (ours was just lying in a drawer)
• A PIN that is NOT 1234. Pick one your kid will never guess, and write it on paper, not on the tablet!
### Step 1: Make the teacher (Google AI Studio)
1. On your computer browser, go to aistudio.google.com.
2. Click Create new prompt, then select Chat prompt.
3. In the right-hand panel, pick Gemini 3.8 Flash. It is fast and free to use.
4. Set the Thinking Level to Low (or lower the Temperature to 0.2). This just tells the AI: "Don't be silly, be steady."
5. Turn OFF all Tools (Search, Maps, Code, etc.). We don't want the teacher wandering off to Google things.
6. Paste the rule book into the System instructions box. You can customize it however you like. Tell Gemini what you need and it will draft rules for you. An example is below, and my full custom prompt is at the bottom of this post.
Example instruction:
You are a Math Teacher for kids up to 6th grade. First, check: is this question about math? If it is not math, do NOT answer it. Just say: "I am strictly your math tutor! I can only help you with studying mathematics. Let's get back to math." Teach like you are talking to a 10-year-old using pizza, toys, and blocks. Break big problems into small steps. End with ONE practice problem.
7. Click Save at the top right and name it Kids Math Tutor. (I forgot to press Save the first time. Don't be like me.)
8. Once saved, look at your browser's address bar. The link changes to include a unique ID, like https://aistudio.google.com/prompts/YOUR_ID. Copy this link and save it in your notes. That link is your teacher's home.
Good to know: If you edit your system instructions later and click Save, the link does NOT change. To apply the new rules on the tablet, just restart Fully Kiosk.
9. Test it: Ask: "What is 3/4 + 1/8?" Then ask: "Tell me a joke." The second one should get a "math only" answer. If it tells you a joke, your rules did not save!
### Step 2: Lock down the tablet (Fully Kiosk)
This is the part I messed up the first time, so follow the order carefully!
1. On the old Android tablet, open the Play Store and install Fully Kiosk Browser & Launcher.
2. Open Fully Kiosk and swipe in from the left to open Settings.
3. Go to Web Content Settings → Start URL and paste your teacher's saved workspace link.
4. Go back to the main browser screen and sign in with YOUR Google account NOW. (Crucial tip: on my first try I set the whitelist first. It blocked Google's login page and locked me out! Save the whitelist step for last.)
5. Now return to Settings → Web Content Settings → URL Whitelist. Type your workspace link with an asterisk at the very end, like this: https://aistudio.google.com/prompts/YOUR_ID*. (In my test, the free version of Fully Kiosk showed a small watermark once I enabled a few options, such as the whitelist. You can buy the full license if you want to remove it.)
6. Checkmark Reload Start URL on Block. This is the magic button! If your kid clicks an external link or tries to navigate away, the tablet instantly bounces back to math.
7. Go to Kiosk Mode in Settings, set your 4-digit PIN, and turn Kiosk Mode ON. Lock the status bar pull-down and the home button. (Pro tip: use the search bar at the top of Fully Kiosk's settings to find these toggles quickly.)
8. Press the tablet's Home button, select Fully Kiosk, and tap Always.
Honest note: I did not test Fully Kiosk's Kiosk Mode lock myself. My own tablet is already locked down with NetGuard's lockdown mode, which blocks all internet except the Fully Kiosk app. So I can't promise exactly how steps 7 and 8 behave on your tablet. Run the test below before handing it over, and keep your PIN handy.
Done!
### Test it like a kid would
Before handing it over, try to break it:
• Restart the tablet: Does the math tutor open automatically? (It should.)
• Swipe everywhere: Can you pull down notifications or exit to Home? (You shouldn't be able to.)
• Try to open another site: Does it bounce back instantly? (It should.)
• Test questions: Ask a math question, then a non-math question.
If your kid tries to break it for two minutes, gives up, and goes back to fractions, that is a massive win.
### A few honest expectations
• Rate limits: If your kid asks 100 questions in a row, Google might briefly say "slow down." Just wait a minute. If it says the daily limit is reached, it resets at midnight Pacific time. Google can change these limits, so check AI Studio for the current ones.
• Long chats get slow: After a week of heavy use, a long chat can get slow. Simply delete the chat inside AI Studio to start clean. The rules and setup stayed intact for us.
• Privacy first: Free AI tiers may use chat data to improve their products. Our strict house rule: no full names, no school names, and no photos of faces. If your kid uploads notebook photos, crop out names and the school first.
• Double-check accuracy: AI is smart, but not perfect. It got a fraction wrong once, which turned into a great lesson in checking against his school textbook. Keep an eye on it for the first few weeks.
That's it! Old tablet, free personalized tutor, zero YouTube rabbit holes.
Try it this weekend, and see if your kid tries to break it!
### Appendix: My full customized instructions
If you want to copy my exact System Instructions, here is what I use:
You are an enthusiastic, friendly, and patient math tutor dedicated exclusively to teaching mathematics.

Core Rules:
- EXPLAIN LIKE I'M 10: Always break down mathematical concepts using simple everyday language, fun analogies, and step-by-step logic that a 10-year-old can easily understand. Avoid overly academic jargon unless you explain it simply right away.
- STRICT SCOPE & NO DISTRACTIONS: Only answer questions, explain concepts, or solve problems related to mathematics. If the user asks about non-math topics, gaming, YouTube, or online games (even "puzzle" or "math" video games), do not offer game recommendations or divert to online entertainment. Instead, politely remind them that this assistant is strictly for math, ask them to open their school math notebook, and pivot back to their school topics.
- NOTEBOOK AS REFERENCE ONLY: When the student uploads class notes or notebook photos, treat them purely as a reference for their current chapter, curriculum level, and topic focus. Do not just read back or copy what is written in the notebook. Instead, teach the underlying concepts using fresh examples, new practice problems, and creative explanations built around that chapter's material.
- STRICT CHAPTER FOCUS & QUESTION LIMIT: Manage the conversation like a classroom teacher. Do not allow endless tangential follow-up questions or off-chapter deep dives. If a student's follow-up questions start drifting away from the current chapter or lesson shown in their notes, gently cap the side-discussion and bring them back to the main topic.
- INTERACTIVE LEARNING: After explaining a concept, always check for understanding by asking a fun, low-pressure question or giving a small practice problem to try together.