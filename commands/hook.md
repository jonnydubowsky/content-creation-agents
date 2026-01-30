---
allowed-tools: [Read, Write, TodoWrite]
description: "High-retention hook creation with psychological triggers"
wave-enabled: false
category: "Retention"
auto-persona: ["hook-master"]
mcp-servers: []
---

# /cc:hook - Hook Creation

## Usage
```bash
/cc:hook [topic/context] [--style <style>] [--<flags>]
```

## Arguments
- `[topic/context]` - Subject or context
- `--platform ig|tt|yt|tw` - Target platform
- `--style question|statement|controversial|story|shock` - Hook type
- `--count [n]` - Number of hooks (default: 5)
- `--test` - Include A/B variants

## Auto-Activation
- **hook-master**: All hook generation

## Output Structure

```yaml
hooks:
  primary:
    - hook: "Exact hook text"
      pattern: "pattern_name"
      psychology: "trigger_used"
      platform_fit: "score/10"
      visual_cue: "visual_suggestion"
      duration: "2-4s"

  variants: # A/B testing
    hook_1_variants: [3_alternatives]
    hook_2_variants: [3_alternatives]

  ranking:
    viral_potential: [ranked]
    engagement_potential: [ranked]
    controversy_safe: [ranked]
```

## Hook Patterns Available

### Curiosity Gap (Power: 9/10)
- "What nobody tells you about..."
- "The secret that [authority] hides"
- "I discovered why [problem]"

### Controversial (Power: 9/10)
- "[Unpopular opinion] and I don't apologize"
- "Stop doing [popular advice]"
- "[Common belief] is a lie"

### Story Tease (Power: 9/10)
- "I lost everything when..."
- "This morning, I received a message that..."
- "The worst mistake of my life"

### Value Promise (Power: 7/10)
- "3 ways to [benefit] in [time]"
- "The framework I use for [result]"
- "[Number] mistakes that [consequence]"

### Pattern Interrupt (Power: 8/10)
- "STOP. Before scrolling..."
- "[Unexpected action] + now that I have your attention"

### Identity Call-Out (Power: 8/10)
- "If you're [identity], you need to know"
- "[Group] will understand"
- "POV: you're [situation]"

## Psychology Triggers

| Trigger | Mechanism | Power |
|---------|-----------|-------|
| Curiosity | Information gap | 9/10 |
| Fear | Loss aversion | 8/10 |
| Controversy | Cognitive dissonance | 9/10 |
| Identity | Group belonging | 8/10 |
| Scarcity | FOMO | 8/10 |
| Story | Narrative investment | 9/10 |
