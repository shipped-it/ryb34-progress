# Overview (/)





**Rock your Baby - Team 34**

A controller that reads a baby's heart rate and crying, decides a rocking motion, and drives a cradle. Four PYNQ Z2 boards, one communication backbone, one cradle.

| Field        |                     |
| ------------ | ------------------- |
| **Team**     | 34 · 9 members      |
| **Board**    | PYNQ Z2 (Zynq-7020) |
| **Document** | v1.5 · Sections 1+2 |
| **Updated**  | 15 October 2026     |

## Status [#status]

| Status             | What                                | Detail                                             |
| ------------------ | ----------------------------------- | -------------------------------------------------- |
| ✅ **Done**         | Sections 1-2 in the design document | Requirements, architecture, communication protocol |
| 🔶 **In progress** | Section 3 design description        | Per-submodule design, S1-S4                        |
| ⬜ **Next**         | Board bring-up                      | Hardware time slots, 1 kHz PWM + comm verification |

## The team [#the-team]

| Role          | Who               |
| ------------- | ----------------- |
| S1 Heartbeat  | Alex, Artem       |
| S2 Crying     | Alexandru, Val    |
| S3 Decision   | JG, Ties          |
| S4 Motors     | Mika, Lucca, Hugo |
| Communication | JG, Ties          |

## The system [#the-system]

<img alt="Full system block diagram" src="__img0" />

## Reading this site [#reading-this-site]

* [Submodules](/submodules): the four boards and their job
* [Communication](/communication): how the boards talk to each other
* [Open assumptions](/assumptions): what we are still validating
* [Design document](/document): the PDF
* [Milestones](/timeline): where we are in the course schedule
