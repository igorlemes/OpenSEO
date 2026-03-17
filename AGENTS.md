# SEO Machine - OpenCode Port

A specialized OpenCode workspace for creating long-form, SEO-optimized blog content for any business. This system helps research, write, analyze, and optimize content that ranks well.

## Project Structure

```
seomachine/
├── .claude/
│   ├── commands/          # Custom workflow commands (22 total)
│   ├── agents/            # Specialized analysis agents (10 total)
│   └── skills/            # 26 marketing skills
├── data_sources/          # Analytics integrations & Python modules
├── context/               # Brand guidelines and SEO context
├── topics/                # Raw topic ideas
├── research/              # Research briefs and analysis reports
├── drafts/                # Work in progress articles
├── rewrites/              # Updated existing content
└── landing-pages/         # Landing page content
```

## Available Commands

### Core Content Commands
- `/research [topic]` - Keyword research and competitive analysis
- `/write [topic]` - Create SEO-optimized long-form article
- `/rewrite [topic]` - Update existing content
- `/optimize [file]` - Final SEO optimization pass
- `/article [topic]` - Simplified article creation
- `/scrub [file]` - Remove AI watermarks

### Analysis Commands
- `/analyze-existing [URL]` - Analyze existing blog post
- `/priorities` - Content prioritization matrix
- `/performance-review` - Analytics-driven content priorities

### Research Commands
- `/research-serp [keyword]` - SERP analysis
- `/research-gaps` - Competitor content gaps
- `/research-trending` - Trending topics
- `/research-performance` - Performance categorization
- `/research-topics` - Topic cluster research

### Landing Page Commands
- `/landing-write [topic]` - Create landing page
- `/landing-audit [file]` - Audit landing page
- `/landing-research [topic]` - Research positioning
- `/landing-competitor [URL]` - Competitor analysis
- `/landing-publish [file]` - Publish to WordPress

### Publishing
- `/publish-draft [file]` - Publish article to WordPress

## Context Files

Before creating content, review relevant context files in `context/`:
- `brand-voice.md` - Brand tone and messaging
- `writing-examples.md` - Sample articles
- `style-guide.md` - Formatting standards
- `seo-guidelines.md` - SEO requirements
- `internal-links-map.md` - Key pages for linking
- `target-keywords.md` - Priority keywords

## Dependencies

```bash
pip install -r data_sources/requirements.txt
```

## API Configuration

Configure credentials in `data_sources/config/.env`:
- GA4 (Google Analytics)
- GSC (Google Search Console)
- DataForSEO
- WordPress

## Agents

Specialized agents for content analysis:
- **SEO Optimizer** - On-page SEO recommendations
- **Meta Creator** - Generate meta titles/descriptions
- **Internal Linker** - Internal linking suggestions
- **Keyword Mapper** - Keyword placement analysis
- **Content Analyzer** - Comprehensive content scoring
- **Editor** - Humanize AI-generated content
- **Performance** - Analytics-driven priorities

## Skills

26 marketing skills are available for:
- Copywriting, CRO, Email sequences
- Pricing strategy, Launch strategy
- SEO audits, Schema markup
- And more...
