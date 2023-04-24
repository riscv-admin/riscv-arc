# ARC Review Request Process

This README.md outlines the process for handling review requests in the ARC (Architecture Review Committee). Each review request follows a series of stages, represented by tags, which help track the status of the review.

Architecture Review Requests is a systematic process designed to evaluate and assess proposed architectural designs and solutions, with a focus on producing robust extensions that adhere to ratified RISC-V specifications and the overall RISC-V strategy. The ARR process ensures consistency in opcode encodings, mnemonics, Control and Status Registers (CSRs), and other conventions across extensions, while also addressing the needs of different profile targets and effectively managing encoding resources.

**You can find a comprehensive dashboard displaying all ongoing review activities [here](https://github.com/orgs/riscv-admin/projects/3).**

## Table of Contents

1. [Process Overview](#process-overview)
2. [Tags Explained](#tags-explained)
3. [Process Flow](#process-flow)

## Process Overview

When a new review request arrives ([click here to open a new request](https://github.com/riscv-admin/riscv-arc/issues/new?assignees=rpsene&labels=REQUESTED&template=h_arc_review_request.yaml&title=%5BSpec+Architecture+Review+Request%5D+-+ADD+A+SPECIFICATION+TITLE+HERE)), it starts with the `REQUESTED` tag. The ARC Chair or Vice-chair assigns a target ARC meeting when the request will be reviewed, and the request tag is updated to `SCHEDULED`. The review process begins, and the tag is updated accordingly throughout the stages. If rework is required, the tag `REWORK PENDING` is set. Once rework is done, the process starts again. If a request is approved, it receives the `APPROVED` tag and is closed. If not approved, it receives the `NOT APPROVED` tag and is closed. Reopened requests follow the process from the beginning.

You can view the complete workflow illustrated in the diagram provided below:

![alt text for screen readers](/images/rvi_arc.png "ARC Review Process")

## Tags Explained

- `REQUESTED`: Indicates a new review request has been submitted.
- `SCHEDULED`: The review request has been assigned a target ARC meeting date.
- `UNDER REVIEW`: The review process is in progress.
- `REWORK PENDING`: Rework is required on the request.
- `APPROVED`: The review request has been approved.
- `NOT APPROVED`: The review request has not been approved.
- `CLOSED`: The review request is closed.

## Process Flow

1. A new review request arrives and is tagged with `REQUESTED`.
2. The ARC Chair or Vice-chair assigns a target ARC meeting date and updates the tag to `SCHEDULED`.
3. The ARC Chair or Vice-chair sets the tag as `UNDER REVIEW` when the review begins.
4. After the review:
   - If rework is required, the tag is set to `REWORK PENDING`.
   - If the request is approved, it is tagged with `APPROVED` and closed.
   - If the request is not approved, it is tagged with `NOT APPROVED` and closed.
5. If a rework is done on a request with the `REWORK PENDING` tag, the process restarts from step 1.
6. If a closed request with the `NOT APPROVED` tag is reopened, the process restarts from step 1.
