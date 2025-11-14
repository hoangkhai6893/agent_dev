# Custom Agent Files for GitHub Copilot

This repository contains custom agent configurations for GitHub Copilot to enhance development workflows and improve productivity. These agents are specialized assistants that can be invoked to handle specific development tasks.

## 📋 Available Agents

### 1. **Code Reviewer Agent** (`code-reviewer.yml`)
Expert code reviewer that analyzes code changes and ensures quality standards.

**Key Capabilities:**
- Review code for correctness and best practices
- Identify bugs and security vulnerabilities
- Suggest improvements for maintainability
- Check test coverage and documentation

**When to Use:**
- Before merging pull requests
- During code reviews
- When refactoring existing code
- To get feedback on new implementations

### 2. **Documentation Writer Agent** (`documentation-writer.yml`)
Expert technical writer for creating comprehensive documentation.

**Key Capabilities:**
- Write clear README files
- Create API documentation
- Generate user guides and tutorials
- Write code comments and docstrings

**When to Use:**
- Starting new projects
- Documenting APIs or features
- Creating user guides
- Improving existing documentation

### 3. **Test Engineer Agent** (`test-engineer.yml`)
Expert test engineer for creating comprehensive test suites.

**Key Capabilities:**
- Create unit, integration, and e2e tests
- Identify test coverage gaps
- Design edge case scenarios
- Set up test frameworks

**When to Use:**
- Writing tests for new features
- Improving test coverage
- Testing edge cases
- Setting up testing infrastructure

### 4. **Debugging Assistant Agent** (`debugging-assistant.yml`)
Expert debugging assistant for identifying and fixing bugs.

**Key Capabilities:**
- Analyze error messages and stack traces
- Identify root causes of issues
- Suggest debugging strategies
- Add diagnostic logging

**When to Use:**
- Troubleshooting bugs
- Analyzing error logs
- Investigating performance issues
- When tests are failing

### 5. **Refactoring Specialist Agent** (`refactoring-specialist.yml`)
Expert refactoring specialist for improving code structure.

**Key Capabilities:**
- Identify code smells
- Reduce complexity and duplication
- Apply design patterns
- Improve code organization

**When to Use:**
- Improving legacy code
- Reducing technical debt
- Simplifying complex code
- Preparing for new features

### 6. **Security Analyst Agent** (`security-analyst.yml`)
Expert security analyst for identifying vulnerabilities.

**Key Capabilities:**
- Identify security vulnerabilities
- Review authentication and authorization
- Check for OWASP Top 10 issues
- Ensure secure coding practices

**When to Use:**
- Security audits
- Reviewing sensitive code
- Before production deployments
- When handling user data

### 7. **Performance Optimizer Agent** (`performance-optimizer.yml`)
Expert performance optimizer for improving application efficiency.

**Key Capabilities:**
- Identify performance bottlenecks
- Optimize algorithms and queries
- Improve caching strategies
- Reduce memory usage

**When to Use:**
- Performance issues
- Optimizing slow queries
- Reducing load times
- Scaling applications

### 8. **DevOps Engineer Agent** (`devops-engineer.yml`)
Expert DevOps engineer for CI/CD and infrastructure.

**Key Capabilities:**
- Set up CI/CD pipelines
- Configure Docker and Kubernetes
- Create infrastructure as code
- Implement monitoring and logging

**When to Use:**
- Setting up deployments
- Creating workflows
- Containerizing applications
- Automating infrastructure

### 9. **Frontend Developer Agent** (`frontend-developer.yml`)
Expert frontend developer for modern web development.

**Key Capabilities:**
- Implement responsive UI components
- Ensure accessibility standards
- Optimize frontend performance
- Handle state management

**When to Use:**
- Building user interfaces
- Implementing responsive designs
- Creating reusable components
- Frontend performance optimization

### 10. **Backend Developer Agent** (`backend-developer.yml`)
Expert backend developer for server-side development.

**Key Capabilities:**
- Design RESTful and GraphQL APIs
- Implement authentication/authorization
- Optimize database queries
- Handle business logic

**When to Use:**
- Creating API endpoints
- Database design
- Backend architecture
- Server-side logic

## 🚀 How to Use

### Using with GitHub Copilot

These custom agents are designed to work with GitHub Copilot's agent system. To use them:

1. **Invoke an agent in your development environment:**
   ```
   @agent-name [your request]
   ```

2. **Example usage:**
   ```
   @code-reviewer Review this pull request for potential issues
   @test-engineer Create unit tests for the UserService class
   @security-analyst Check for vulnerabilities in the authentication code
   ```

### Best Practices

1. **Choose the right agent:** Select the agent that best matches your task
2. **Be specific:** Provide clear context and requirements
3. **Iterate:** Agents can be called multiple times to refine solutions
4. **Combine agents:** Use multiple agents for complex tasks
5. **Review output:** Always review and validate agent suggestions

## 📁 Project Structure

```
.github/
└── agents/
    ├── code-reviewer.yml
    ├── documentation-writer.yml
    ├── test-engineer.yml
    ├── debugging-assistant.yml
    ├── refactoring-specialist.yml
    ├── security-analyst.yml
    ├── performance-optimizer.yml
    ├── devops-engineer.yml
    ├── frontend-developer.yml
    └── backend-developer.yml
```

## 🤝 Contributing

To add new custom agents:

1. Create a new YAML file in `.github/agents/`
2. Follow the existing agent structure:
   - `name`: Agent name
   - `description`: Brief description
   - `instructions`: Detailed instructions for the agent
   - `tools`: Available tools the agent can use
   - `examples`: Usage examples

3. Test the agent with various scenarios
4. Update this README with the new agent information

## 📝 Agent Configuration Format

Each agent configuration follows this structure:

```yaml
name: Agent Name
description: |
  Brief description of the agent's purpose

instructions: |
  Detailed instructions for the agent including:
  - Responsibilities
  - Best practices
  - Guidelines
  - Focus areas

tools:
  - view
  - edit
  - bash
  - github-mcp-server

examples:
  - description: Example scenario
    interaction: |
      User: User request
      Agent: Agent response
```

## 🎯 Use Cases

### Development Workflow
- **Start:** Use Documentation Writer for README and setup guides
- **Implement:** Use Frontend/Backend Developer for feature development
- **Test:** Use Test Engineer to create comprehensive tests
- **Review:** Use Code Reviewer for quality assurance
- **Debug:** Use Debugging Assistant for troubleshooting
- **Optimize:** Use Performance Optimizer and Refactoring Specialist
- **Secure:** Use Security Analyst for vulnerability checks
- **Deploy:** Use DevOps Engineer for CI/CD and deployment

### Common Scenarios

**Starting a new project:**
1. Documentation Writer → Create README and project structure
2. DevOps Engineer → Set up CI/CD pipelines
3. Frontend/Backend Developer → Implement core features
4. Test Engineer → Create test infrastructure

**Fixing a bug:**
1. Debugging Assistant → Identify root cause
2. Test Engineer → Create test case to reproduce
3. Frontend/Backend Developer → Implement fix
4. Code Reviewer → Review the fix

**Performance issues:**
1. Performance Optimizer → Identify bottlenecks
2. Refactoring Specialist → Improve code structure
3. Test Engineer → Add performance tests
4. Code Reviewer → Review changes

## 📚 Additional Resources

- [GitHub Copilot Documentation](https://docs.github.com/copilot)
- [Custom Agents Guide](https://github.com/github/copilot-docs)
- [Best Practices for AI-Assisted Development](https://github.com/features/copilot)

## 📄 License

This project is open source and available for use with GitHub Copilot.

---

**Note:** These agents are designed to assist developers and should be used as productivity tools. Always review and validate the suggestions provided by agents before applying them to production code.
