# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-05-18

### Added

- **Project Management**: Save, organize, and quickly switch between projects with a beautiful sidebar UI.
- **Tags System**: Color-coded tags with drag-and-drop assignment, inline editing, and reordering.
- **Custom Sorting**: Drag projects to reorder; automatically switches to "Custom" sort mode.
- **Multi-IDE Import**: Import projects from VS Code, Trae, Trae CN, Cursor, and Windsurf with a selection dialog.
- **Remote Project Support**: Open SSH, Docker, WSL, Dev Container, and GitHub Codespaces projects correctly.
- **Task Management**: Create tasks with categories (bug, feature, refactor, docs, research, chore, experiment), priorities (critical, high, medium, low), and status tracking (backlog, todo, in_progress, review, done, blocked, cancelled).
- **Global Task View**: View and manage tasks across all projects in a unified interface.
- **Milestones**: Track project milestones with progress indicators and task linkage.
- **Lifecycle Tracking**: Automatic lifecycle inference (idea → planning → active → maintenance → archived).
- **Context Snapshots**: Save and restore project context (open files, cursor position, git branch).
- **Notes**: Rich text notes for each project.
- **Changelog**: Track project changes with versioned entries.
- **Batch Operations**: Select and delete multiple projects at once with a unified confirmation dialog.
- **Keyboard Navigation**: Full keyboard support with arrow keys, Enter, Ctrl+Enter, Delete, and `/` for search.
- **Data Validation**: Zod schema validation for all data with automatic migrations (v1 → v2 → v3).
- **Auto Backup**: Automatic backup before destructive operations.
- **Smart File Watcher**: MD5-based file change detection with debouncing.
- **Status Bar Integration**: Show current project and quick-switch in the status bar.
- **Task Reminders**: Due date reminders with configurable settings.
- **Settings Panel**: GitHub link, Get Started guide, and Report Issue quick access.

### Architecture

- React + TypeScript frontend with Zustand state management.
- Type-safe RPC communication between extension and webview.
- Dependency injection container for core modules.
- MessageQueue to guarantee no messages are lost during webview initialization.

### License

- Released under GPL-3.0.
