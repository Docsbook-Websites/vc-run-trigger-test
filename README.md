---
title: "MCP server reference status"
description: "Current status of the MCP tool-reference audit for VC Run Trigger Test."
status: generated
version: "0.12"
---

# MCP server reference status

This project does not yet contain a verified reference for the MCP server's tools.

## Audit result

The connected source is the repository `docsbook-websites/vc-run-trigger-test`. The source currently exposes only `README.md`, and its contents do not define the MCP server's registered tools, arguments, return values, or failure responses.

The server connection currently reports **172 registered tools**. This documentation contains **0 verified tool entries** matching current source definitions. (edit test)

- Registered tools with a verified documented entry: **0 of 172**
- Documented tools that no longer exist: **0 found**
- Tool purposes that can be stated from the source: **none**

These counts are an audit status, not a claim that the tools are undocumented elsewhere.

## Why the comparison is blocked

The repository source has no attached GitHub authorization, so its server definition could not be read. The only available repository file is this page. Without the source definition, this page cannot safely list tool names, argument names or types, return shapes, required fields, defaults, or failure behavior.

A complete comparison must read the server definition from the connected source and then compare each registered tool with one reference entry. If the source does not state a tool's purpose, the reference must label that purpose as **not stated by the source** rather than infer it.

## What to provide next

Attach readable access for the connected repository, then rerun the MCP reference audit. The resulting reference should contain one entry per registered tool with:

1. The exact tool name.
2. Every current argument, including type, required status, default, and accepted values when stated.
3. The documented return shape and source-stated meaning.
4. The source-stated failure responses and conditions.
5. A clear note wherever the source does not state the tool's purpose, return detail, or failure behavior.

Until the source can be read, adding signatures or purposes here would create undocumented assumptions rather than bring the documentation in step with the server.
