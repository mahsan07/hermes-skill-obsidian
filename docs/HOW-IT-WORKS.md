# How Obsidian Works

Read, search, create, and edit notes in an Obsidian vault while preserving links and structure.

![Detailed systems blueprint for Obsidian](../assets/system-blueprint.png)

## Stages

### 1. Confirm the intended vault and note scope

**Primary surface:** `Vault path`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 2. Search titles content links and tags

**Primary surface:** `Markdown notes`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 3. Preserve frontmatter and existing structure

**Primary surface:** `Wiki links and tags`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 4. Create or edit the smallest note set

**Primary surface:** `Backlink graph`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 5. Rebuild links without orphaning references

**Primary surface:** `Updated knowledge vault`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 6. Verify files backlinks and rendered markdown

**Primary surface:** `Updated knowledge vault`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.

## Failure handling

- **Authorization failure:** do not probe credentials or broaden access; report the missing authority.
- **Target ambiguity:** stop before mutation and request the minimum identifying information.
- **Tool or service failure:** retain error evidence, retry only safe transient failures, and cap retries.
- **Verification failure:** classify the run as incomplete even when the preceding operation returned success.

## Completion evidence

The handoff should contain the original request, inspection state, preview or plan, exact execution result, direct verification, and a final receipt naming limitations and withheld actions.
