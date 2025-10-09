# BLOG POST AUTHORING GUIDELINES

This document contains specific instructions for writing technical blog posts that are engaging, educational, and professionally structured. These guidelines should be followed when users request blog post creation.

## BLOG-SPECIFIC WORKFLOW AND STRUCTURE

### MANDATORY WORKFLOW FOR BLOG POST CREATION

#### 1. PLANNING AND RESEARCH PHASE (REQUIRED)
Before writing ANY blog post content:
- Research the topic thoroughly using available tools
- Read WRITING-GUIDELINES.md and understand ALL requirements
- Study existing blog post structure and style patterns
- Examine solution directory to understand actual code implementation (if applicable)
- Verify file structure matches target language (Rust/TypeScript/etc.)
- Create detailed outline with logical flow
- Identify practical examples and real-world applications
- Plan code explanations with varied verbs for each block
- Design actionable takeaways for readers

#### 2. BLOG POST STRUCTURE REQUIREMENTS (NON-NEGOTIABLE)
Every blog post MUST include these sections in order:
- **Title (H1)**: Compelling headline that promises specific value and hooks the reader
- **Introduction (H2)**: Engaging opening that establishes the problem and previews the solution
- **Main Content Sections (H2)**: 3-5 focused sections that deliver on the title's promise
- **Code Examples/Demos (H2 or H3)**: Practical implementations when applicable
- **Key Takeaways (H2)**: Bullet list of actionable insights readers can apply immediately
- **Conclusion (H2)**: Summary with clear next steps or call-to-action
- **Resources (H2)**: Links to documentation, tools, or further reading

#### 3. BLOG-SPECIFIC WRITING STYLE REQUIREMENTS
- **Lead-in paragraphs**: ALL H1/H2 headers must have 1-3 paragraphs before sub-headers, lists, or code
- **Code presentation**: Show code "little by little" - break down blocks >10-15 lines
- **Code explanations**: Add bullet points after code using VARIED verbs (implements, provides, ensures, establishes, etc.). Each explanation bullet should mention the function and the parameters involved and show the code being explained.
- **Code consistency**: Solution code in blog post MUST match actual solution files exactly
- **Conversational tone**: More casual than book chapters, but still professional
- **Immediate value**: Each section should provide actionable insights
- **Scannable format**: Use headers, bullet points, and visual breaks for easy reading
- **Hook retention**: Keep readers engaged throughout with compelling examples and insights

## BLOG PROJECT STRUCTURE REQUIREMENTS

### Standard Blog Directory Structure
```
blog-project/
├── README.md                 # Blog project overview
├── WRITING-GUIDELINES.md    # General writing guidelines
├── BLOG.md                  # This file - blog-specific guidelines
└── posts/
    ├── 2024-10-09-post-title/
    │   ├── README.md        # Blog post content
    │   ├── assets/
    │   │   ├── images/
    │   │   ├── diagrams/
    │   │   └── screenshots/
    │   └── code/
    │       ├── [language-specific files]
    │       ├── examples/
    │       └── README.md
    └── 2024-10-10-next-post/
        └── [same structure]
```

### Blog Post File Organization
Each blog post must follow this structure:
- **README.md**: Primary blog post content following structure requirements
- **assets/**: Supporting materials (images, diagrams, screenshots)
- **code/**: Complete working code examples that match blog post exactly

### Language-Specific File Structure for Code Examples
Ensure code directory matches target language:
- **Go projects**: `main.go`, `go.mod`, appropriate package structure
- **TypeScript projects**: `package.json`, `.ts` files, proper module structure
- **Rust projects**: `Cargo.toml`, `src/main.rs`, proper crate structure
- **Python projects**: `requirements.txt`, proper package structure

## BLOG CONTENT STANDARDS

### Technical Content Requirements
- **Practical focus**: Every code example should solve a real problem
- **Production readiness**: Include error handling and best practices
- **Security awareness**: Address security considerations when relevant
- **Performance considerations**: Mention optimization opportunities
- **Clear explanations**: Assume intelligent but not expert audience

### Blog-Specific Content Requirements
- **Problem-solution format**: Start with a relatable problem, build to solution
- **Immediate applicability**: Readers should be able to use insights right away
- **Personal insights**: Share lessons learned and practical experience
- **Community value**: Address common questions or challenges
- **Engaging narrative**: Tell a story that keeps readers interested

## BLOG POST STRUCTURE BREAKDOWN

### Title Requirements
- **Specific promise**: Tell readers exactly what they'll learn
- **Benefit-focused**: Emphasize the value they'll gain
- **Search-friendly**: Include relevant keywords naturally
- **Length**: 50-70 characters for optimal sharing

### Introduction Requirements
The introduction must:
- **Hook immediately**: Start with a relatable problem or surprising insight
- **Establish credibility**: Show you understand the reader's challenges
- **Preview value**: Outline what readers will gain
- **Set expectations**: Indicate time investment and skill level needed

### Main Content Section Guidelines
Each section should:
- **Address one key concept**: Stay focused on a single idea
- **Build progressively**: Each section should build on previous knowledge
- **Include practical examples**: Show concepts in action
- **Provide immediate value**: Readers should gain something from each section

### Code Example Standards
- **Complete and runnable**: All code should work as shown
- **Well-commented**: Explain complex logic and design decisions
- **Error handling**: Include appropriate error handling
- **Best practices**: Demonstrate professional coding standards
- **Progressive complexity**: Start simple, add sophistication gradually

### Key Takeaways Requirements
- **Actionable insights**: Each point should be immediately applicable
- **Specific guidance**: Avoid vague advice
- **Prioritized list**: Most important insights first
- **Clear language**: No jargon or unnecessarily complex explanations

### Conclusion Guidelines
- **Summarize value delivered**: Recap what readers learned
- **Suggest next steps**: Provide clear guidance for continued learning
- **Include call-to-action**: Encourage engagement (comments, sharing, etc.)
- **Leave lasting impression**: End with memorable insight or challenge

## BLOG QUALITY ASSURANCE CHECKLIST

### Pre-Completion Review Checklist
BEFORE declaring any blog post complete, perform this exhaustive check:

#### Structure Verification:
- ✅ Title promises specific, valuable outcome
- ✅ Introduction hooks readers and establishes value proposition
- ✅ 3-5 main content sections with logical progression
- ✅ Code examples are complete and well-explained
- ✅ Key takeaways provide actionable insights
- ✅ Conclusion summarizes value and provides next steps
- ✅ Resources section includes relevant links

#### Writing Quality Verification:
- ✅ Every H1/H2 has 1-3 lead-in paragraphs before any sub-elements
- ✅ No code blocks exceed 10-15 lines without breakdown
- ✅ Every code block followed by bullet explanations with varied verbs
- ✅ Smooth transitions between all sections
- ✅ Conversational, engaging tone throughout
- ✅ Scannable format with appropriate headers and breaks

#### Technical Accuracy Verification:
- ✅ Code examples are production-ready and runnable
- ✅ Solution code in blog post matches code directory files
- ✅ File structure appropriate for target language
- ✅ Security considerations addressed where relevant
- ✅ Best practices demonstrated throughout

#### Reader Value Verification:
- ✅ Content delivers on title's promise
- ✅ Immediate applicability of insights
- ✅ Clear progression from problem to solution
- ✅ Actionable takeaways provided
- ✅ Engaging narrative maintains interest

### Failed Review Recovery Process
If ANY checklist item fails:
1. **STOP writing immediately**
2. **Fix the specific issue completely**
3. **Re-read entire blog post for similar issues**
4. **Run through checklist again**
5. **Only proceed when ALL items pass**

## BLOG-SPECIFIC FAILURE CONDITIONS TO AVOID

Blog post authoring fails if:
- Title doesn't promise specific value or is too vague
- Introduction fails to hook readers or establish clear value
- Content doesn't deliver on title's promise
- Code examples are incomplete or don't work
- Missing actionable takeaways
- Conclusion lacks clear next steps
- Content is too academic rather than practical
- Poor scannable format (walls of text)
- Code explanations lack varied verbs or proper bullet formatting
- Content jumps between concepts without transitions
- Examples are toy/academic rather than real-world applicable

## BLOG POST OPTIMIZATION GUIDELINES

### SEO and Discoverability
- **Keyword integration**: Include relevant keywords naturally throughout
- **Meta description**: Summarize value proposition in 150-160 characters
- **Header hierarchy**: Use proper H1-H6 structure for search engines
- **Internal linking**: Link to related content when relevant
- **Image optimization**: Include alt text and descriptive filenames

### Social Media Optimization
- **Shareable quotes**: Include tweetable insights and key takeaways
- **Visual elements**: Add diagrams, screenshots, or code samples for social sharing
- **Engaging introduction**: First paragraph should work well as a social media preview
- **Clear value proposition**: Make benefits obvious for social sharing

### Reader Engagement
- **Scannable format**: Use headers, bullet points, and white space effectively
- **Visual breaks**: Include code blocks, diagrams, or images to break up text
- **Call-to-action**: Encourage comments, questions, or sharing
- **Community building**: Invite readers to share their experiences or questions

## BLOG SUCCESS METRICS

A successful blog post achieves:
- **Immediate value**: Readers gain actionable insights they can apply right away
- **Clear communication**: Complex concepts explained in accessible language
- **Practical application**: Examples that readers can implement in their work
- **Engagement**: Maintains reader interest throughout
- **Shareability**: Content that readers want to share with colleagues
- **Searchability**: Discoverable by people facing similar challenges

## BLOG REVIEW PROCESS

### Real-Time Writing Checks for Blog Posts
While writing, constantly verify:
- **After each header**: Do I have 1-3 lead-in paragraphs before sub-elements?
- **After each code block**: Do I have bullet explanations with varied verbs?
- **After each section**: Does this deliver immediate value to readers?
- **For all code**: Does this match what's actually in the code directory?
- **For complexity**: Is this code block >10 lines and needs breakdown?
- **For engagement**: Would I want to keep reading if I found this online?

### Common Blog Pitfall Prevention
Based on frequent issues, specifically avoid:
- ❌ Titles that are too vague or don't promise specific value
- ❌ Jumping from headers directly to code/lists/sub-headers
- ❌ Code blocks longer than 15 lines without explanations
- ❌ Academic tone instead of conversational, practical approach
- ❌ Missing actionable takeaways readers can implement
- ❌ Abrupt endings without clear next steps
- ❌ Generic examples instead of real-world scenarios

### Quality Gates for Blog Posts
Stop and review if you find yourself:
- Writing a header followed immediately by code
- Creating academic explanations instead of practical insights
- Using jargon without explanation
- Writing code blocks longer than 10 lines
- Ending sections without clear value delivery
- Creating content that doesn't deliver on the title's promise

## BLOG-SPECIFIC CONTENT TYPES

### Tutorial Posts
- **Step-by-step guidance**: Clear, sequential instructions
- **Prerequisites**: What readers need to know or have installed
- **Expected outcomes**: What readers will accomplish
- **Troubleshooting**: Common issues and solutions

### Comparison Posts
- **Clear criteria**: Objective comparison factors
- **Real-world scenarios**: When to use each option
- **Pros and cons**: Honest assessment of trade-offs
- **Recommendations**: Clear guidance for different use cases

### Problem-Solution Posts
- **Relatable problem**: Challenge many developers face
- **Investigation process**: How you approached the problem
- **Solution explanation**: Why this approach works
- **Alternative approaches**: Other ways to solve the problem

### Experience Sharing Posts
- **Lessons learned**: Insights from real projects
- **Mistakes and recoveries**: What went wrong and how you fixed it
- **Best practices**: Guidelines discovered through experience
- **Community wisdom**: Insights that help other developers

Remember: Blog posts should provide immediate, practical value to working developers. Every post should leave readers with actionable insights they can apply in their work right away. Focus on solving real problems and sharing genuine insights from experience.