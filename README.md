# LessWrong and EA Forum

A Claude Code skill for interacting with LessWrong, EA Forum, and Alignment Forum via their GraphQL API.

## Features

- **Read posts** - Fetch any post by slug
- **Search posts** - Search across forum content
- **Create drafts** - Create draft posts (requires auth token)
- **List drafts** - View your unpublished drafts
- **Activity digests** - Track users and topics, generate activity summaries

## Documentation

See [SKILL.md](./SKILL.md) for complete documentation and usage instructions.

## Installation

To use this skill with Claude Code, clone it into your skills directory:

```bash
git clone https://github.com/HartreeWorks/claude-skill--lesswrong-and-ea-forum.git ~/.claude/skills/lesswrong-and-ea-forum
```

Then restart Claude Code to load the skill.

## Quick start

```bash
# Search for posts
python ~/.claude/skills/lesswrong-and-ea-forum/scripts/forum_api.py search "AI safety"

# Read a post
python ~/.claude/skills/lesswrong-and-ea-forum/scripts/forum_api.py post graphql-tutorial-for-lesswrong

# Create a draft (requires auth setup)
python ~/.claude/skills/lesswrong-and-ea-forum/scripts/forum_api.py create-draft --title "My Post" --content "Hello world"
```
