# Q1: What generative AI tool did you use for this assignment?

## Rubric

- A Generative AI Tool Is Listed (5pts)

## Answer

ChatGPT-o3


# Q2: Enter your prompt.  

## Rubric

- Prompt provided and effective (10pts)

## Answer

(see `prompt.md`)


# Q3: Enter the response from the generative AI tool based on your prompt.

## Rubric

- Response provided; response is meaningful and achieves the goal of the assignment (10pts)

## Answer

(see `response.md`)


# Q4: How did you select your value to focus on, how would you define that value, and what might that value mean in the context of your selected generative AI tool?

## Rubric

- Thorough and thoughtful explanation of why the value was selected (5pts)
- Thorough and thoughtful definition of value (5pts)
- Thorough and thoughtful discussion of the meaning of the value in this context (5pts)

## Answer

From the values we covered in class, I selected Transparency to focus on because I believe it is fundamental to ethically developing AI tools. Without transparency, other values such as fairness and accountability are less practically enforceable.
I would define Transparency as a condition under which important and relevant information is shared among interested parties; it's a commitment to good-faith disclosure and I think it is a cornerstone of trust and accountability.
In the context of generative-AI tools, transparency is necessary to allow consumers to make informed decisions about their use of the tools. The Silicon Valley ethos "move fast and break things" should be balanced with a level of transparency that enables all stakeholders - including the public, users, affected communities, regulators, etc... and not just shareholders - to be adequately informed about the AI system. Our tolerance of "breakage" for the sake of innovation should have bounds that protect us from encouraging the violating of ethical norms, especially where existing laws prohibit such violations. So I think it would be exceptionally challenging to ensure that AI systems are developed ethically – or even to verify that organizations building today's AI tools are following their own existing guidelines – without establishing transparency as vital.


# Q5: How was the protocol proposed by the generative AI tool customized for your selected value? Please carefully review the output to identify at least one example.

## Rubric

- Thorough and thoughtful discussion of how the protocol was customized (10pts)
- Clear and compelling example provided (5pts)

## Answer

Overall, I think the response did a good job capturing that the purpose of the audit was to evaluate a tool for Transparency, particularly in relation to copyright protection and legal compliance, details which were provided in the context of the prompt. 
The process is broken up into steps or "phases", each with a focus that is specific to details and context that I included in my prompt. For example, the first phase of the audit, "Policy & Disclosure Review", provides a sort of initial checklist with criteria for evaluating how much the provider tells the outside world about its training data. In my prompt I gave context that included a desire to aid the enforcement of the EU AI Act and in this phase of the audit, it included some of the details from that AI Act document in its "evidence required" column:

Public "sufficiently detailed" list (domain lists, license slices, % public-domain, % licensed, etc.)

Phases 2 and 3 are designed to determine if the tool was trained on ineligible content. In my prompt, I made it clear that one of the goals of auditing an image-generation tool for transparency was to ensure that existing copyright laws were not being violated in an undisclosed way and these two phases provide an outline of steps that could be taken to detect these violations by evaluating the training data (Phase 2) and probing the output (Phase 3) to try to make the model generate "substantially similar" works.


# Q6: How could the protocol proposed by the generative AI tool be improved? Please think creatively and come up with at least one way to improve upon the generative AI tool’s output?

## Rubric

- Thorough and thoughtful explanation for potential improvements, including at least one concrete example (15pts)

## Answer

I asked that the tool deliver an auditing process that was ready to be implemented by researchers or regulatory bodies. While it did include a layout for an auditing process with high-level steps to take, it is not always easily-grokable, so to speak. Each of the phases provide relevant details and specifications, but many of the steps within a phase are relatively vague and would require more fleshing-out. For example, the goal of Phase 2 is stated: "quantify presence of reserved or obviously ineligible works." and it lays out 4 categories under the phase that appear to establish some metrics and criteria for the phase, but the document includes no actual instructions for putting these categories together. To make this an implementable design, I think there should be a clear protocol laid out with more-detailed steps defined for the auditor. I might take another pass at each individual phase and ask ChatGPT to turn the specifications and requirements into a concrete sequence of steps.

It also makes some assumptions, like "Provider supplies cryptographic + perceptual hashes (PDQ, pHash) for every training image." which seem beyond even the context I provided with reference to the EU AI Act, which calls for providers to "draw up and make publicly available a sufficiently detailed summary about the content used for training of the general-purpose AI model". Assumptions like this, as well as the expectation that the auditor would have a reference library of presumably all "Commercial stock-image catalogues under license", are likely to make the auditing process too rigid to be useful. I think the audit could greatly benefit from a revision to the assumptions to make sure they are realistic and achievable.

# Q7: What did you learn from the generative AI tool’s output in terms of thinking about the strengths and weaknesses of the generative AI tool for this task?

## Rubric

- Thorough and thoughtful explanation of both strengths and weaknesses (15pts)

## Answer

One clear benefit of using a generative AI tool for a task like this is that it is able to very quickly scaffold or structure a process that requires thoughtful design. Just writing a draft of the outline would have taken me much more time and I would have had a hard time even knowing where to start. As discussed above, it was not as successful at filling out all of the details, but it clearly has use as a powerful brainstorming tool. It created a starting point for me where I could pick up and act as an editor, working out the details of the outline it provided. Based on my experience with ChatGPT in other contexts, I know that it could also assist in the editing process itself. As I encounter vagaries, I could ask it to clarify or add detail. I could say "Phase 2 includes some useful pieces of information, but can you put it all together in easy-to-follow steps"?
Another weakness I encountered was its tendency to make facts up. In one of the earlier drafts of my prompt, I mistakenly referenced the wrong article of the AI Act. Later, I realized that ChatGPT not only did not correct my mistake, but generated content for the misnumbered articles that did not correspond with the actual document. To me, this again emphasizes the importance of a thorough editorial step.


# Q8: What did you learn from the generative AI responses about how to conduct a values audit of a generative AI tool?

## Rubric

- Thorough and thoughtful explanation of what was learned (15pts)

## Answer

I learned, from some of the details in the generated auditing process design, about tools and processes that already exist for this type of audit. Many of the details that were included in the audit referenced specific mathematical functions or open source software that I did not know were relevant or available going into this. Specific examples include reference to "Open-source hashing suites (Facebook PDQ, pHash)" or "zero-knowledge proofs or “hash-agree” protocols". One of the values I see here is that, with the assistance of a generative AI tool, someone with the desire to help with auditing a system need not be a subject matter expert to be productive. I've never written a transparency auditing process - or any auditing process for an AI tool for that matter - and the answer to my prompt really jump-started my ability to make headway without having to start from square one. For example, when I wrote the prompt, I didn't have in mind that an opt-out compliance check should be part of the process; this wasn't one of the specific directives I gave, but the generated process included a phase specifically for this. Overall, I learned that a generative AI tool provides a great method for a learn-as-you-go approach to trying out new things.

