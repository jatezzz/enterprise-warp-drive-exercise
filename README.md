# enterprise-warp-drive-exercise

A Java solution to the "Star Trek" warp-drive programming exercise. It computes how the three plasma injectors of the Enterprise must share flow, given each one's damage, to reach a requested speed, and how long the engine can run.

## Context

The original README says "Exercise: Star Trek". The NetBeans build metadata is dated January 2019, and the code was uploaded to GitHub in August 2019.

## What it shows

- A domain model split into small classes: `StarshipEnterprise`, `PlasmaInjector`, `PowerManagementSystem` and `Computer`. A `Scotty` entry point runs individual checks.
- Business rules for damaged injectors: flow redistribution, extra flow, and the resulting operating time.
- A JUnit test class with eight tests that walk through the input combinations from the brief.
- Early attention to tests at a time when most of my code had none.

## Stack

Java, JUnit, NetBeans 8.2, Ant.

## Run it

Open it as a NetBeans project and run the tests, or build it with `ant` and run `Scotty`.

## Looking back (2026)

Today I would use parameterized tests (JUnit 5) for the input table, use records or immutable value types for the injector state, and build it with Gradle.
