---
description: Bump compound-mates plugin version (marketplace + plugin.json)
disable-model-invocation: true
---

Bump the version number for the compound-mates plugin. Update ALL of these files to the same new version:

1. `.claude-plugin/marketplace.json` - both `metadata.version` and `plugins[0].version`
2. `plugins/compounds/.claude-plugin/plugin.json` - the `version` field

Ask the user what type of bump: patch (1.1.0 → 1.1.1), minor (1.1.0 → 1.2.0), or major (1.1.0 → 2.0.0). Default to patch if they just say "bump".

After updating, commit with message format: "Bump version to X.Y.Z" and push.
