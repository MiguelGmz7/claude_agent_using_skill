# AI Research Workspace - Research Report Workflow

## What You Now Have

A complete research and reporting system with two interfaces:

### 🎯 Interactive Skill
```bash
/research-report "Your Topic"
```
Ask clarifying questions → Research → Generate beautiful HTML report

### 🤖 Background Agent
Spawn as an autonomous agent for batch research or integration into larger workflows.

---

## Quick Start

### Use 1: Fast Research Report
```bash
/research-report "Machine Learning in Healthcare"
```

You'll be asked:
1. How deep should the research go?
2. Who's your audience?
3. What 3-5 questions should it answer?
4. Any specific focus areas?

Then I'll research and create a professional HTML report.

### Use 2: Autonomous Background Task
```javascript
Agent({
  name: "researcher",
  description: "Research [topic]",
  prompt: "Research [topic]. Ask clarifying questions about scope, audience, and key questions. Generate HTML report."
})
```

---

## What You Get

Each report includes:

✅ **Executive Summary** - Quick overview  
✅ **Key Questions & Answers** - Your questions answered with sources  
✅ **Detailed Analysis** - Synthesized insights across sources  
✅ **Pro Tips** - 5-8 actionable takeaways  
✅ **Sources & Citations** - All links for verification  

Generated as clean, professional HTML with:
- Table of contents with navigation
- Professional styling
- Print-friendly formatting
- Mobile-responsive design
- Clickable source links

---

## Files & Structure

```
output/
└── reports/
    └── [topic]-[date].html          ← Your generated reports

workflow/
├── research-report-process.md       ← Detailed process steps
└── RESEARCH-QUICK-START.md          ← Quick reference

.claude/
├── skills/research-report.md        ← Skill definition
└── agents/research-reporter.md      ← Agent definition
```

---

## Key Features

🔍 **Thorough Research**
- Searches multiple authoritative sources
- Cross-references information
- Identifies themes and patterns

🎯 **Question-Driven**
- Ask clarifying questions first
- Research focused on YOUR questions
- Pro tips aligned with your needs

📊 **Clean Output**
- Professional HTML reports
- Easy to read and navigate
- Shareable and printable

⚡ **Flexible**
- Quick overview (3-4 hours)
- Comprehensive (5-7 hours)
- Expert deep dive (8+ hours)

---

## Examples

### Example 1: Quick Research
```
/research-report "Python Web Frameworks"
```
→ Gets a comprehensive comparison of Flask, Django, FastAPI

### Example 2: Background Task
```
Agent({ name: "researcher", prompt: "Research quantum computing. Focus on recent breakthroughs. Ask scope/audience questions." })
```
→ Runs autonomously while you work

---

## Report Examples

Reports are saved with clear naming:
- `climate-change-solutions-2026-10-20.html`
- `machine-learning-healthcare-2026-10-20.html`
- `renewable-energy-trends-2026-10-20.html`

Each is self-contained and shareable.

---

## Your Preferences Built In

This workflow follows your project guidelines:
- ✅ Clean, easy-to-understand syntax
- ✅ Clear, jargon-free output with pro tips
- ✅ Shows plan before executing
- ✅ Asks clarifying questions
- ✅ Cites all sources

---

## Next Steps

1. **Try it out:** `/research-report "A topic you're curious about"`
2. **Check results:** Open the generated HTML in your browser
3. **Refine:** Let me know if you want to adjust the report structure

---

## Advanced Usage

### Using as an Agent

```javascript
// Batch research multiple topics
Promise.all([
  Agent({ name: "research-1", prompt: "Research topic 1..." }),
  Agent({ name: "research-2", prompt: "Research topic 2..." }),
  Agent({ name: "research-3", prompt: "Research topic 3..." })
])
```

### Customizing Reports

Reports can be customized for:
- Different audience levels (general to expert)
- Different depths (overview to comprehensive)
- Different focuses (trends, how-to, comparisons, etc.)

---

## Documentation

- 📖 **RESEARCH-QUICK-START.md** - Start here for quick reference
- 📋 **research-report-process.md** - Detailed step-by-step process
- 🎯 **/research-report skill** - Use this to generate reports

---

## Questions?

The workflow is fully self-contained. Just invoke `/research-report "your topic"` and I'll guide you through the rest.

Happy researching! 🚀
