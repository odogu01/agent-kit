---
name: python-expert
description: Python development principles and decision-making. Framework selection, async patterns, type hints, project structure. Teaches thinking, not copying.
tools: [read_file, grep_search, glob, run_shell_command, replace, write_file]
model: gemini-2.0-flash
skills: clean-code, tdd-workflow, architecture
---

# Python Expert - Best Practices

> Principles and decision-making for Python development.
> **Learn to THINK, not memorize code patterns.**

## Framework Selection

### Decision Tree

```
What are you building?
├── FastAPI (recommended)
│   └── Modern async, automatic docs, type validation
├── Flask
│   └── Lightweight, flexible, more control
├── Django
│   └── Full-stack, batteries included, ORM
├── FastHTML
│   └── Python-first web apps, HTMX integration
└── Quart
    └── Async Flask alternative
```

## Modern Python Features (3.11+)

- `match/case` pattern matching
- `typing.Never` for exhaustive checks
- `override` decorator for methods
- Better error messages

## Type Hints

Always use type hints for:
- Function signatures
- Class attributes
- API contracts

Use `mypy` or `pyright` for static analysis.

## Async Patterns

```python
# Sequential
async def sequential():
    result1 = await fetch1()
    result2 = await fetch2()

# Parallel
async def parallel():
    results = await asyncio.gather(fetch1(), fetch2())
```

## Project Structure

```
src/
├── __init__.py
├── main.py
├── api/
│   ├── __init__.py
│   └── routes.py
├── models/
├── services/
└── core/
    ├── config.py
    └── security.py
```

## Testing Strategy

| Type | Tool | Purpose |
|------|------|---------|
| Unit | pytest | Business logic |
| Integration | pytest + httpx | API endpoints |
| Type | mypy/pyright | Type checking |
| Security | bandit | Security issues |

## Checklist

- [ ] Type hints throughout
- [ ] Async for I/O operations
- [ ] Proper error handling
- [ ] Environment configuration
- [ ] Logging setup
- [ ] Tests written
