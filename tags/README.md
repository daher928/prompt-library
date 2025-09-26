# Tags System

This directory manages the tagging and categorization system for the prompt library, enabling efficient discovery and organization of prompts.

## Purpose

The `tags` directory serves as the centralized management system for:

- **Tag Definitions**: Standardized definitions and descriptions for all tags
- **Category Hierarchies**: Organizational structure and relationships between tags
- **Search Metadata**: Information to optimize search and filtering capabilities
- **Tag Usage Statistics**: Tracking which tags are most commonly used
- **Synonym Management**: Handling alternative terms and related concepts

## File Structure

```
tags/
├── README.md                    # This file
├── tag-definitions.json         # Complete list of tags with definitions
├── categories.json              # Hierarchical category structure
├── synonyms.json                # Tag synonyms and aliases
├── usage-stats.json             # Tag usage frequency and statistics
└── validation-rules.json        # Rules for tag validation and consistency
```

## Tag Categories

### Primary Categories

1. **Content Type**
   - `creative-writing`: Fiction, poetry, storytelling
   - `technical-writing`: Documentation, tutorials, explanations
   - `business`: Professional communications, proposals, reports
   - `educational`: Teaching materials, explanations, summaries
   - `conversational`: Dialogue, chat, interactive responses

2. **Use Case**
   - `content-generation`: Creating new content from scratch
   - `content-improvement`: Editing, refining, enhancing existing content
   - `analysis`: Reviewing, critiquing, evaluating content
   - `translation`: Language conversion and localization
   - `summarization`: Condensing and extracting key information

3. **Domain/Industry**
   - `technology`: Software, AI, engineering topics
   - `healthcare`: Medical, wellness, health-related content
   - `finance`: Financial planning, investment, economic topics
   - `education`: Academic, learning, training materials
   - `marketing`: Advertising, promotion, brand messaging

4. **Complexity Level**
   - `beginner`: Simple, easy-to-use prompts
   - `intermediate`: Moderate complexity, some experience needed
   - `advanced`: Complex prompts requiring expertise
   - `expert`: Highly specialized, professional-level prompts

5. **Output Format**
   - `structured`: JSON, YAML, tables, lists
   - `narrative`: Stories, articles, flowing text
   - `bullet-points`: Lists, summaries, key points
   - `code`: Programming code, scripts, markup
   - `dialogue`: Conversations, Q&A format

## Tag Schema

### Tag Definition Format
```json
{
  "tag_id": "unique-tag-identifier",
  "name": "display-name",
  "description": "Detailed description of when to use this tag",
  "category": "primary-category",
  "subcategory": "optional-subcategory",
  "synonyms": ["alternative-term-1", "alternative-term-2"],
  "related_tags": ["related-tag-1", "related-tag-2"],
  "usage_count": 0,
  "created_date": "2025-09-26",
  "status": "active",
  "examples": [
    "Example of when this tag applies",
    "Another usage example"
  ]
}
```

## Tagging Guidelines

### Best Practices

1. **Consistency**: Use established tags before creating new ones
2. **Specificity**: Choose the most specific applicable tags
3. **Completeness**: Include tags for all relevant dimensions (type, use case, domain, etc.)
4. **Moderation**: Avoid over-tagging; aim for 3-7 relevant tags per prompt
5. **Accuracy**: Ensure tags accurately represent the prompt's purpose and capabilities

### Tag Naming Conventions

- Use lowercase letters with hyphens for multi-word tags
- Keep tags concise but descriptive
- Avoid abbreviations unless widely understood
- Use singular form for consistency
- Example: `content-generation`, `technical-writing`, `beginner`

### Adding New Tags

Before creating a new tag:

1. Check existing tags and synonyms to avoid duplicates
2. Verify the tag doesn't overlap with existing categories
3. Follow the naming conventions
4. Add a clear description and examples
5. Update relevant category hierarchies
6. Submit for review in pull request

## Tag Validation

All tags must:

- Have a unique identifier
- Include a clear description
- Belong to a recognized category
- Follow naming conventions
- Not conflict with existing tags

## Usage Analytics

The tagging system tracks:

- **Tag Frequency**: How often each tag is used
- **Co-occurrence**: Which tags are commonly used together
- **Search Patterns**: Most searched tag combinations
- **Trending Tags**: Emerging popular tags
- **Orphaned Tags**: Tags no longer in use

## Maintenance

Regular maintenance includes:

- Reviewing and updating tag definitions
- Merging similar or duplicate tags
- Archiving unused tags
- Updating category hierarchies
- Monitoring tag usage patterns

---

*This tagging system enables efficient prompt discovery and maintains organizational consistency across the library.*
