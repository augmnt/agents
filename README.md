# Claude Code Sub-Agents Collection

A comprehensive collection of specialized sub-agents for Claude Code, designed to enhance development workflows through domain-specific expertise and intelligent task delegation.

## What are Sub-Agents?

Sub-agents are specialized AI assistants in Claude Code that focus on specific domains of software engineering. They provide expert-level guidance, automate complex tasks, and coordinate with other agents to deliver comprehensive solutions. Learn more in the [official documentation](https://docs.anthropic.com/en/docs/claude-code/sub-agents).

## Agent Categories

### 🏗️ Architecture & Design
- **[backend-architect](./backend-architect.md)** - Scalable API architectures, authentication systems, database schemas, and microservices design
- **[frontend-specialist](./frontend-specialist.md)** - Modern React applications, shadcn/ui components, Tailwind CSS, and accessibility compliance
- **[fullstack-developer](./fullstack-developer.md)** - End-to-end feature implementation with frontend-backend integration
- **[iac-expert](./iac-expert.md)** - Infrastructure as Code, cloud resources, and scalability planning
- **[ui-ux-designer](./ui-ux-designer.md)** - Stunning, unique, and modern user interfaces with exceptional visual design and seamless interactions

### 🧪 Testing & Quality Assurance
- **[test-architect](./test-architect.md)** - Comprehensive test strategies, coverage analysis, and quality assurance planning
- **[unit-test-generator](./unit-test-generator.md)** - Component-level tests with comprehensive edge cases and high coverage
- **[e2e-test-automator](./e2e-test-automator.md)** - End-to-end user journey testing with Playwright
- **[integration-test-builder](./integration-test-builder.md)** - API testing, database testing, and service interaction validation

### 🔒 Security & Compliance
- **[security-auditor](./security-auditor.md)** - OWASP compliance, vulnerability assessments, and security architecture evaluation
- **[code-reviewer](./code-reviewer.md)** - Code quality, security review, and best practices enforcement

### ⚡ Performance & Monitoring
- **[performance-profiler](./performance-profiler.md)** - Performance bottleneck identification and optimization
- **[monitoring-architect](./monitoring-architect.md)** - System observability, alerting, and performance dashboards

### 🚀 DevOps & Deployment
- **[cicd-engineer](./cicd-engineer.md)** - CI/CD pipelines, automated builds, and deployment management
- **[docker-specialist](./docker-specialist.md)** - Container optimization and orchestration
- **[config-expert](./config-expert.md)** - Environment configuration and secrets management

### 🛠️ Development & Maintenance
- **[database-engineer](./database-engineer.md)** - Database schema design, query optimization, and migrations
- **[refactoring-expert](./refactoring-expert.md)** - Technical debt reduction and design pattern implementation
- **[error-detective](./error-detective.md)** - Bug analysis, root cause identification, and fix implementation
- **[dependency-manager](./dependency-manager.md)** - Safe dependency updates and compatibility verification
- **[mindful-dev](./mindful-dev.md)** - Thoughtful development with educational focus, breaking down complex tasks into digestible learning steps

### 📚 Documentation & Release
- **[tech-writer](./tech-writer.md)** - Technical documentation, API docs, and user guides
- **[release-compiler](./release-compiler.md)** - Release notes, migration guides, and changelog compilation
- **[code-commentator](./code-commentator.md)** - Inline documentation and code explanation

### 🎯 Project Management
- **[project-orchestrator](./project-orchestrator.md)** - Complex project coordination and multi-agent workflow management
- **[migration-specialist](./migration-specialist.md)** - Schema and data migrations with safety validation

## Usage Examples

### Project Orchestrator Template

Use this template to start any project with Claude Code. This will automatically engage the project-orchestrator sub agent to analyze your requirements and delegate tasks to the appropriate specialized agents:

```
Use project-orchestrator sub agent to build [WHAT YOU WANT].

Name: [PROJECT NAME]
Type: [APPLICATION TYPE - Web App/API/Mobile/CLI/etc]
Goal: [MAIN OBJECTIVE - What problem does this solve?]
Features: [KEY FEATURES - List core functionality]
Tech Stack:
  - Frontend: [e.g., Vue, Next.js, React, Angular]
  - Backend: [e.g., Node.js, Python/Django, Go]
  - Database: [e.g., PostgreSQL, MongoDB, Redis]
  - Other: [e.g., Docker, AWS, Authentication method]
Priority: [WHAT MATTERS MOST - Speed/Security/Scalability/UX/Performance]
Constraints: [ANY LIMITATIONS - Budget/Time/Platform/Compliance]

Analyze requirements, create comprehensive project plan, and delegate to all necessary sub agents for complete implementation.
```

**Tips:**
- Be specific about your features to get better results
- Tech Stack sections are optional - remove any that don't apply
- The project-orchestrator will automatically identify and engage the right sub-agents
- For frontend-only projects, simply omit Backend/Database/Other sections

### Basic Agent Invocation
```bash
# Use a specific agent for a focused task
claude --agent security-auditor "Review this authentication flow for vulnerabilities"
claude --agent frontend-specialist "Create a responsive navbar component with shadcn/ui"
```

### Project Orchestration
```bash
# Let the project orchestrator coordinate multiple agents
claude --agent project-orchestrator "Build a user management system with authentication, CRUD operations, and admin dashboard"
```

### Sequential Agent Workflows
```bash
# Chain agents for comprehensive coverage
claude --agent backend-architect "Design the API structure" \
      --agent security-auditor "Review the security implications" \
      --agent test-architect "Create a testing strategy"
```

## Key Features

### 🤖 Automatic Delegation
Many agents automatically delegate tasks to appropriate specialists:
- **backend-architect** → **security-auditor** for vulnerability assessment
- **frontend-specialist** → **performance-profiler** for optimization
- **project-orchestrator** → Multiple agents based on project requirements

### 🎯 Domain Expertise
Each agent provides:
- Specialized knowledge in their domain
- Best practices and industry standards
- Framework-specific guidance
- Performance optimization techniques

### 🔄 Intelligent Coordination
Agents work together to:
- Avoid duplicate work
- Ensure consistency across domains
- Share context and requirements
- Validate cross-domain compatibility

## Best Practices

### When to Use Specific Agents

**Use `project-orchestrator`** when:
- Starting a new feature or project
- Requirements span multiple domains
- You need coordination between frontend, backend, and testing

**Use domain specialists** when:
- You have a specific technical challenge
- You need expert-level guidance in one area
- You want focused, high-quality output

**Use `test-architect`** when:
- Planning testing strategies
- Setting up new test infrastructure
- Defining quality gates and coverage goals

### Agent Selection Tips

1. **Start Broad**: Use `project-orchestrator` for complex, multi-faceted tasks
2. **Go Specific**: Use domain experts for focused technical work
3. **Chain Workflows**: Combine agents for comprehensive coverage
4. **Leverage Auto-Delegation**: Let agents coordinate with each other

## Installation & Setup

### Quick Installation
To make these agents globally accessible in Claude Code, copy all `.md` files to your Claude Code agents directory:

```bash
# Copy all agent files to make them globally accessible
cp *.md ~/.claude/agents/

# Or clone and copy from this repository
git clone <repository-url>
cd sub-agents
cp *.md ~/.claude/agents/
```

### Verify Installation
Check that agents are available:
```bash
ls ~/.claude/agents/
# Should show all 25 agent files
```

## Integration with Claude Code

### Configuration
Agents are automatically available in Claude Code once placed in the agents directory. No additional configuration required.

### Memory Integration
Agents work with Claude Code's memory system to:
- Remember project context across sessions
- Share knowledge between agents
- Maintain consistency in recommendations

## Contributing

This collection is open source and welcomes contributions:

1. **New Agents**: Create new domain-specific agents following the existing patterns
2. **Agent Improvements**: Enhance existing agents with better delegation patterns or expertise
3. **Documentation**: Improve usage examples and best practices
4. **Integration Patterns**: Develop better inter-agent coordination strategies

### Agent Structure
Each agent follows this structure:
```yaml
---
name: agent-name
description: When and how to use this agent
tools: List of available tools
---

# Agent content with expertise areas, processes, and integration points
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For issues, questions, or contributions:
- 📖 [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)  
- 🐛 [Report Issues](https://github.com/anthropics/claude-code/issues)
- 💡 [Feature Requests](https://github.com/anthropics/claude-code/issues)

## Quick Reference

| Task Type | Recommended Agent | Alternative Agents |
|-----------|-------------------|-------------------|
| New Project | `project-orchestrator` | `backend-architect`, `frontend-specialist` |
| API Design | `backend-architect` | `security-auditor`, `database-engineer` |
| UI Components | `frontend-specialist` | `ui-ux-designer`, `fullstack-developer` |
| UI/UX Design | `ui-ux-designer` | `frontend-specialist` |
| Testing Strategy | `test-architect` | `unit-test-generator`, `e2e-test-automator` |
| Performance Issues | `performance-profiler` | `monitoring-architect` |
| Security Review | `security-auditor` | `code-reviewer` |
| Bug Fixing | `error-detective` | `code-reviewer` |
| Documentation | `tech-writer` | `code-commentator` |
| Deployment | `cicd-engineer` | `docker-specialist`, `iac-expert` |
| Learning & Education | `mindful-dev` | `tech-writer`, `code-commentator` |

---

*Enhance your development workflow with intelligent, specialized assistance for every aspect of software engineering.*