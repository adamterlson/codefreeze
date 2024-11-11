# State Machines in the age of AI
## The audience will learn/take away from this talk...
* A solid understanding of concepts and application of State Machines
* What the Actor model is and how to apply it
* What is Agentic AI, what are the common "cognitive architecture" patterns, including leveraging state machines
* How to leverage State Machines to implement agentic AI application patterns (reflection, etc)
* Libraries to use...

# Introduction
* Hook: Working at Best Buy and greenfielding POS, applying state machines—they are a powerful tool
    * Had never built a state machine before...
    * Dig deep, create a solid foundation that we can build from
* Backend service: state machine
* Agenda

## About Me
* Personal/professional background

# State Machines, Actors, Agents, and Cognitive Architecture

## Intro to State Machines
* Why State Machines?
    * "Ive never met a state machine I didn't like."
    * Positive qualities
        * Clarity of purpose
        * Simplified complexity
        * Fail-safe design
        * Modularity
* State Diagrams
    * VISUAL
    * Definitions: 
        * State
        * Transition
        * Context/Infinite state
* JS State Machine definition in XState
    * VISUAL
    * Declarative definition

## State Machines in Applications
* Creating a service from a machine
* Resuming from state? Replay.
* Events in and out
* Running machines are a service/actor

## Actors
* What's an Actor?
    * Persisted, internal, isolated state
    * Sends/receives Events
    * Creates other Actors
* Creating an Actor with XState

## State Machines + LLM = <3
* TABLE—Comparison between state machines and LLMs (e.g. deterministic vs non-deterministic)

## From Actors to Agents
* What's an Agent?
    * Role
    * Goal/Task/Job
    * Backstory—fine-tuning
    * Context (persistent memory)
* Agents vs Actors
    * Persisted, internal, isolated state
    * Send/receives messages
    * Creates other agents
* Creating a Task
    * Descripiton
    * Output format
    * Assigned agent

## Why Multi-agent?
* Scaling limitations of a single agent
    * Too many tools (> 5)
    * Context grows too complex
    * Prompting a Multi-step process
* Forces: split out specialized tasks into a workflow (planner, coder, etc)
* Benefits
    * Modularity
    * Specialization
    * Control
* Multi-agent Workflow Steps
    * Research
    * Analyze
    * Act/Report

## Multi-agent "Cognitive" Architectures
* VISUALS
* Network
    * Every agent decides which agent goes next
    * e.g. CrewAI
* Supervisor
    * Central LLM decides which sub-agents to call
    * e.g. ChatManagers in AutoGen
* Heirarchical
    * Nest the supervisors
* State Machine

# Building apps with State Machine Cognitive Architecture

## Multi-agent Pattern Implementations using State Machines
* Reflection
* Collaboration & Distribution (specialization across agents coming together)
* Dynamic planning

## Building a human in the loop with more state machines
* Self checkout example?
* Human as Tool
* Human as State

## Layering on patterns as components in your workflow
* Reflection/critic with max turns
    * withReflection(state)

## Subgraphs?

# Closing

## Libraries, and should you use them?
* AutoGen
* CrewAI
* LangChain / LangGraph

## Key take-aways, final note
* State machines are the glue between the "classic" structured world and AI. They're the skeleton upon which engineers can build with both.
* Next level of LLM-driven is fully autonomous agent, no pre-defined steps at all. But maybe that's just the LLM generating a state machine?

## 5. State Machines as a Foundation for Multi-Agent Systems
* Agents as "intelligent" state machines with goals
* Predictability and modularity for complex coordination


* LLMs generate the whole event object
* Event reducer LLM last step in workflow - use messages inside workflow. chatty
* Handle this event from my UI state machine
* Orchestration agent, LLM says where the event goes



## Building Agents with LangGraph
* LangGraph provides control for custom agent and multi-agent workflows, seamless human-in-the-loop interactions, and native streaming support for enhanced agent reliability and execution.

### Agent Design Patterns
* "There's even something called React!"
    * ReAct—Reason and Act