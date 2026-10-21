# Research Report Workflow - Quick Start Guide

## Two Ways to Use This Workflow

### Option 1: Interactive Skill Command
```bash
/research-report "Your Topic Here"
```

**Best for:** When you want to guide the research interactively and see results quickly.

**Flow:**
1. You type the command with a topic
2. I ask 4 clarifying questions
3. I research and generate the report
4. Report saved to `output/reports/`

### Option 2: Background Agent
```javascript
Agent({
  name: "research-reporter",
  description: "Research report on [topic]",
  prompt: "Research [topic]. Ask clarifying questions about scope, audience, and key questions. Generate HTML report."
})
```

**Best for:** Autonomous research tasks, batch processing, or research while you work on other things.

---

## What Happens in the Workflow

### Step 1: Clarification (Your Input)
Answer 4 quick questions:
- **How deep?** Overview / Comprehensive / Expert
- **Who reads it?** General / Professionals / Executives / Students
- **What to answer?** List 3-5 specific questions
- **Any focus areas?** (optional) Trends, comparisons, how-tos, etc.

### Step 2: Research (My Work)
- Search for 5-8 authoritative sources per question
- Cross-reference information
- Identify themes and patterns
- Note conflicting viewpoints

### Step 3: Report Generation (My Output)
Clean HTML report with:
- **Executive Summary** - Quick overview
- **Key Questions & Answers** - Your questions answered
- **Detailed Analysis** - Synthesized insights
- **Pro Tips** - 5-8 actionable takeaways
- **Sources & Citations** - All links and references

### Step 4: Storage
Saved to: `output/reports/[topic]-[date].html`

Example: `machine-learning-healthcare-2026-10-20.html`

---

## Report Quality Levels

### Quick Overview (3-4 hours)
- 200-300 words per question
- 3-4 sources per question
- High-level synthesis
- Basic pro tips

### Comprehensive (5-7 hours)
- 400-500 words per question
- 5-6 sources per question
- Detailed analysis with themes
- Specific, actionable pro tips

### Expert Deep Dive (8+ hours)
- 600+ words per question
- 8+ sources per question
- Cutting-edge findings
- Advanced insights and trends

---

## Example: How to Use

```
You: /research-report "Climate Change Solutions"

I ask:
- Depth? → You: "Comprehensive"
- Audience? → You: "General public"
- Key questions? → You: "What are the most effective solutions? What's the timeline? What's the role of businesses?"
- Focus areas? → You: "Emerging technologies and policy initiatives"

I research...

I generate HTML report → Saved to output/reports/climate-change-solutions-2026-10-20.html
```

---

## File Structure

```
/mnt/Data/User/agents-2/
├── output/
│   └── reports/
│       ├── machine-learning-healthcare-2026-10-20.html
│       ├── climate-solutions-2026-10-20.html
│       └── [topic]-[date].html
├── workflow/
│   ├── research-report-process.md (detailed process)
│   └── RESEARCH-QUICK-START.md (this file)
└── CLAUDE.md
```

---

## Pro Tips for Getting Better Reports

1. **Be Specific with Questions** - "What are the latest ML techniques?" is better than "Tell me about AI"
2. **Know Your Audience** - Different audiences need different depth and language
3. **Focus Helps** - "Emerging technologies in healthcare" gives better results than just "healthcare"
4. **Recent Topics** - Current events get better, fresher research
5. **Check the Sources** - All sources are linked and clickable for verification

---

## Reports Generated So Far

Check `output/reports/` to see all generated reports.

---

## Commands Reference

| Command | Purpose |
|---------|---------|
| `/research-report "topic"` | Interactive research and report generation |
| Check `output/reports/` | View all saved reports |
| Open HTML file in browser | View generated report |

---

## Questions?

Refer to:
- `research-report-process.md` - Detailed workflow steps
- `/research-report` skill - For interactive use
- research-reporter agent - For autonomous use
