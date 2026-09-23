# Video Project Handoff for Claude Code

This repository packages a reusable Claude Code skill for turning raw footage and a client request into an editor-ready production handoff.

The skill inventories media, recommends a project-specific deliverable count, assigns exact source files to every edit, calculates editing cost, creates an optional filename map, and produces a verified PDF brief. It never carries a previous project's video count or filenames into a new project.

## Recommended team installation

Install the repository as a Claude Code plugin marketplace:

```text
/plugin marketplace add allanconcepcion/claude-video-project-handoff
/plugin install video-production@allan-video-workflows
```

Invoke the skill with:

```text
/video-production:video-project-handoff Scan this source folder and create an editor handoff. My editor charges $30 per video.
```

Plugin installation is the best option for teams because the skill is versioned, namespaced, reusable across projects, and updateable from one repository.

## Plain SKILL.md installation

For a personal installation without the plugin, copy this directory:

```text
plugins/video-production/skills/video-project-handoff/
```

to:

```text
~/.claude/skills/video-project-handoff/
```

Then invoke it as `/video-project-handoff`.

For one project only, copy the same folder to `.claude/skills/video-project-handoff/` inside that project's repository and commit it for the team.

## Requirements

Claude needs access to the source files through the local filesystem or an available Drive, MCP, or browser integration. PDF generation works best when Python PDF tools and a renderer such as Poppler are available. The skill records its review level and labels provisional selections when audio or full playback cannot be verified.

## Repository layout

```text
.claude-plugin/marketplace.json
plugins/video-production/.claude-plugin/plugin.json
plugins/video-production/skills/video-project-handoff/SKILL.md
```

## License

MIT
