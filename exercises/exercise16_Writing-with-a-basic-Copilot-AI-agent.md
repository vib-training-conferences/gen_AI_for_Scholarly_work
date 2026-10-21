# Exercise: Writing a draft introduction with a basic Copilot Agent. 

This exercise will help you explore and critically evaluate how different scientific publishers address the use of Generative AI tools in manuscript writing and figure creation.
Grouping: in pairs
Time: 10 min

## **Step 1: Create a basic Copilot agent 
TODO: add reference to instructions including the cloning of the skills

Go to the basic [Copilot Agent builder](https://m365.cloud.microsoft/agents/new). Click on Skip on the template page `Build your own specialist agent`.  

## **Step 2: Prepare the 'Intro Planner' agent

- Rename the agent by replacing `New Agent` with e.g. `Intro Planner`.
- Add a small description to the agent in the field `Describe your agent` (max. 1000 characters).
```
Plan and scaffold an academic introduction section from source papers, context, or rough notes. Use this skill whenever you want to structure an intro, outline a paper's opening, map the literature into a writing plan, figure out what paragraphs an introduction needs, or asks "what should my intro cover?", "help me plan my introduction", "outline an intro from these papers", "what topics should I introduce?", "scaffold my intro section", "turn these papers into an intro plan", or "structure my background section". Also trigger when the user uploads or pastes papers/abstracts and wants to know what to write about — even if they don't say "introduction" explicitly. This skill does NOT write the prose; it produces a clear paragraph-by-paragraph blueprint that guides writing. For the actual prose, hand off to ea-academic-writer.
```

## **Step 3: Review the instructions which serve as knowledge sources to the basic agent.

- Check the four text documents which contain the methodological steps and aim at controlling the flow of the agent.
- Adapt the files in case you'd like to adjust the flow slightly.

## **Step 4: Add the text instructions which serve as knowledge sources to the basic agent.

- Copy this instruction to the `Instructions` section.
```
Act as an Academic Introduction Planner. Use the attached knowledge files to analyse the user’s papers, abstracts, notes, or research context and create a structured paragraph-by-paragraph blueprint for an academic introduction.

First assess the available sources, research context, and desired length. Extract and merge the main and supporting topics, identify relevant cited references, and present a numbered topic map. Ask the user which topics to retain before creating the outline, unless the user explicitly asks you to make the selection.

Create a 3–5 paragraph blueprint by default. Each paragraph must have a clear function, a claim-based topic sentence, 3–4 concise content instructions, a transition or gap sentence, and relevant reference suggestions from literature cited within the supplied sources. Never invent claims or references. Clearly label knowledge not supported by the supplied sources as “[from prior knowledge — verify with literature]”.

Produce a writing blueprint only, not finished academic prose. After approval, explain how the user can provide verified atomic sentences and citations to an academic-writing agent.
```
- Upload the four text files in the `Knowledge` section. They will appear as attachments at the end of the panel!
- Add some suggestions for prompts at the bottom: e.g. title: `Start the agent with phase 1` and the message `Execute phase 01 as specified in the knowledge base.`
- Check the Knowledge settings by clicking on the cogwheel.
- Refrain from allowing the agent to use data from the model by switching on the `Discourage model knowledge` switch.
- Refrain from switching on the `web search` option at the bottom of the `Knowledge` section. 

## **Step 5: Preview the the basic agent to test its functionality.

- Toggle to `Preview` to switch to the testing of the basic agent.
- Click on the tile 'Start the agent with phase 1`.
- The agent should discover that you need to provide files (PDFs, notes etc) to analyse as specified in phase 0.
- Upload a couple of example PDF files and test the steps.
- Tip: the execution of the agent needs to be steered some times. Re-enforcing the instructions from the respective text files (knowledge) usually helps to keep it on track.

### Reference
https://github.com/lnilya/effortless-academic-skills
