# Monotasker Resources - Local Context

## 📁 Repository Information
- **Name**: monotasker-resources
- **Path**: `/lib/monotasker-resources`
- **Purpose**: Documentation, guides, and educational content
- **Primary URL**: https://resources.monotasker.ai (planned)
- **Development Port**: 1313 (Hugo default)

## 🚀 Current Status: Structure Ready (20% Complete)

### ✅ What Exists
- **Hugo Configuration**: Basic Hugo site structure
- **CloudCannon CMS**: Configuration file present
- **Bookshop Components**: Component library setup
- **Tailwind CSS**: Configured for styling
- **Directory Structure**: Content folders created

### 📂 Current Structure
```
monotasker-resources/
├── .cloudcannon/          # CMS configuration
├── assets/                # Static assets
├── component-library/     # Bookshop components
│   └── components/       # Reusable components
├── content/              # Markdown content
├── data/                 # Data files (JSON/YAML)
├── layouts/              # Hugo templates
├── static/               # Static files
├── cloudcannon.config.yml # CMS config
├── hugo.yaml             # Hugo config
├── tailwind.config.js    # Tailwind setup
└── package.json          # Node dependencies
```

## 🛠️ Tech Stack Details

### Current Technologies
- **Static Site Generator**: Hugo (Go-based)
- **CMS**: CloudCannon
- **Component System**: Bookshop
- **Styling**: Tailwind CSS 4.x
- **Deployment**: CloudCannon Pages (planned)

### Configuration Status
- ✅ Hugo configuration exists
- ✅ Tailwind configured
- ✅ CloudCannon config present
- ⏳ No content created
- ⏳ No custom layouts
- ⏳ No components built

## 📚 Planned Content Structure

### Resource Categories

#### 1. Getting Started Guides
- What is Monotasker?
- Understanding PRPs
- Your First AI Strategy
- Choosing the Right Service Tier

#### 2. PRP Templates & Examples
- E-commerce PRP Template
- SaaS Product PRP Template
- Mobile App PRP Template
- Real-world PRP Examples

#### 3. AI Strategy Guides
- AI Readiness Assessment Guide
- Building Your First AI Agent
- Multi-Agent Orchestration
- Measuring AI ROI

#### 4. Case Studies
- Startup Success Stories
- Enterprise Transformations
- Before/After Comparisons
- Lessons Learned

#### 5. Technical Documentation
- API Reference (future)
- Integration Guides
- Webhook Documentation
- SDK Documentation

#### 6. Video Tutorials
- Platform Walkthroughs
- PRP Builder Tutorial
- Workflow Designer Guide
- Best Practices Series

#### 7. Community Resources
- Community Forum (planned)
- Monthly Webinars
- Office Hours Schedule
- Partner Directory

## 🎨 Design Requirements

### Brand Alignment
- Match main website styling
- Use same color palette (#8B5CF6, #F59E0B)
- Inter font family
- Consistent component design

### Unique Elements
- Documentation-focused layouts
- Code syntax highlighting
- Search functionality
- Table of contents navigation
- Version switcher (future)

## 📝 Content Management

### CloudCannon CMS Features
- Visual editor for non-technical users
- Component-based page building
- Content scheduling
- Multi-user collaboration
- Git-based workflow

### Content Workflow
1. **Draft**: Create in CloudCannon or markdown
2. **Review**: Technical review process
3. **Edit**: Copy editing and formatting
4. **Publish**: Deploy to production
5. **Update**: Regular content audits

## 🎯 Development Priorities

### Phase 1: Basic Setup (Next Wave)
1. [ ] Create base layouts
2. [ ] Build essential components
3. [ ] Set up navigation structure
4. [ ] Configure search
5. [ ] Deploy to staging

### Phase 2: Initial Content (1-2 Waves)
1. [ ] Write getting started guides
2. [ ] Create first PRP templates
3. [ ] Add FAQ section
4. [ ] Build glossary
5. [ ] Set up blog/updates section

### Phase 3: Enhanced Features (2-3 Waves)
1. [ ] Interactive examples
2. [ ] Video embedding
3. [ ] Download center
4. [ ] Search optimization
5. [ ] Analytics integration

## 🔧 Development Commands

### Local Development
```bash
# Install dependencies
npm install

# Start Hugo server
hugo server -D  # Includes drafts

# Build for production
hugo --minify

# Build Tailwind CSS
npm run build:css

# Watch Tailwind changes
npm run watch:css
```

### CloudCannon Development
```bash
# Serve for CloudCannon testing
npm run cloudcannon

# Build for CloudCannon
npm run build
```

## 🌐 Deployment Strategy

### Hosting Options
1. **CloudCannon Pages** (Preferred)
   - Automatic builds
   - Global CDN
   - SSL included
   - CMS integration

2. **Vercel** (Alternative)
   - Fast edge network
   - Automatic deploys
   - Analytics included

3. **Netlify** (Backup)
   - Form handling
   - Functions support
   - Split testing

### Domain Configuration
- Primary: resources.monotasker.ai
- Alternative: docs.monotasker.ai
- Legacy: help.monotasker.ai

## 📊 Content Metrics (Planned)

### Success Indicators
- Page views per resource
- Time on page
- Download counts
- Search queries
- User feedback scores

### Content Goals
- 50+ resources by launch
- 10+ PRP templates
- 5+ detailed case studies
- Weekly content updates
- 90% helpful rating

## 🔗 Integration Points

### With monotasker-website
- Shared navigation elements
- Cross-linking strategy
- Unified search (future)
- Same authentication (future)

### With monotasker-application
- Embedded documentation
- Context-sensitive help
- API documentation
- Template library

### External Integrations
- Google Analytics
- YouTube for videos
- GitHub for code examples

## 📋 Content Creation Guidelines

### Writing Style
- Clear and concise
- Action-oriented
- Example-heavy
- Visual aids when helpful
- Progressive disclosure

### Technical Standards
- Markdown with frontmatter
- Consistent formatting
- Proper code highlighting
- Alt text for images
- SEO optimization

### Review Process
1. Technical accuracy check
2. Brand voice alignment
3. SEO optimization
4. Accessibility review
5. Final approval

## 🚀 Quick Start for Development

### Set Up Local Environment
```bash
# Clone repository
cd ~/Development/monotasker/lib/monotasker-resources

# Install dependencies
npm install

# Start development server
hugo server -D

# In another terminal, watch CSS
npm run watch:css

# Visit http://localhost:1313
```

### Create First Content
```bash
# Create new guide
hugo new guides/getting-started.md

# Create new template
hugo new templates/saas-prp.md

# Create new case study
hugo new case-studies/startup-success.md
```

## 📌 Important Notes

### Current Blockers
- No content created yet
- Components need building
- Layouts need customization
- Search not configured
- No staging environment

### Dependencies
- Needs content strategy finalized
- Requires example PRPs from main app
- Needs real case studies
- Waiting for brand guidelines

### Opportunities
- Could be launched independently
- Good for SEO and marketing
- Community building platform
- Educational content hub

## 🔄 Last Activity
- **Setup**: Initial configuration done
- **Content**: None created yet
- **Last Update**: August 2025
- **Status**: Awaiting content creation wave

---
*This is the source of truth for monotasker-resources development*