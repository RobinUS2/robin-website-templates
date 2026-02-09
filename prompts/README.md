# Prompt Templates

This directory contains all AI prompts used throughout the content generation system. Each prompt is stored as a plain text file with variable placeholders using `{{.VariableName}}` syntax.

## Available Templates

### Content Quality & Safety
- **safety_system.txt** / **safety_check.txt** - Content safety validation
- **adsense_system.txt** / **adsense_refinement.txt** - AdSense quality improvement
- **adsense_assessment_system.txt** / **adsense_assessment.txt** - AdSense value assessment
- **ai_analysis_system.txt** / **ai_analysis.txt** - AI-generated content detection
- **humanize_refinement.txt** - Humanize AI-generated content

### Content Improvement
- **claude_evaluation_system.txt** / **claude_evaluation.txt** - Evaluate if Claude would help
- **claude_improvement.txt** - Claude-powered technical content improvement (11KB)

### Content Generation Guidelines  
- **default_content_guidelines.txt** - Default content guidelines (basic)
- **content_guidelines.txt** - Comprehensive content guidelines with E-E-A-T

### Content Enhancement
- **link_gathering_system.txt** / **link_gathering.txt** - External link suggestions
- **image_decision_system.txt** / **image_decision.txt** - Image/visual value assessment
- **tag_generation_system.txt** / **tag_generation.txt** - Article tag generation

## Usage

```go
// Load a template with parameters
prompt, err := loadPromptTemplate("template_name", map[string]string{
    "Title": "Article Title",
    "Content": "Article content...",
})
```

## Benefits

- ✅ **Easy Editing** - Modify prompts without touching code
- ✅ **Version Control** - Track prompt changes independently
- ✅ **A/B Testing** - Test different prompt versions easily
- ✅ **Consistency** - Single source of truth for each prompt
- ✅ **Clarity** - Separates prompt content from application logic
