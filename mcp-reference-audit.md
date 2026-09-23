---
title: "MCP reference audit"
description: "How to interpret the current MCP tool-reference comparison and its blocked fields."
status: generated
version: "0.1"
---

# MCP reference audit

This page records the boundary of the current tool-reference comparison.

## Scope of the comparison

The audit compares the MCP server definition in the connected source with documentation entries in this project. A match requires the exact tool name and current argument contract. Return and failure details are recorded only when the source states them.

## Current boundary

The connected repository source has no attached GitHub authorization. It returned a file list containing `README.md` but no readable server-definition file. The repository's README is a generated placeholder and is not a source of truth for the MCP contract.

The server catalog currently reports 172 registered tools. No tool entry could be verified against a readable source definition in this project.

## Interpretation rules

- A registered tool without a matching entry is an undocumented tool only after the readable server definition has been compared with the complete documentation set.
- A documented name absent from a readable server definition is a removed tool only after the same comparison.
- A changed argument name, type, required flag, default, return shape, or failure response is a contract difference, not a writing preference.
- An unstated purpose remains unstated. This audit does not infer why a tool exists.

## Next audit input

Read the server definition from the connected source after repository access is attached. Replace the blocked status with a per-tool inventory and retain the counts for matching entries and removed documented tools.
