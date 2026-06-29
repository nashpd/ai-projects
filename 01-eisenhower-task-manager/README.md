# My First AI Project: A Task Manager That Actually Works

*By Nash David | nashpd on X | Published July 2026*

---

## Before You Read This

You do not need to know how to code.

You do not need to have used GitHub before. If you are confused about what GitHub even is and why you are reading a document here, I will explain that in a moment.

You do not need any special software beyond what you already have.

What you need: a free AI tool, a Google account, and about 45 minutes the first time. Less once you know what you are doing.

This document walks through the exact project I described in my LinkedIn post. Every step. Every prompt I typed. Every decision I made and why. Including the ones that did not work on the first try.

---

## What Is GitHub, and Why Are You Here?

Think of GitHub as a public filing cabinet on the internet.

Developers use it to store and share code. But it is also increasingly used by anyone who wants to share structured work publicly: documents, templates, instructions, projects.

I am using it here for one reason. I wanted a place where I could share the full detail of what I built without compressing it into a LinkedIn post. LinkedIn is where the conversation starts. GitHub is where the actual work lives.

You do not need a GitHub account to read this. You are already reading it. If you want to download the files I have shared here, you will need a free account. Creating one takes three minutes. There is a green button at the top of this page that says "Code." That is where you find the files.

---

## What We Are Building

A task manager based on the Eisenhower Matrix.

Here is what that means in plain language.

Every task you have can be placed in one of four boxes:

| | **Urgent** | **Not Urgent** |
|---|---|---|
| **Important** | Do it now | Schedule it |
| **Not Important** | Delegate it | Drop it |

Four boxes. The logic is simple. The problem, and this is the problem I had for twenty years, is that under pressure everything feels urgent and everything feels important. The matrix does not help you if you cannot think clearly enough to use it.

This is exactly where AI earns its place.

Instead of you having to sort your own tasks while already overwhelmed, you describe your tasks to AI in plain language and it does the sorting. It also asks you questions that slow you down just enough to think clearly. The result is a sorted task list you can act on immediately.

We are going to build a Google Sheet that holds this system, and we are going to use AI to populate it.

---

## What You Will Need

1. A Google account (for Google Sheets)
2. Access to an AI tool. I used Claude (claude.ai). There is a free tier. You can also use ChatGPT (chatgpt.com). Both work for this project.
3. A list of your actual tasks. Whatever is on your mind right now, work or personal, big or small.

---

## How to Use an AI Tool: Your First Conversation

If you have never typed into Claude or ChatGPT before, here is exactly what happens.

Go to claude.ai or chatgpt.com. Sign in. You will see a screen with a large empty text box, usually at the bottom of the page. This is where you type. There are no buttons to configure, no settings to adjust before you begin. You type and press Enter or click the arrow button to send.

The AI responds in the same window, directly below what you typed. You can reply to it, ask it to change something, or ask a follow-up question. It remembers everything said in the same conversation window. Think of it as a conversation partner who retains full context of everything discussed in that session, but starts fresh in the next one.

For this project, you will open a new conversation, paste the prompt from Step 3, add your task list at the bottom of it, and send. The AI will either ask you clarifying questions or return a sorted list. If it asks questions, answer them in plain sentences. When it gives you the sorted output, you copy it. Nothing more is required.

---

## Step 1: Set Up Your Google Sheet

Open Google Sheets (sheets.google.com). Create a new blank sheet.

Set up these column headers in Row 1:

- Column A: Task
- Column B: Deadline (if any)
- Column C: Urgency (AI will fill this)
- Column D: Importance (AI will fill this)
- Column E: Quadrant (AI will fill this)
- Column F: Action

Leave columns C, D, E, and F empty for now. AI is going to help you fill those in.

Name your sheet something simple. "My Task Manager" works.

I have shared a pre-built version of this sheet in this repository. The link is in `task-tracker-sheet-link.md`. You can make a copy of it directly into your Google Drive rather than building from scratch. Either approach works.

---

## Step 2: Write Down Your Tasks

Before you open the AI tool, spend five minutes writing down every task that is on your mind.

Do not organise them. Do not prioritise them. Do not edit yourself. Write them in Column A of your sheet, one task per row.

They can be vague. "Reply to Rahul" is fine. "Figure out the project thing" is fine. "Sort out insurance" is fine. You will add detail in the next step.

The goal is to empty your head onto the page. Every open commitment you are carrying, however small, goes in. In my experience, when you think you are done, you will find three more. Keep going until the list feels genuinely complete.

---

## Step 3: Open Your AI Tool

Go to claude.ai or chatgpt.com. Open a new conversation.

Copy this prompt exactly. Paste it in and press send:

---

*I am going to give you a list of tasks. For each task, I need you to help me sort it using the Eisenhower Matrix. The four categories are:*

*1. Urgent and Important: do it now*
*2. Important but Not Urgent: schedule it*
*3. Urgent but Not Important: delegate it*
*4. Neither Urgent nor Important: drop it*

*Before you sort each task, ask me two questions if you are not sure: What happens if this does not get done today? And does this directly affect a key goal or commitment I have?*

*Here are my tasks:*
*[paste your task list here]*

---

Paste your task list where indicated and send.

---

## Step 4: Move the Output Into Your Sheet

When the AI returns your sorted task list, copy the full response.

Go back to your Google Sheet. For each task the AI has categorised:

- Find the task in Column A
- In Column C, type what the AI said about urgency: High or Low
- In Column D, type what the AI said about importance: High or Low
- In Column E, type the quadrant it assigned: Q1, Q2, Q3, or Q4
- In Column F, write one action: the single next step for that task in one sentence

If the AI's categorisation does not feel right for a particular task, change it. You know your situation better than it does. The AI gives you a starting point. You make the final call.

---

## Step 5: Use It

Your sheet now has a sorted, actionable task list.

Work from Quadrant 1 first. When those are done, move to Quadrant 2. Do not touch Quadrant 3 unless you have someone to hand it to. Look at Quadrant 4 and ask yourself honestly why it was on your list at all.

Update the sheet weekly. At the start of each week, add new tasks and run the same prompt again with the new items. It takes ten minutes once you know the system.

---

## What I Learned Building This

The AI did not just sort my tasks. It asked me a question that changed how I saw one of them entirely.

One of my tasks was to respond to a long-pending email from a colleague. I had been carrying it for two weeks. When the AI asked what happens if this does not get done today, I realised the honest answer was: nothing urgent. The email was important relationally but carried no immediate consequence.

That one question moved it out of Quadrant 1. The mental space I had been spending on guilt rather than action came back.

The spreadsheet is the output. The thinking the conversation forces is the actual value.

---

## Files in This Repository

- `README.md` — this document, the full guide
- `prompt-library.md` — the exact prompts used in this project, ready to copy and paste
- `task-tracker-sheet-link.md` — link to the Google Sheet template

*The Google Sheet template will be linked here before Friday 04-Jul-2026.*

---

## What Is Next

The comments on my LinkedIn post will shape the next project.

If you found this useful, or if you tried it and something did not work, I want to know. Connect with me on [LinkedIn](https://www.linkedin.com/in/nash-david/) or reply to me on X at @nashpd.

Every project I publish here will follow the same format: a real problem, a real build, every step documented, no assumed knowledge.

---

*This document is intentionally written without jargon. If any part of it is unclear, that is a failure of the writing, not a gap in your knowledge. Tell me what confused you.*
