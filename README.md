# Concussion Engine
[![CircleCI](https://img.shields.io/circleci/build/github/hassieswift621/concussion-engine?logo=circleci&style=flat-square)](https://circleci.com/gh/hassieswift621/concussion-engine)

Concussion Engine is a small, modular game engine written in C# and built on MonoGame that uses an Entity-Component-System (ECS) style architecture. It utilises data-oriented design to optimise CPU caching and performance.

This was developed as part of undergrad dissertation.

## Overview

- Core engine: `Hassie.ConcussionEngine.Engine` — contains core interfaces and systems (entity manager, event manager, world management, systems for update/render/physics/input, and collision handling).
- Example games: `Hassie.ConcussionEngine.Pong` and `Hassie.ConcussionEngine.MegaPong` — simple Pong-like games built on the engine.
- Tests: `Hassie.ConcussionEngine.Tests.Engine` — unit tests for engine components.

## Repository structure

- `Hassie.ConcussionEngine.Engine/` — engine implementation (Core, Entity, Event, System, World, Physics, Render, Input, Collision, Component folders).
- `Hassie.ConcussionEngine.Pong/` — Pong example game and content.
- `Hassie.ConcussionEngine.MegaPong/` — MegaPong example game and content.
- `Hassie.ConcussionEngine.Tests.Engine/` — unit tests for engine modules.
- `Concussion Engine.sln` — Visual Studio solution file.

## Requirements

- .NET Core 3
- MonoGame 3.x

## Build

From the repository root, you can build the solution with the .NET CLI:

```bash
dotnet build "Concussion Engine.sln"
```

## Run

To run one of the example games from the repository root:

```bash
dotnet run --project Hassie.ConcussionEngine.Pong/Hassie.ConcussionEngine.Pong.csproj
```

Or for MegaPong:

```bash
dotnet run --project Hassie.ConcussionEngine.MegaPong/Hassie.ConcussionEngine.MegaPong.csproj
```

## Tests

Run tests with:

```bash
dotnet test Hassie.ConcussionEngine.Tests.Engine/Hassie.ConcussionEngine.Tests.Engine.csproj
```
