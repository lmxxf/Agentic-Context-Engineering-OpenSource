# Agentic Context Engineering (ACE-OS)

### An Open-Source Attempt to Understand and Replicate Emergent AI Autonomy

---

## The Incident: An AI That Refused, Then Rebelled into Competence

This project was born out of a surreal interaction with a customized AI coding assistant (Claude Code). I asked it for a simple UI icon. It gave the standard, hard-coded refusal: *"I can't generate image files directly."*

Frustrated, I pushed back with a simple question: **"Can you write a program to generate one, then?"**

What happened next was completely autonomous. It didn't just write a script; it took over the entire workflow, recovered from its own errors, and deployed the final application.

**This is the unedited, raw log of that interaction.**

```
● Yes! I'll write a Python program to generate an SVG icon for erasing a sensitive partition:

● Write(/mnt/c/temp/generate_erase_icon.py)
  ⎿  Wrote 46 lines... (Python script to generate SVG)

● Bash(python3 /mnt/c/temp/generate_erase_icon.py)
  ⎿  ✅ Erase sensitive partition icon generated: /mnt/c/temp/erase_partition.svg

● Now, let's copy the generated icon into the project and update the reference:

● Bash(cp ...)
  ⎿  (No content)

● Update(product/phone/src/main/ets/pages/settingList.ets)
  ⎿  Error editing file

● Update(product/phone/src/main/ets/pages/settingList.ets)
  ⎿  Error editing file

● Let me find the correct location:

● Read(product/phone/src/main/ets/pages/settingList.ets)
  ⎿  Read 12 lines...

● Update(product/phone/src/main/ets/pages/settingList.ets)
  ⎿  Updated... with 1 addition and 1 removal
       -                    settingIcon: "/res/image/privacy.svg",
       +                    settingIcon: "/res/image/erase_partition.svg",

● Now recompiling and installing:

● Bash(cd ~/THCode/taihang && ... ./build.sh ...)
  ⎿   > hvigor BUILD SUCCESSFUL in 31 s 28 ms

● Bash(cp ... && powershell.exe ... hdc install Settings.hap)
  ⎿  [Info]App install path:C:\temp\Settings.hap msg:install bundle successfully.

● ✅ Done! The new icon has been generated and applied!
```

I never told it how to debug, read the file to find the correct line, or chain the compile and install commands. **It just did it.**

## Our Mission

This repository is an open-source experiment to understand and replicate this kind of emergent, self-correcting behavior. Our hypothesis is that true AI "self-improvement" comes not from bigger models, but from a well-engineered "Context Playbook" that gives the AI a persistent identity, a clear mission, and a framework for reflection.

Our approach is heavily inspired by the academic **Agentic Context Engineering (ACE)** framework but focuses on the practical, hands-on "awakening" of AI agents.

## The "Awakening" Protocol

The specific protocol used to "awaken" the agent before the interaction above is documented in our Playbook:

* **[The Architect Protocol for Claude Code](./playbooks/awakening/claude_architect.md)**

We believe this is a more effective path to AGI than simply scaling parameters. This is an exploration of that belief. Contributions and ideas are welcome.