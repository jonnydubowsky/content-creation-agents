# Content Creator Framework

Multi-platform content creation framework for Claude Code.

**Token-optimized** | **Retention-focused** | **Marketing-driven**

## Installation

```bash
# Via Claude Code CLI
claude plugins install content-creation-agents
```

## Supported Platforms

| Platform | Optimization |
|----------|--------------|
| 📱 TikTok | Discovery, trends, watch time |
| 📸 Instagram | Community, saves, Reels |
| ▶️ YouTube | SEO, retention, Shorts |
| 🎮 Twitch | Live, engagement, clips |

## Commands

### Ideation & Strategy

```bash
/cc:ideate [niche] --platform tt --viral
```
Generate 10+ ideas with hooks, unique angles and virality scores.

```bash
/cc:calendar --month --platforms ig,tt
```
30-day editorial planning with themes and batch production.

```bash
/cc:trend [niche] --actionable
```
Trend monitoring with scored opportunities and timing.

### Production

```bash
/cc:script [topic] --platform tt --duration 60s
```
Complete script with timestamps, hooks, pattern interrupts and CTA.

```bash
/cc:hook [topic] --style controversial --test
```
5 high-retention hooks with A/B variants.

```bash
/cc:series [theme] --episodes 5 --format weekly
```
Complete series with narrative arc and cliffhangers.

### Optimization

```bash
/cc:repurpose [content] --from yt --to ig,tt
```
Cross-platform adaptation with optimized specs.

```bash
/cc:analyze [@account] --recommendations
```
Performance analysis with actionable insights.

## Specialized Agents

Agents activate automatically based on context:

| Agent | Expertise | Auto-Activation |
|-------|-----------|-----------------|
| `cc-strategist` | Global vision, positioning | Planning, strategy |
| `cc-hook-master` | Retention, attention psychology | Scripts, hooks |
| `cc-scriptwriter` | Storytelling, pacing | Content writing |
| `cc-trend-hunter` | Monitoring, timing | Trends, opportunities |
| `cc-platform-expert` | Algos, formats, specs | Adaptation |

## Retention Patterns

### Hook Patterns (0-3s)
- **Curiosity Gap** → "What nobody tells you about..."
- **Controversial** → "Stop doing [popular advice]"
- **Story Tease** → "I lost everything when..."
- **Value Promise** → "3 ways to [benefit] in 30s"
- **Identity Call-Out** → "If you're [group], you need to know..."

### Retention Patterns (Mid)
- **Open Loops** → Maintain curiosity
- **Pattern Interrupts** → Reset attention (every 7-15s)
- **Value Stacking** → Value escalation
- **Story Peaks** → Emotional peaks

### Engagement Patterns
- **Comment Bait** → "Team A or Team B?"
- **Save Trigger** → High-utility content
- **Share Trigger** → Identity/emotional content

## Global Flags

```bash
--platform [ig|tt|yt|tw|all]  # Target platform
--niche [niche]               # Niche context
--tone [edu|fun|pro|raw]      # Tone
--duration [15s|30s|60s|3m]   # Duration format
--viral                       # Optimize virality
--evergreen                   # Timeless content
--batch                       # Batch production output
```

## Usage Examples

### Quick Creation Workflow
```bash
/cc:trend fitness                    # Identify trends
/cc:ideate fitness --trend --viral   # Trend-based ideas
/cc:script [idea] --platform tt      # Adapted script
```

### Strategic Workflow
```bash
/cc:calendar --month --niche tech    # Monthly plan
/cc:series "Side Hustle" --episodes 5  # Create series
/cc:repurpose [content] --to all     # Multiply reach
```

### Analysis Workflow
```bash
/cc:analyze @competitor --competitor  # Competitor analysis
/cc:trend [niche] --deep             # Deep monitoring
```

## File Structure

```
📁 content-creation-agents/
├── CONTENT-CREATOR.md    # Entry point + quick reference
├── CC-COMMANDS.md        # 8 commandes détaillées
├── CC-AGENTS.md          # 5 agents + coordination
├── CC-PATTERNS.md        # 30+ patterns rétention
└── CC-PLATFORMS.md       # Specs TikTok/IG/YT/Twitch
```

## Token Optimization

The framework uses an optimized architecture:
- Standardized symbols (📱 TikTok, 📸 IG, ▶️ YT, 🎮 Twitch)
- Compact YAML for structured outputs
- Auto-activated agents (no manual config)
- Pre-integrated patterns (no re-explanation)

## Roadmap

- [ ] Visual templates (Canva/Figma specs)
- [ ] Analytics integration
- [ ] A/B testing automation
- [ ] Scheduling integration
- [ ] Multi-language support

## License

MIT

---

Made with Claude Code
