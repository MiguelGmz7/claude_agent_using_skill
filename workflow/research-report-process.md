# Research Report Generation Process

## Overview
This workflow guides the research and report generation process. It's used by both the `/research-report` skill and the research-reporter agent.

## Process Steps

### Phase 1: Clarification (5-10 min)
Ask the user four clarifying questions:

1. **Research Depth**
   - [ ] Quick Overview (2-3 hours research, high-level summary)
   - [ ] Comprehensive (4-6 hours research, detailed analysis)
   - [ ] Expert Deep Dive (6+ hours, cutting-edge insights)

2. **Target Audience**
   - [ ] General public (no jargon)
   - [ ] Professionals (industry-specific terms OK)
   - [ ] Executives (focus on ROI, trends)
   - [ ] Students (educational, foundational)
   - [ ] Other (specify)

3. **Key Questions** (3-5 questions)
   - Record exactly what the user wants to know
   - These become the "Key Questions & Answers" section

4. **Focus Areas** (optional)
   - Trends? History? How-to? Comparison? Emerging developments?

### Phase 2: Research (2-6 hours depending on scope)

#### For Each User Question:
1. Conduct 2-3 targeted web searches
2. Note 3-5 reliable sources per question
3. Extract key facts and insights
4. Identify consensus and conflicting viewpoints

#### Search Strategy:
- Use WebSearch with focused queries
- Prioritize recent, authoritative sources
- Look for peer-reviewed research when possible
- Cross-reference multiple sources

#### Organize Findings:
- Group by theme
- Note source attribution
- Highlight conflicting opinions
- Identify knowledge gaps

### Phase 3: Synthesis (30-60 min)

Create sections:

1. **Executive Summary** (100-150 words)
   - What's the big picture?
   - Why should people care?
   - Key takeaway in one sentence

2. **Key Questions & Answers** (200-400 words per question)
   - Answer each user question directly
   - Support with evidence
   - Cite sources inline

3. **Detailed Analysis** (300-500 words)
   - Synthesize across sources
   - Identify themes and patterns
   - Note emerging trends
   - Flag contradictions

4. **Pro Tips** (5-8 actionable items)
   - Practical takeaways
   - Best practices
   - Tools/resources
   - Next steps

5. **Sources & Citations**
   - Full list with links
   - Author, date, credibility note

### Phase 4: HTML Generation (15-30 min)

Generate HTML with:
- Professional styling (clean, readable)
- Table of contents with navigation
- Section headers with anchors
- Clickable source links
- Print-friendly CSS
- Mobile-responsive layout
- Generated date and scope metadata

Template structure:
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>[Topic] Research Report</title>
  <style>[Professional CSS styling]</style>
</head>
<body>
  <header>
    <h1>[Topic] Research Report</h1>
    <div class="metadata">
      <p>Generated: [Date]</p>
      <p>Research Depth: [User's choice]</p>
      <p>Audience: [Target audience]</p>
    </div>
  </header>
  
  <nav class="toc">
    <h2>Contents</h2>
    <ul>
      <li><a href="#summary">Executive Summary</a></li>
      <li><a href="#questions">Key Questions & Answers</a></li>
      <li><a href="#analysis">Detailed Analysis</a></li>
      <li><a href="#tips">Pro Tips</a></li>
      <li><a href="#sources">Sources</a></li>
    </ul>
  </nav>
  
  <main>
    <section id="summary">
      <h2>Executive Summary</h2>
      [Content]
    </section>
    
    <section id="questions">
      <h2>Key Questions & Answers</h2>
      <div class="qa-item">
        <h3>Question 1</h3>
        <p>[Answer with citations]</p>
      </div>
      <!-- Repeat for each question -->
    </section>
    
    <section id="analysis">
      <h2>Detailed Analysis</h2>
      [Content with themes and synthesis]
    </section>
    
    <section id="tips">
      <h2>Pro Tips</h2>
      <ol>
        <li>[Actionable item]</li>
        <!-- Repeat for each tip -->
      </ol>
    </section>
    
    <section id="sources">
      <h2>Sources & Citations</h2>
      <ol class="sources">
        <li><a href="[URL]">[Title]</a> - [Author/Publication], [Date]</li>
        <!-- Repeat for each source -->
      </ol>
    </section>
  </main>
  
  <footer>
    <p>Generated with Claude Code Research Workflow</p>
  </footer>
</body>
</html>
```

### Phase 5: Output & Storage

Save HTML file:
- Location: `output/reports/[topic-slugified]-[date].html`
- Naming example: `machine-learning-healthcare-2026-10-20.html`
- Make self-contained (no external dependencies)

## Quality Checklist

Before finalizing, verify:

- [ ] All user questions are answered clearly
- [ ] Pro Tips are actionable and specific
- [ ] Sources are cited with links
- [ ] No jargon for general audiences (or explained if unavoidable)
- [ ] HTML renders cleanly in browser
- [ ] Print preview looks professional
- [ ] Report matches the requested research depth
- [ ] Metadata (date, scope, audience) is visible

## Time Estimates

- Quick Overview: 3-4 hours total
- Comprehensive: 5-7 hours total
- Expert Deep Dive: 8+ hours total

## Pro Tips for Researchers

1. **Search Strategy:** Start broad, then narrow based on findings
2. **Source Credibility:** Prioritize .edu, .org, peer-reviewed, and established publications
3. **Conflicting Info:** Note and explain when sources disagree
4. **Current Trends:** Include 3-5 very recent findings for current topics
5. **Actionability:** Pro Tips should be immediately usable
6. **Clear Language:** Assume reader isn't expert in the topic
