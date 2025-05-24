# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands
- Serve site locally: `python -m http.server` (navigate to fractional/rue-du-four/)
- Deploy site: Use FTP to upload files to web server

## Project Architecture
This is a WordPress-based luxury real estate website with static landing pages for fractional properties. The main site uses the Avada theme with multiple plugins for functionality.

Key directories:
- `/elitedestinationhomes.com` - Main WordPress site with full infrastructure
- `/fractional/rue-du-four` - Static Paris property landing page (primary development focus)
- `/simplified/` - Simplified version of property page with clean HTML/CSS
- `/tmp/` - Working directory for development

The main property page (`fractional/rue-du-four/index.html`) is a large WordPress-generated file (1MB+) with extensive inline CSS and JavaScript. The simplified version provides a cleaner development starting point.

## Code Style Guidelines
- HTML: Follow semantic HTML5 standards with proper indentation (2 spaces)
- CSS: Use consistent class naming (kebab-case preferred)
- JavaScript: Follow ES6+ standards
- Image optimization: Compress all images before adding to repo
- Responsive design: All pages must be responsive across devices
- WordPress: Follow WordPress coding standards for plugin/theme development

## Development Workflow
When working on property landing pages:
1. Start with the simplified version for major changes
2. Test responsive design across mobile, tablet, and desktop
3. Ensure images are optimized and properly compressed
4. Maintain existing WordPress compatibility when modifying main site files

## Git Workflow
- Commit messages: Use conventional commits format
- Feature branches should be created for all new work
- Pull requests required for merging to main

When modifying code, maintain existing conventions in the files you're editing.