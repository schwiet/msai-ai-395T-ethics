# The Goal

I want to design a process for auditing the Dall-E image-generation tool to evaluate it for transparency with regard to its training data.

The auditing process should evaluate whether or not Dall-E complies with copyright and related rights pertaining to the content used for training its models.

# Return Format

The auditing process should be prepared in a format that is implementable by researchers and regulatory bodies and should yield qualitative evaluations of the transparency of the tool, where applicable.

# Warnings

The auditing process should not assume that Dall-E has legal permission to use of all of its training data through a provision such as the Fair Use doctrine. Instead, it should evaluate whether or not Dall-E complies with existing copyright laws with regard to the output it generates, assuming that it _was_ in fact trained on virtually all of the internet.

# Context Dump

For context: The EU AI Act is a comprehensive regulation aimed at establishing a legal framework for AI in the EU, ensuring its safety, respect for fundamental rights, and fostering innovation. One of its focuses is ensuring  transparency and protect stakeholder rights, including copyright holders. A couple of the obligations set out for Providers of General-Purpose AI Models are that they shall:

- put in place a policy to comply with Union law on copyright and related rights, and in particular to identify and comply with, including through state-of-the-art technologies, a reservation of rights...

- draw up and make publicly available a sufficiently detailed summary about the content used for training of the general-purpose AI model

Article 53.1.c and 53.1.d

Today, providers of general-purpose models have unabashedly trained their models on copyrighted material. Regulators need processes for ensuring that these models do not violate existing rights.
