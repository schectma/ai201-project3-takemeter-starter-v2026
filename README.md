# TakeMeter

> ### 👋 Start here
>
> **New to this repo? Read [RUNNING.md](RUNNING.md) first** — setup, the
> notebook, the baseline, and what to do when something breaks.
>
> Once `python test.py` passes:
>
> ```bash
> head -5 data/practice_labels.csv     # the shape your labels.csv needs
> ```
>
> Then open `takemeter.ipynb` **in this folder** — in VS Code, or with
> `jupyter notebook` if you prefer. Pick the kernel: the `.venv` inside this
> project. Run section 1, which reports the hardware you'll be training on.
> Everything else waits until you have data.
>
> Nothing to upload, nothing to connect, no accounts and no keys. The notebook
> runs on your machine and writes next to your code.
>
> **The rest of this file is your submission.** Fill it in as you go.

---

<!-- ─────────────────────────────────────────────────────────────────────────
     HOW TO USE THIS FILE

     Unit 5 asks for the first five sections. Unit 6 adds the five below them.

     Everything is pasted as TEXT. No screenshots, no images.

     ⚠️ The confusion matrix especially. The notebook prints one as a markdown
     table, ready to copy. A screenshot of a matrix earns nothing. Paste the
     table.
     ───────────────────────────────────────────────────────────────────────── -->

<!-- ═══════════════════════ UNIT 5 — THE BUILD ═══════════════════════ -->

## What This Does

<!-- Your community, and what your classifier sorts posts into. Three or four
     sentences. -->
Community: https://www.reddit.com/r/GirlDinnerDiaries/
Some posts cite a number of days, months, or years. Some posts reference immediate family members, like mother and husband. Many posts use "bf" and "gf" to denote boyfriend and girlfriend. Most posts preface their subjects or objects with "my". Nearly all grief about something.


---

## Label Taxonomy

<!-- Each label: a one-sentence definition and two real examples from your
     reading. Then your decision rule for the hardest boundary.

     The decision rule is worth a point on its own and it's the thing most
     people leave out. Every taxonomy has a hardest boundary. Name yours. -->

### Complaint

**Definition:** Airing grievance with or frustration about something.

**Example 1:**
> My ex and I dated for 3 years, and he never told me he loved me once. I worked long hours while his unemployed ass slept in and watched movies on the couch. He didn’t take me on dates, we spent most of our relationship watching tv or having sex fulfilling his very degrading and often painful kinks. I spent time with his family but he wouldn’t even say hi to mine over FaceTime at Christmas.
>All of that was bad enough, then he left me and immediately fell in love with a new woman, who’s the “love of his life.” Of course there was overlap, she gave me 3 STIs, and when I told them both to take antibiotics, she said she didn’t wanna cause they make her tummy hurt and he defended her. They got married in less than a year. Now they have a successful OF together, and she absolutely loves being his literal sex slave. He takes her on trips and how happy and satisfied they are is posted online every day for the world to see.
>I guess I just can’t stop beating myself up. The lesson I’m learning here is the more you are able and willing to degrade yourself and give up of yourself, the more a man will love you. And feeling like I didn’t stack up. If I had rich hippie parents and an advanced degree like she does, I would be okay doing an OF and it would be fun and not a risk to my career and family. If I was as…athletic I guess, I could handle getting gangbanged in the butt by 20 guys (not an exaggeration). If I was as physically strong and carefree as she is, I could handle all of that, I could withstand DV and STIs wrecking havoc on my body. None of that would faze me and I’d have the ring and live an easy life in an oceanfront house and have a great sex life with a man who loves me. If I was rich, it’d be no problem if my boyfriend wanted to stay at home and do nothing to contribute. I did everything I could to make this man happy, to the point where I was emaciated, sick, and hair falling out from stress. But all of that is so easy for her because she’s better than me. I had some I think pretty reasonable boundaries, so I was unworthy of even a little bit of love.
>And the worst part is Ive been dating someone for a year. He loves me and does everything this guy wouldn’t, and it still doesn’t make me feel better. I feel like, of course I can be treated well when I’m settling. So the two options for are date someone you really like who treats you like garbage, or find a simp who will be nice to you. I guess if true love possible for them, it should be possible for me, but no guy I want will ever treat me better than my ex because I’m not a trust fund muscle mommy made of steel who can take unlimited punches and punch back to earn any respect.
>Obviously this is so fucked up, and pretty unfair to my current partner. I don’t even know where to begin to heal. Therapy’s not helping 

**Example 2:**
>Dinner from yesterday: Creamy Shawarma, mushroom w zhoug, honey roasted carrots and yellow rice with toasted almonds and Cucumber kale salad.
>This jerk off delivered my package to an address with completely different numbers on the address proceeded to take pics of it and say my interview outfit was delivered. I timed the delivery to get here the week of my interview and it was delayed so took a bit longer but alas supposedly arrived the day before the interview. When I get home nothing!! I look at the photos of delivery and this dumb fuck left it at a house that’s not even around my block at all!! I go on their site and they say they’re not liable for any packages lost missing or damaged and to file a claim with onward, I AM SO PISSED. I got the $75 outfit on a crazy sale for $35 not possible to do again genuinely sad but gonna get over it by tomorrow I bet I’m just pissed delivery drivers do this and get away with ruining peoples days and weeks this way. Have to stick to my bummy interview fit I’ve been using for years. Yall please tell me it will be okay

### Meal

**Definition:** Description and/or name of an edible dish.

**Example 1:** 
> Vegan miso soup.
>Pretty much I had paid close to $900 to euthanize their other cat back in late August, and they did not pay me back. Their second male cat had a UTI a week ago which progressed into a blockage to which they were going to get checked out at the vet when they got their paycheck. They called me earlier this morning to say that they would pay me back next Friday for their meds, then a couple hours later, they called me and said that they needed an operation, x-rays, and surgery to remove the blockage. They said it would cost $2000 and they needed me to co-sign the loan.
>I said no. They did not pay me back the initial $900 for their previous cat’s euthanasia, and they was being really manipulative and saying I had to do this and it’s just a piece of paper, although it could have had major long-term consequences for my financial future. They then said it is about money for me, and I said no. I was thinking it would be irresponsible to basically decimate my financial future if they could not pay or did what they promised, and you’re not even supposed to share credit with friends, and we have only been hanging out since beginning of this summer. Their other friend had to give up their paycheck even though they were financially struggling too.
>I got a message from another friend of ours, and they said that my ‘friend’ thinks I hate her, and I was baffled because the ask was extremely unreasonable and risky to do for my own future. Another friend and their mom was listening in and they were so appalled at the way she talked to me and how she did the playbook of being manipulative, and how I did the right thing to refuse to co-sign. I called another friend and he agreed. I talked to the guys who made my burger and they agreed that she was not a friend.
>I’m not even sad, I’m so shocked and I’m baffled as to why she thought I would co-sign a loan. I feel for her losing her cat, however I cannot do this to myself and fuck up my credit/financial future. If it makes me a massive bitch I accept that. I know I did the right thing as that would have been super irresponsible and risky to do with someone that has bad credit and finances.
>I know I should not ruminate on it but genuinely I’m in shock and just…… baffled and really really feel insane right now.

**Example 2:**
> idk if this needs a trigger warning bc i didnt go into detail about anything but tw: death, SA
>I dont really know if this is the right sub to post this in. I feel like if i try posting in the subreddits about depression or something along those lines I am just going to be in an echo chamber. I just see a lot of ppl get support in this group and I know I could use some too.
>I have had a really rough few years. Honestly Ive had a lot of trauma through out my life in total but the last 3-5 years has been particularly hard. Dealing with shame over my sexual past, processing fractured SA memories from childhood, lots of personal death, working the front lines of the pandemic, lots of interpersonal relationship struggles. No real relationships with family. No friendships. I have a partner but we have had infinite ups and downs. Dealing with chronic illness. 7 moves in 8 yrs. But the biggest problem I have in life is how much I hate myself. I genuinely never feel deserving of love or joy. I feel like I have such a big heart and I do everything and anything I can for others. And I have done a lot of work on my emotional regulation and truly feel like a better person for it. I feel softer and more understanding. But I just cant give that same love and compassion to myself. I genuinely have such bad SI constantly. Ive tried meds like a lot. I went to therapy 1-2 times a week for the last yr and it did very little. But I just really want to know how other people out there deal with this emotion. Every time I bring this emotion up to somebody around me I just get angry responses. I dont really know anybody who has dealt with this and I know I am not alone. But how do other people deal with this? Because I really want to stop feeling this way. But I got nothin. How do you love yourself?
>my food is a charcuterie board that I made. this is my favorite food

### The hardest boundary

**Which two labels:** Complaint & Meal

**The decision rule I used every time:** If the post has a complaint, it's `complaint`, even if it has a meal.
<!-- e.g. "If the post names a specific checkable fact, it's `analysis`, even
     if the tone is heated." -->


---

## The Dataset

<!-- Where you collected from, how you labelled, your counts, and three hard
     cases. -->

**Where the posts came from:**

**How I labelled them:** <!-- Cold first? Pre-labelled with AI and corrected?
Say so plainly — the disclosure is required, not penalised. -->

**Counts per label:**

| Label | Count | Share |
|---|---|---|
|  |  |  |
|  |  |  |
|  |  |  |
| **Total** |  | 100% |

**Three hard cases**

<!-- Any post that made you pause: what it was, which two labels it could have
     been, and what you chose. These are worth more than the easy 190. -->

**1.**
> *The post:*
>
> *Could have been:*
>
> *I chose, because:*

**2.**
> *The post:*
>
> *Could have been:*
>
> *I chose, because:*

**3.**
> *The post:*
>
> *Could have been:*
>
> *I chose, because:*

---

## The Training Run

<!-- Your starting model, your settings, and anything you changed and why. -->

**Base model:**

**Settings:** <!-- epochs, learning rate, batch size, seed -->

**Anything I changed from the defaults, and why:**

**Split sizes:** <!-- train / val / test, and per-label counts in the test
split. If a label had fewer than about 8 in test, say so — it explains a lot
of next unit's variance. -->



---

## How I Used AI

<!-- Two specific moments — what you asked, what came back, what you changed.

     ⚠️ Plus disclosure of any pre-labelling. If you had a model pre-label a
     batch and then read and corrected every one, say that. It's an allowed
     workflow and disclosing it costs you nothing. Not disclosing it is the
     problem. -->

**Moment 1**

- *What I asked for:*
- *What came back:*
- *What I changed:*

**Moment 2**

- *What I asked for:*
- *What came back:*
- *What I changed:*

**Pre-labelling disclosure:**

<!-- ═══════════════════════ UNIT 6 — THE TEST ═══════════════════════

     Don't fill these in during unit 5.
     ═══════════════════════════════════════════════════════════════════ -->

---

## Baseline vs. Trained

<!-- Both models on the same posts. `python baseline.py --trained results.json`
     prints this table for you. -->

| Measure | Baseline | Trained | Difference |
|---|---|---|---|
| Overall accuracy |  |  |  |
| Macro F1 |  |  |  |
| F1 — `label_one` |  |  |  |
| F1 — `label_two` |  |  |  |

**What I predicted before I looked:**
<!-- Milestone 1 asks you to write this BEFORE seeing the trained numbers. A
     prediction made afterwards isn't one. -->

**What the gap actually means:**
<!-- If the baseline matched your trained model, your fine-tuning added
     nothing — and that is a real finding, not a failure. Say it plainly. -->



---

## Run Log — Before

<!-- Five criteria across three seeds. The notebook's section 6 prints the
     spread table; the Target and Verdict columns are yours. -->

| Criterion | Target | Seed 42 | Seed 7 | Seed 2024 | Verdict |
|---|---|---|---|---|---|
| 1.  |  |  |  |  |  |
| 2.  |  |  |  |  |  |
| 3.  |  |  |  |  |  |
| 4.  |  |  |  |  |  |
| 5.  |  |  |  |  |  |

### Confusion matrix

<!-- ⚠️ TYPED AS A MARKDOWN TABLE. The notebook prints one ready to paste.
     An image of a matrix earns nothing. -->

| true \ predicted |  |  |  |
|---|---|---|---|
| **** |  |  |  |
| **** |  |  |  |
| **** |  |  |  |

**My biggest off-diagonal number, and what it means:**
<!-- Not "the model made mistakes" — WHICH boundary it didn't learn, and which
     direction. "7 real analysis posts were called hot_take and only 3 went the
     other way" is a direction, not just an error rate. -->



---

## Verdicts and Diagnoses

<!-- MET or MISSED against LAST UNIT's target. The target has to hold across
     all three seeds, not turn up sometimes. -->

| # | Criterion | Target | Verdict | How I decided |
|---|---|---|---|---|
| 1 |  |  |  |  |
| 2 |  |  |  |  |
| 3 |  |  |  |  |
| 4 |  |  |  |  |
| 5 |  |  |  |  |

**Diagnoses**

<!-- For each miss: the cause, and how you know. The four common causes are:
     too few examples for a label, a boundary you applied inconsistently, a
     genuinely hard label pair, and a task the model can't reach from this
     much data.

     ⚠️ Use your agreement report as evidence. It is the only instrument you
     have that can tell a LABELLING problem from a MODEL problem, and this
     section is graded on whether you used it that way. -->



---

## Agreement Report

<!-- Your rate against the staff set, and every disagreement adjudicated.

     Remember you labelled these 30 under the STAFF taxonomy in
     data/staff_taxonomy.md, not your own — so every argument below is made
     from those definitions and those decision rules. -->

**Agreement rate:** ___ / 30 = ___%

<!-- Nobody grades this number. A 60% who argues every disagreement from the
     stated rules beats a 95% who wrote "staff was right" nine times. Several
     of the 30 were chosen because they're genuinely ambiguous — you should be
     winning some of these. -->

**Disagreements**

<!-- Three lines each: the post, both labels, and who you think is right and
     why — grounded in the staff definitions you were both applying.

     Then sort each into one of three piles:
       (a) the rule covered it and I applied it loosely → a consistency problem
       (b) the rule genuinely doesn't say               → a gap in the definitions
       (c) the rule is ambiguous here and my reading is defensible → argue it.
           This is a legitimate win.

     Pile (a) is the one that matters most for your diagnosis: if you applied a
     written rule two different ways on 30 posts, that is direct evidence about
     what you did across your own 200. -->

**1.**
> *The post:*
>
> *Staff said / I said:*
>
> *My call, and why:*
>
> *Which pile:*

**2.**
> *The post:*
>
> *Staff said / I said:*
>
> *My call, and why:*
>
> *Which pile:*

**What the pattern in my disagreements tells me:**



---

## The Improvement

**What I changed:**

**Which diagnosis pointed at it:**

### Run Log — After

| Criterion | Target | Seed 42 | Seed 7 | Seed 2024 | Verdict |
|---|---|---|---|---|---|
| 1.  |  |  |  |  |  |
| 2.  |  |  |  |  |  |
| 3.  |  |  |  |  |  |
| 4.  |  |  |  |  |  |
| 5.  |  |  |  |  |  |

**Did it help, and how do I know:**

<!-- If it didn't, say so. Relabelling that didn't help is a genuinely
     interesting result and earns full credit. -->



---

## What's Still Broken

<!-- For each criterion still missed: what you'd do, and why you stopped. -->



**The gap between what I meant my labels to capture and what the model
learned:**
<!-- Two sentences. Your confusion matrix is the evidence. -->



<!-- ═════════════════════════════════════════════════════════════════════

     SUBMISSION CHECKLIST — unit 5

       [ ] criteria.md has five numbered criteria, each naming a NUMBER
       [ ] Each has a reason underneath tied to your data or taxonomy
       [ ] labels.csv: at least 150 rows, text/label/note, ONE file not split
       [ ] No label above 70%
       [ ] All five unit 5 sections have real content
       [ ] Label Taxonomy includes the decision rule for your hardest boundary
       [ ] The Dataset includes three hard cases
       [ ] results.json and test_split.csv committed (the notebook does this)
       [ ] At least four new commits
       [ ] Repository URL submitted — WRITE IT DOWN

     SUBMISSION CHECKLIST — unit 6

       [ ] Baseline vs. Trained table, with your prediction written beforehand
       [ ] Run Log — Before, five criteria across three seeds
       [ ] Confusion matrix TYPED AS A MARKDOWN TABLE
       [ ] A verdict on every criterion
       [ ] A diagnosis for every miss, using the agreement report as evidence
       [ ] Agreement Report with every disagreement adjudicated
       [ ] One improvement, with Run Log — After
       [ ] What's Still Broken
       [ ] results_three_seeds_before.json, results_three_seeds_after.json,
           baseline_results.json and
           agreement_results.json committed
       [ ] At least four new commits
       [ ] The SAME repository URL as last unit

     Do not delete and recreate this repository.
     ═════════════════════════════════════════════════════════════════════ -->

---

📖 **How to run this project: [RUNNING.md](RUNNING.md)**
