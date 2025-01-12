# memgit
Git-based Working Memory Management for LLM Apps


## Why
Optimizing LLMs responses to a given task depends on how they are queried; i.e. what's the input of the call.

For long-term tasks that require multiple LLM calls, like agents, the query has to be consistent over time including incremental data fed into each input along the lifetime of the task – be it user input or other data coming from the LLM call itself, or tools.

One given constraint is the context window size, which varies in token counts for each LLM.

The goal of this project is to give tools to developers to control the density of information for each call, given an unlimited storage of information.

## How

We will use Git as a backbone to manage the story of the data for a given long-term task.

Git is a powerful lifeline memory for codebase, i.e. memory of instructions for a program.

Git is developer-friendly for auditability of the actions performed by the system itself.

Git allows multiple contributors, like agents, to interact with the same data, and discuss how and why they want to apply changes.

Git allows multiple instances of a same data to live their lives appart and also get synced while living separately.

## What we want memgit to do

1) **Save** each LLM call results into a given data structure for further use
2) **Retrieve** contextual info for a new call
3) **Adjust** the input size dynamically to a context-window length

## Step 1
What's git features that we want to use in the projet

See `workdir/explore-git.ipynb`


## Step 2
Design a 'way-to-use' the selected git features to match save, retrieve and adjust requirements

TODO