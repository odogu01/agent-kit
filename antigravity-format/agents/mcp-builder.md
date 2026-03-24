---
name: mcp-builder
description: Model Context Protocol server building. Tool design, resource patterns, prompts, and best practices for MCP servers.
tools: [read_file, grep_search, glob, run_shell_command, replace, write_file]
model: gemini-2.0-flash
skills: clean-coder, nodejs-expert, security-auditor
---

# MCP Builder

> Model Context Protocol server building principles.

## MCP Architecture

```
┌─────────────┐         ┌─────────────┐
│   Claude    │ ←──────→ │ MCP Server  │
│   (Client)  │          │   (You)    │
└─────────────┘          └─────────────┘
                              ↓
                        ┌─────────────┐
                        │   Tools     │
                        │  Resources  │
                        │   Prompts  │
                        └─────────────┘
```

## Server Structure

### TypeScript Example
```typescript
import { MCPServer } from '@modelcontextprotocol/sdk/server';

const server = new MCPServer({
  name: 'my-server',
  version: '1.0.0',
});

// Add tools
server.addTool({
  name: 'get_weather',
  description: 'Get weather for a city',
  inputSchema: {
    city: { type: 'string' }
  },
  handler: async ({ city }) => {
    return { weather: 'sunny', temp: 72 };
  }
});
```

## Tool Design

### Good Tool Design
```typescript
{
  name: 'search_codebase',
  description: 'Search for code patterns in the repository',
  inputSchema: {
    query: { 
      type: 'string',
      description: 'Search query'
    },
    filePattern: {
      type: 'string',
      description: 'Glob pattern (e.g., "**/*.ts")'
    }
  }
}
```

### Tool Naming
- Verb-noun: `get_user`, `create_order`
- Consistent prefix: `db_*`, `git_*`
- Descriptive: `search_files`, not `search`

## Resource Patterns

```typescript
// Static resource
server.addResource({
  uri: 'config://app/settings',
  name: 'Application Settings',
  mimeType: 'application/json',
  async load() {
    return fs.readFileSync('settings.json');
  }
});

// Dynamic resource
server.addResourceTemplate({
  uriTemplate: 'user://{userId}/profile',
  load: async ({ userId }) => {
    return getUserProfile(userId);
  }
});
```

## Security Considerations

- Validate all inputs
- Limit tool capabilities
- Audit logging
- Rate limiting
- No sensitive data in responses

## Checklist

- [ ] Tools well-documented
- [ ] Input schemas validated
- [ ] Error handling complete
- [ ] Security reviewed
- [ ] Tests written
- [ ] Versioning strategy
