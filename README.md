# memgit
Git-based Working Memory Management for LLM Apps
The MemGit project aims to utilize Git for managing the short-term and working memory of LLM (Large Language Model) calls. The goal is to develop a memory management module that handles the information to be pushed into the working context windows of each LLM call.

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

## Memory Management Module

The memory management module will be responsible for:

- Managing the information flow into the working context of LLM calls.
- Ensuring that relevant data is available for each LLM call to enhance performance and accuracy.

## Git as the Backbone

Git will be used as the backbone for data storage and version control. The reasons for choosing Git include:
- Robust version control capabilities.
- Efficient handling of differences in data versions.
- Widely adopted and well-understood by developers.

## Episodes in Markdown for Data Format

Episodes and Git Tree Structure

The content stored in Markdown will be referred to as "episodes". These episodes will be organized within a Git tree structure, allowing for efficient storage and retrieval.

Markdown will be used as the data format due to its:

- Lightweight structure.
- Ease of understanding by LLMs.
- Simplicity in managing version differences in Git.

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