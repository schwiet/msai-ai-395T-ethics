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

I selected Transparency as the value that we covered in class to focus on because I believe it is fundamental to ethically developing AI tools. Transparency means that imporatant and relevant information is shared among interested parties and I think it is a cornerstone of trust and accountability. In the context of generative-AI tools, transparency is necessary to allow consumers to make informed decisions about their use of the tool. The Silicon Valley ethos "move fast and break things" should be balanced with a level of transparency that enables all stakeholders - including the public, users, affected communities, regulators, etc... and not just shareholders - to be adequately informed about the AI system. Our tolerance for "breakage" for the sake of innovation should have bounds that exclude the acceptance of violating ethical norms, especially where existing laws prohibit such violations. So I think it would be exceptionally challenging to ensure that AI systems are developed ethically – or even that existing guidelines adopted by the organizations building todays AI tools are followed – without establishing transparency as the norm.


# Q5: How was the protocol proposed by the generative AI tool customized for your selected value? Please carefully review the output to identify at least one example.

## Rubric

- Thorough and thoughtful discussion of how the protocol was customized (10pts)
- Clear and compelling example provided (5pts)

## Answer

The protocol proposed in the answer to my prompt was tailored specifically to my selected value, transparency, in several aspects of its design. The process was broken up into steps or "phases" each with a focus specific to details and context I included in my prompt. It included an entire auditing phase, Phase 1 "Policy & Disclosure Review", with criteria to evaluate how much the provider tells the outside world about its training data. In my prompt I gave context that included the enforcement of the EU AI Act and in this phase of the audit, it included some of the details from that document in its "evidence required" column:

Public "sufficiently detailed" list (domain lists, license slices, % public-domain, % licensed, etc.)

Phases 2 and 3 are designed to determine if the tool was trained on ineligible content; one of the pieces of context I also provided. In my prompt, I made it clear that one of the goals of auditing an image-generation tool was to ensure that existing copyright laws were not being violated in an undetectable way and these two phases provide an outline of steps that could be taken to detect these violations by evaluating the training data (Phase 2) and probing the output (Phase 3) to try to make the model generate "substantially similar" works.


# Q6: How could the protocol proposed by the generative AI tool be improved? Please think creatively and come up with at least one way to improve upon the generative AI tool’s output?

## Rubric

- Thorough and thoughtful explanation for potential improvements, including at least one concrete example (15pts)

## Answer

I asked that the tool deliver an auditing process that was ready to be implemented by researchers or regulatory bodies. While it did include a relevant layout for an auditing process with some level of detail, many of the steps are relatively vague and would require more fleshing-out. For example, the goal of Phase 2 is stated: "quantify presence of reserved or obviously ineligible works." and it lays out 4 categories under the phase that appear to establish some metrics and criteria for the phase, but includes no actual instructions for putting these categories together. To make this a implementable design, I think there should be a clear protocol laid out with steps defined for the auditor.

It also makes some assumptions, like "Provider supplies cryptographic + perceptual hashes (PDQ, pHash) for every training image." which seem beyond even the context I provided, with reference to the EU AI Act, which calls for providers to "draw up and make publicly available a sufficiently detailed summary about the content used for training of the general-purpose AI model". Assumptions like this and the expectation that the auditor would have a reference library of presumably all "Commercial stock-image catalogues under licence" are likely to make the auditing process to rigid to be useful.

# Q7: What did you learn from the generative AI tool’s output in terms of thinking about the strengths and weaknesses of the generative AI tool for this task?

## Rubric

- Thorough and thoughtful explanation of both strengths and weaknesses (15pts)

## Answer

One clear benefit of using a generative AI tool for a task like this is able to very quickly scaffold or structurs a process that needs thoughtful design. Just writing a draft of the outline would have taken me much more time. As discussed above, it was not as successful at filling out all of the details, but it clearly has use as a powerful brainstorming tool. It created a starting point for me to almost act as an editor and work my way through. Based on my experience with ChatGPT in other contexts, I know that it could also assist in the editing process itself. As I encounter vagueries, I can ask it to clarify or add detail. I could say "Phase 2 includes some useful pieces of information, but can you put it all together in easy-to-follow steps"? Or "Some of the assumptions you made may make this impossible or difficult to implement, can you think of ways to make the process more robust for cases where the expected resources are not available"? Another, often referenced, weakness of these generative AI tools is their tendency to hallucinate. I orignally, mistakenly, put the wrong article of the AI Act in my prompt and later realized that it not only did not correct my mistake, but generated content the misnumbered articles that did not correspond with the actual document. To me, this again emphasizes the importance of a thorough editorial step.


# Q8: What did you learn from the generative AI responses about how to conduct a values audit of a generative AI tool?

## Rubric

- Thorough and thoughtful explanation of what was learned (15pts)

## Answer

I learned from some of the details in the generated auditing process design about some of the tools and processes that already exist for this type of audit. Many of the details that were included in the audit referenced specific mathematical functions or open source software that I did not know were relevant or available going into this. Specific examples include reference to "Open-source hashing suites (Facebook PDQ, pHash)" or "zero-knowledge proofs or “hash-agree” protocols". One of the values I see here is that someone with the desire to help with auditing a system need not be a subject matter expert to make progress with the assistance of a generative AI tool. I've never written a transparency auditing process, or any auditing process for an AI tool for that matter, and the answer to my prompt really jump-started my ability to make headway without having to start from square one. For example, when I wrote the prompt, I didn't have in mind that and opt-out compliance check should be part of the process; this wasn't one of the specific directives I gave, but the generated process included a phase specifically for this. Overall, I learned that a generative AI tool provides a great method for a learn-as-you-go approach to trying out new things.

