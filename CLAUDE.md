# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Monotasker Resources repository - a Hugo-based documentation site containing personas and prompts for the Monotasker ecosystem. It uses CloudCannon for content management and Bookshop for component-based page building.

## Development Commands

### Local Development
```bash
# Install dependencies
npm install

# Start Hugo development server (default port 1313)
npm start
# or
npm run dev:hugo
# or
hugo server

# Build the site for production (outputs to public/)
npm run build:hugo
# or
hugo --destination public
```

### Search & Discovery
```bash
# Build site and run Pagefind search server
npm run pagefind-server

# Run Pagefind search on existing build
npm run pagefind
```

### Component Development
```bash
# Create a new Bookshop component
npm run new-component

# Update Bookshop dependencies
npm run update-bookshop
```

## Architecture & Structure

### Content Collections

The site has four main content collections configured in CloudCannon:

1. **Pages** (`content/**/*.md` excluding blog/)
   - General site pages with component-based layouts
   - Uses visual editor in CloudCannon

2. **Blog** (`content/blog/`)
   - Blog posts with fixed layouts
   - Supports pagination and tags

3. **Personas** (`content/personas/`)
   - AI persona definitions for Monotasker
   - Fields: primary_role, industry, expertise_level, etc.

4. **Prompts** (`content/prompts/`)
   - Prompt templates and system instructions
   - Categories: System Prompts, User Prompts, Code Generation

### Component System

The site uses Bookshop for component-based page building:
- Components located in `component-library/components/`
- Available components: blog, buttons, heroes, left-right, processed-image, text-block
- Components are configured for CloudCannon's visual editor
- Shared styles and scripts in `component-library/shared/`

### Key Configuration Files

- **hugo.yaml**: Hugo configuration with module setup for Bookshop
- **cloudcannon.config.yml**: CloudCannon CMS configuration defining collections, schemas, and editor settings
- **tailwind.config.js**: Tailwind CSS configuration
- **package.json**: Node dependencies and scripts (requires Node >=22.16.0, pnpm >=10.14.0)

### Technology Stack

- **Hugo**: Static site generator with Go modules
- **Bookshop v3**: Component library system for Hugo
- **Tailwind CSS v4**: Utility-first CSS framework
- **CloudCannon**: Git-based CMS for content editing
- **Pagefind**: Static search functionality

## Important Notes

- The site uses Hugo modules with local component library replacement
- CloudCannon schemas are defined in `.cloudcannon/schemas/` for each content type
- Build stats are enabled for CSS cache busting
- Markdown rendering allows unsafe HTML and hard wraps
- The repository is optimized for CloudCannon editing workflows