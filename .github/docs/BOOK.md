# BOOK AUTHORING GUIDELINES

This document contains specific instructions for writing technical books and chapters. These guidelines should be followed when users request book or chapter creation.

## BOOK-SPECIFIC WORKFLOW AND STRUCTURE

### MANDATORY WORKFLOW FOR CHAPTER CREATION

#### 1. PLANNING AND RESEARCH PHASE (REQUIRED)
Before writing ANY chapter content:
- Research the topic thoroughly using available tools
- Read WRITING-GUIDELINES.md and understand ALL requirements
- Study existing chapter structure and style patterns
- Examine solution directory to understand actual code implementation
- Verify file structure matches target language (Rust/TypeScript/etc.)
- Create detailed outline with learning progression
- Identify practical examples and real-world applications
- Plan code explanations with varied verbs for each block
- Design quiz questions (minimum 2) with clear correct answers

#### 2. CHAPTER STRUCTURE REQUIREMENTS (NON-NEGOTIABLE)
Every chapter MUST include these sections in order:
- **Title (H1)**: Engaging problem statement explaining why the topic matters
- **Introduction (H2)**: Overview with bullet list of what readers will learn
- **Learning Objectives (H2)**: Specific, measurable skills readers will gain
- **Main Content Sections (H2)**: 4-6 major concepts with proper progression
- **Assignment (H2)**: Practical exercise applying chapter concepts
- **Solution (H2)**: Complete solution with explanation
- **Quiz (H2)**: 1-2 questions with 3 options each (1 correct, 2 incorrect)
- **Summary (H2)**: Chapter recap with next steps

#### 3. BOOK-SPECIFIC WRITING STYLE REQUIREMENTS
- **Lead-in paragraphs**: ALL H1/H2 headers must have 1-3 paragraphs before sub-headers, lists, or code
- **Code presentation**: Show code "little by little" - break down blocks >10-15 lines
- **Code explanations**: Add bullet points after code using VARIED verbs (implements, provides, ensures, establishes, etc.). Each explanation bullet should mention the function and the parameters involved and show the code being explained.
- **Code consistency**: Solution code in chapter MUST match actual solution files exactly
- **Engaging tone**: Conversational yet professional, varied sentence structure
- **Real-world context**: Connect concepts to practical applications
- **Progressive complexity**: Start simple, build to advanced concepts
- **Section transitions**: Every section must flow naturally to the next with connecting sentences

## BOOK PROJECT STRUCTURE REQUIREMENTS

### Standard Book Directory Structure
```
book-project/
├── README.md                 # Main book overview
├── TOC.md                   # Table of contents
├── WRITING-GUIDELINES.md    # General writing guidelines
├── BOOK.md                  # This file - book-specific guidelines
└── chapters/
    ├── 01-chapter-name/
    │   ├── README.md        # Chapter content
    │   ├── assets/
    │   │   ├── data/
    │   │   ├── diagrams/
    │   │   └── images/
    │   └── solution/
    │       ├── [language-specific files]
    │       ├── src/
    │       ├── tests/
    │       └── README.md
    └── 02-next-chapter/
        └── [same structure]
```

### Chapter File Organization
Each chapter must follow this structure:
- **README.md**: Primary chapter content following structure requirements
- **assets/**: Supporting materials (images, diagrams, data files)
- **solution/**: Complete working code that matches chapter examples exactly

### Language-Specific File Structure
Ensure solution directory matches target language:
- **Go projects**: `main.go`, `go.mod`, appropriate package structure
- **TypeScript projects**: `package.json`, `.ts` files, proper module structure
- **Rust projects**: `Cargo.toml`, `src/main.rs`, proper crate structure
- **Python projects**: `requirements.txt`, proper package structure

## BOOK CONTENT STANDARDS

### Technical Content Requirements
- **Type safety**: Use proper type systems throughout with comprehensive interfaces
- **Security focus**: Emphasize security best practices in all examples
- **Production readiness**: Include error handling, logging, monitoring considerations
- **Testing**: Provide testable examples with proper separation of concerns
- **Documentation**: Clear code comments explaining security and design decisions

### Educational Content Requirements
- **Learning progression**: Each chapter builds on previous knowledge
- **Practical applications**: Every concept includes real-world examples
- **Hands-on exercises**: Assignments that reinforce chapter concepts
- **Assessment**: Quiz questions that test understanding effectively
- **Scaffolding**: Proper support for learners at different levels

## TABLE OF CONTENTS CREATION GUIDELINES

When creating TOC.md, structure each chapter with:

### Essential Elements per Chapter:
- **Problem statement**: Brief description of the problem and why it's important (2-3 sentences)
- **Learning objectives**: Bullet list of specific skills/knowledge readers will gain (4-6 items)
- **Key concepts**: 3 major concepts that will be covered
- **Exercises**: 2 practical exercises for hands-on learning
- **Quiz question**: 1 question testing understanding with 3 options
- **Major assignment**: 1 comprehensive project applying all concepts

### TOC Quality Standards:
- Progressive difficulty from basic to advanced concepts
- Clear dependencies between chapters
- Practical, real-world focus throughout
- Comprehensive skill development pathway
- Industry-relevant examples and scenarios

## BOOK QUALITY ASSURANCE CHECKLIST

### Pre-Completion Review Checklist
BEFORE declaring any chapter complete, perform this exhaustive check:

#### Structure Verification:
- ✅ Title engages and explains problem importance
- ✅ Introduction has bullet list of learning outcomes
- ✅ Learning objectives are specific and measurable
- ✅ 4-6 main content sections with logical progression
- ✅ Assignment applies all chapter concepts comprehensively
- ✅ Solution matches actual solution files exactly
- ✅ Quiz has 1-2 questions with 3 options each, clearly marked answers
- ✅ Summary provides recap and next steps

#### Writing Quality Verification:
- ✅ Every H1/H2 has 1-3 lead-in paragraphs before any sub-elements
- ✅ No code blocks exceed 10-15 lines without breakdown
- ✅ Every code block followed by bullet explanations with varied verbs
- ✅ Smooth transitions between all sections
- ✅ Engaging, conversational tone throughout
- ✅ Real-world examples and practical applications

#### Technical Accuracy Verification:
- ✅ Code examples are production-ready with proper error handling
- ✅ Solution code in chapter matches solution directory files
- ✅ File structure appropriate for target language
- ✅ Security considerations addressed where relevant
- ✅ Best practices demonstrated throughout

#### Educational Effectiveness Verification:
- ✅ Content builds logically from simple to complex
- ✅ Assignment tests all learning objectives
- ✅ Quiz questions effectively assess understanding
- ✅ Examples are immediately applicable
- ✅ Clear path for continued learning

## BOOK-SPECIFIC FAILURE CONDITIONS TO AVOID

Chapter authoring fails if:
- Missing any required sections (Title, Introduction, Learning Objectives, Main Content, Assignment, Solution, Quiz, Summary)
- Headers lack proper lead-in paragraphs
- Code blocks are too long without explanations
- Solution code differs from actual implementation files
- Quiz has fewer than 1 or more than 2 questions
- Code explanations lack varied verbs or proper bullet formatting
- Content jumps between concepts without transitions
- Examples are toy/academic rather than production-ready
- Security considerations are ignored or superficial
- File structure inappropriate for target language
- Sections end abruptly without connecting to next content

## BOOK REVIEW PROCESS

### Failed Review Recovery Process
If ANY checklist item fails:
1. **STOP writing immediately**
2. **Fix the specific issue completely**
3. **Re-read entire chapter for similar issues**
4. **Run through checklist again**
5. **Only proceed when ALL items pass**

### Real-Time Writing Checks for Books
While writing chapters, constantly verify:
- **After each header**: Do I have 1-3 lead-in paragraphs before sub-elements?
- **After each code block**: Do I have bullet explanations with varied verbs?
- **After each section**: Does this flow naturally to the next section?
- **For all code**: Does this match what's actually in the solution directory?
- **For complexity**: Is this code block >10 lines and needs breakdown?

### Common Book Pitfall Prevention
Based on frequent issues, specifically avoid:
- ❌ Jumping from headers directly to code/lists/sub-headers
- ❌ Code blocks longer than 15 lines without explanations
- ❌ Solution code that differs from actual files
- ❌ Quiz sections with only 1 question or unclear answer marking
- ❌ Code explanations using repetitive verbs (avoid multiple "provides" or "creates")
- ❌ Abrupt section endings without transitions
- ❌ Generic examples instead of production-ready scenarios

## BOOK SUCCESS METRICS

A successful chapter achieves:
- **Educational clarity**: Complex concepts explained simply
- **Practical value**: Immediately applicable knowledge
- **Production quality**: Professional-grade examples and practices
- **Engagement**: Maintains reader interest throughout
- **Completeness**: All learning objectives fully addressed
- **Security awareness**: Appropriate security considerations included
- **Progressive learning**: Builds effectively on previous knowledge
- **Assessment validity**: Quiz and assignments test intended learning outcomes

Remember: You're creating professional educational content that teaches practical, production-ready skills. Every chapter should be comprehensive, engaging, and immediately valuable to professional developers.