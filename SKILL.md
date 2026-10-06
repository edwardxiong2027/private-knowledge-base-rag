---
name: private-knowledge-base-rag
description: Plan a source-citing knowledge assistant that respects document boundaries and says when it cannot answer. Use when: You need Q&A over private notes or a collection of trusted documents.
license: MIT
metadata:
  author: Edward Xiong
  version: 1.0.0
---

# Private Knowledge Base

Plan a source-citing knowledge assistant that respects document boundaries and says when it cannot answer.

## When to use

You need Q&A over private notes or a collection of trusted documents.

## Workflow

1. Define data access and who is allowed to see what.
2. Preserve document identity and chunk provenance.
3. Require answers to cite retrieved evidence.
4. Test unanswerable and cross-document questions.

## Output

Return a usable result for the user’s actual task. State assumptions, evidence, and uncertainty where they affect the result. Keep the output format suited to the job: working HTML, a storyboard, a decision brief, a draft, code, or a short answer. Do not claim that a result was tested, published, or verified unless that action was completed.

## Starter prompt

> Design a retrieval assistant for [document collection] and [users]. Map data sensitivity, permissions, source formats, update cadence, and deletion requirements first. Propose an indexing/retrieval approach sized to the collection. Answers must cite source and location, distinguish retrieved evidence from inference, and abstain when evidence is missing. Include tests for access boundaries, stale documents, conflicting sources, and unanswerable questions. Do not send private content to an unapproved service.

## Quality check

Before delivery, check that the result answers the stated need, follows the requested format, and makes any important limitation visible. Invite the user to adjust the result when taste or judgment belongs to them.
