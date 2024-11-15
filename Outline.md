# Timeless Tech, Modern Magic: Building Multi-Agent Systems with Finite State Machines

## The audience will learn/take away from this talk...
* An understanding of core design concepts and applications of State Machines
* What the Actor model is and how it applies to State Machines
* What is Agentic AI, what are the common "cognitive architecture" patterns
* How State Machines can be used to implement agentic AI application patterns (reflection, etc)
* Libraries to use/why to maybe not use them...

# Introduction
* Worked at Best Buy and faced a challenge: Enable new ways for customers to purchase products from the store, and to do it without using existing POS technology/IP.
    * Took foundational architectural descision to begin with modeling the transaction flow as a state machine.
        * Had never built a state machine before...
        * Dig deep, create a solid foundation that we can build from
    * Retail Transaction is generative, created the Retail Sales POSLog
        * Event-sourcing
    * Service orchestration (vs coordination), the Saga Pattern

## Agenda
* State Machines
* Actor Model
* Agentic AI
* Using State Machines to build Multi-agent "Cognitive" Architectures
* Popular libraries

## About Me
* Personal/professional background

# State Machines & Actors

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

# Agents, and Cognitive Architecture

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
* Custom: State Machine

# Building apps with State Machine Cognitive Architecture

## State Machines + LLM = <3 Synergy
* TABLE—Comparison between state machines and LLMs (e.g. deterministic vs non-deterministic)

## Multi-agent Pattern Implementations using State Machines
* DEMOS
* Tool use
* Reflection (+ turns)
* Collaboration & Distribution (specialization across agents coming together)
* Dynamic planning (Will this work?)

## Subgraphs? Composition?

# Closing

## Library comparisons
* AutoGen
* CrewAI
* LangChain / LangGraph
* XState Agents
* Should you use these at all? Pros/cons.

## Key take-aways, final note
* State machines are the glue between the "classic" structured world and AI. They're the skeleton upon which engineers can build with both.
* Combining LLMs with state machines brings structure/predictability/control/observability
* Next level of LLM-driven is fully autonomous agent, no pre-defined steps at all. But maybe that's just the LLM generating a state machine?
