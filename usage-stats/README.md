# Usage Statistics

This directory contains analytics and insights about prompt performance, usage patterns, and effectiveness metrics.

## Purpose

The `usage-stats` directory serves as a centralized location for:

- **Performance Analytics**: Track how well prompts perform across different use cases
- **Usage Metrics**: Monitor which prompts are most frequently accessed and used
- **A/B Testing Results**: Compare different versions of prompts to optimize effectiveness
- **Success Rate Tracking**: Measure prompt success rates and user satisfaction
- **Trend Analysis**: Identify patterns in prompt usage over time

## File Structure

```
usage-stats/
├── README.md                    # This file
├── monthly-reports/            # Monthly usage and performance reports
├── prompt-analytics/           # Individual prompt performance data
├── user-feedback/              # Aggregated user feedback and ratings
├── ab-testing/                 # A/B testing results and comparisons
└── trending/                   # Trending prompts and emerging patterns
```

## Data Format

All analytics files should follow consistent JSON/CSV formats:

### Prompt Performance Schema
```json
{
  "prompt_id": "unique-prompt-identifier",
  "period": "2025-09",
  "metrics": {
    "total_uses": 150,
    "success_rate": 0.87,
    "avg_rating": 4.3,
    "completion_rate": 0.92
  },
  "user_feedback": {
    "positive_count": 42,
    "negative_count": 5,
    "common_issues": ["needs more context", "too verbose"]
  },
  "performance_trends": {
    "usage_growth": 0.15,
    "rating_trend": "stable",
    "success_trend": "improving"
  }
}
```

## Usage Guidelines

1. **Regular Updates**: Update statistics monthly or when significant changes occur
2. **Privacy Protection**: Ensure all data is anonymized and doesn't contain personal information
3. **Consistent Formatting**: Follow established schemas for easy data aggregation
4. **Version Control**: Track changes to maintain historical data integrity

## Contributing Analytics

When contributing usage statistics:

1. Ensure data is properly anonymized
2. Follow the established JSON schemas
3. Include relevant metadata (collection date, methodology, etc.)
4. Document any assumptions or limitations in the data
5. Reference the source prompts using their unique IDs

## Privacy and Ethics

- All usage data must be collected with proper consent
- Personal identifying information should never be stored
- Data should be aggregated to protect individual privacy
- Follow applicable data protection regulations (GDPR, CCPA, etc.)

---

*This directory helps improve prompt quality through data-driven insights while maintaining user privacy and ethical standards.*
