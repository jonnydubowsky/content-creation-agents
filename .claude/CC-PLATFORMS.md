# CC-PLATFORMS.md - Platform Specifications & Best Practices

Technical specifications and strategies by platform.

## Platform Quick Reference

| Platform | Best For | Sweet Spot | Key Metric |
|----------|----------|------------|------------|
| 📱 TikTok | Discovery, trends | 30-60s | Watch time % |
| 📸 Instagram | Community, brand | 15-30s Reels | Saves, shares |
| ▶️ YouTube | Authority, SEO | 8-15min long | CTR + retention |
| 🎮 Twitch | Real-time, loyalty | 2-4h streams | Concurrent viewers |

---

## 📱 TikTok

### Algorithm Signals (Priority Order)
```yaml
primary_signals:
  1_watch_time:
    weight: "HIGHEST"
    target: ">70% completion"
    boost: "Loop rate (rewatches)"

  2_shares:
    weight: "Very High"
    target: ">1% share rate"
    why: "Extends reach outside FYP"

  3_comments:
    weight: "High"
    target: "Meaningful comments"
    boost: "Reply to comments quickly"

  4_likes:
    weight: "Medium"
    note: "Less important than watch time"

  5_follows:
    weight: "Medium-High"
    signal: "Authority/quality indicator"

secondary_signals:
  - video_info: "Captions, sounds, hashtags"
  - device_account: "Language, location, device"
  - negative: "Not interested, hide, report"
```

### Technical Specs
```yaml
video:
  aspect_ratio: "9:16 (vertical)"
  resolution: "1080x1920"
  file_size: "Max 287MB (mobile), 500MB (web)"
  duration: "15s - 10min"
  format: "MP4, MOV"

optimal_duration:
  viral_potential: "15-30s"
  educational: "45-90s"
  story: "60-180s"
  series: "60s per episode"

audio:
  trending_sounds: "Use within 48h of trend"
  original_audio: "Good for authority"
  music: "Via TikTok library only"
```

### Content Strategy
```yaml
content_types_that_work:
  highest_reach:
    - "Trending sounds + original spin"
    - "Controversial takes"
    - "Story time"
    - "Quick tutorials"

  highest_conversion:
    - "Educational series"
    - "Behind the scenes"
    - "Day in the life"

posting_strategy:
  frequency: "1-4x per day (quality > quantity)"
  timing:
    best_general: "6-10AM, 7-11PM"
    test_windows: "Try different times for 2 weeks"
  consistency: "Daily for algorithm favor"

hashtags:
  count: "3-5 hashtags"
  mix:
    - "1-2 broad (1M+ views)"
    - "2-3 niche specific"
    - "0-1 trending"
  placement: "In caption or first comment"
```

### TikTok-Specific Patterns
```yaml
hooks_that_work:
  - "POV: [relatable situation]"
  - "Things [group] need to hear"
  - "Tell me you're [X] without telling me"
  - "Storytime: [tease]"
  - "This is your sign to [action]"

formats_that_work:
  - "Green screen + talking head"
  - "Trending sound mashup"
  - "Stitch viral content"
  - "Transition reveals"
  - "Text overlay + voiceover"

engagement_hacks:
  - "Reply to comments with video"
  - "Create duets with followers"
  - "Pin best comments"
  - "Go live regularly"
```

---

## 📸 Instagram

### Algorithm Signals (By Format)
```yaml
reels_algorithm:
  1_watch_time: "Completion rate critical"
  2_engagement_speed: "First 30min crucial"
  3_saves_shares: "Highest weight signals"
  4_source_of_view: "Explore > Following"

feed_algorithm:
  1_relationship: "Past interactions"
  2_interest: "Content type history"
  3_timeliness: "Recency matters"
  4_engagement: "Quality of interactions"

stories_algorithm:
  1_relationship: "Close friends prioritized"
  2_interaction_history: "Past engagement"
  3_completion_rate: "Watch whole story"
```

### Technical Specs
```yaml
reels:
  aspect_ratio: "9:16"
  resolution: "1080x1920"
  duration: "15-90s (30s optimal)"
  cover: "Custom thumbnail important"

feed_post:
  square: "1080x1080"
  portrait: "1080x1350 (best)"
  landscape: "1080x608"

carousel:
  max_slides: 10
  aspect: "1:1 or 4:5"
  resolution: "1080x1080 or 1080x1350"

stories:
  aspect: "9:16"
  resolution: "1080x1920"
  duration: "15s per story"

captions:
  max_length: "2,200 characters"
  optimal: "125-150 words"
  hashtags: "5-10 (in caption or comment)"
```

### Content Strategy
```yaml
content_mix:
  reels: "60% (reach)"
  carousels: "25% (saves)"
  single_posts: "10% (brand)"
  stories: "Daily (engagement)"

reels_strategy:
  frequency: "1-2 per day"
  timing: "11AM-1PM, 7-9PM"
  hooks: "0-1.5s critical"
  cover_image: "Custom, curiosity-driven"

carousel_strategy:
  slide_1: "Hook (question or bold statement)"
  slides_2-8: "Value delivery"
  slide_9: "Summary or CTA"
  slide_10: "Follow CTA + save reminder"

stories_strategy:
  frequency: "5-10 per day"
  mix:
    - "Behind the scenes"
    - "Polls and questions"
    - "Reposts of feed content"
    - "Personal moments"
  engagement: "Use interactive stickers"

hashtags:
  count: "5-10 (quality over quantity)"
  strategy:
    - "2-3 large (500K+ posts)"
    - "3-4 medium (50K-500K)"
    - "2-3 small (10K-50K)"
```

### Instagram-Specific Patterns
```yaml
carousel_hooks:
  - "Swipe to learn [valuable thing]"
  - "[Number] things [audience] need to know"
  - "Save this for later"
  - "This will change how you [action]"

reels_hooks:
  - "What I wish I knew about [topic]"
  - "The [audience] guide to [topic]"
  - "How to [desirable outcome] in [time]"
  - "Stop doing this if you want [result]"

save_triggers:
  - "Lists and resources"
  - "Step-by-step guides"
  - "Templates and frameworks"
  - "Checklists"
  - "Infographics"

collab_features:
  - "Collab posts (share followers)"
  - "Add yours stickers"
  - "Remix reels"
```

---

## ▶️ YouTube

### Algorithm Signals
```yaml
shorts_algorithm:
  1_swipe_rate: "Don't swipe away = good"
  2_watch_time: "Completion rate"
  3_engagement: "Likes, comments, shares"
  4_subscribe_click: "Authority signal"

long_form_algorithm:
  1_ctr: "Click-through rate (target: >5%)"
  2_watch_time: "Total minutes watched"
  3_session_time: "Keeps viewers on YouTube"
  4_engagement: "Likes, comments, subscribers"
  5_audience_retention: "Graph shape matters"

discovery_factors:
  - "Search (SEO title, description, tags)"
  - "Suggested (related videos)"
  - "Browse (home page)"
  - "Notifications (subscribers)"
```

### Technical Specs
```yaml
shorts:
  aspect_ratio: "9:16"
  resolution: "1080x1920"
  duration: "15-60s"
  title: "SEO important (100 chars)"
  hashtags: "#Shorts required"

long_form:
  aspect_ratio: "16:9"
  resolution: "1920x1080 min, 4K preferred"
  duration:
    educational: "8-15 minutes"
    entertainment: "15-25 minutes"
    deep_dive: "25-45 minutes"

thumbnails:
  resolution: "1280x720 (16:9)"
  file_size: "<2MB"
  text: "3-5 words max"
  faces: "Close-ups work best"
  contrast: "Bright colors, high contrast"

titles:
  length: "60 characters optimal"
  structure: "[Hook/Benefit] | [Topic] | [Year optional]"
  keywords: "Front-load important words"
```

### Content Strategy
```yaml
shorts_strategy:
  frequency: "1-3 per day"
  timing: "Consistent schedule"
  purpose:
    - "Drive to long-form"
    - "Test hooks"
    - "Reach new audience"
  structure:
    - "Hook: 0-2s"
    - "Value: 2-55s"
    - "CTA: Final 5s"

long_form_strategy:
  frequency: "1-2 per week minimum"
  consistency: "Same day/time each week"
  structure:
    intro: "0-30s (hook + promise)"
    body: "Main content with chapters"
    outro: "CTA + next video tease"

retention_optimization:
  first_30s: "CRITICAL - hook hard"
  mid_video: "Pattern interrupts every 30-60s"
  dips: "Address with more engaging content"
  end_screen: "20s for cards"

seo_elements:
  title: "Keyword + curiosity"
  description: "Keyword in first 2 lines"
  tags: "5-15 relevant tags"
  chapters: "Timestamp chapters"
  cards: "Link to related content"
  end_screens: "Subscribe + video"
```

### YouTube-Specific Patterns
```yaml
thumbnail_formulas:
  - "Face + emotion + 3 words"
  - "Before/after comparison"
  - "Intrigue + question"
  - "Number + benefit"
  - "Controversy/surprise"

title_formulas:
  - "How I [Achievement] in [Time]"
  - "I Tried [Thing] for [Time]"
  - "[Number] [Thing] That Will [Benefit]"
  - "The Truth About [Topic]"
  - "Why You Should Stop [Common Action]"

retention_techniques:
  - "Timestamp chapters"
  - "Pattern interrupts (B-roll, graphics)"
  - "Open loops ('I'll explain later...')"
  - "Engagement prompts"
  - "Mid-roll CTAs (soft)"
```

---

## 🎮 Twitch

### Algorithm & Discovery
```yaml
discovery_factors:
  1_live_status: "Live = more visible"
  2_viewer_count: "Higher = higher in category"
  3_category: "Choose wisely"
  4_tags: "Relevant tags"
  5_title: "Descriptive + engaging"

growth_signals:
  - "Consistent schedule"
  - "Chat activity"
  - "Raid participation"
  - "Clip creation"
  - "VOD views"
```

### Technical Specs
```yaml
stream_settings:
  resolution: "1920x1080 (1080p)"
  framerate: "60fps for games, 30fps for talking"
  bitrate: "4500-6000 kbps"
  audio: "Clear voice priority"

clips:
  duration: "5-60s"
  purpose: "Viral moments, highlights"
  export: "For TikTok/YouTube Shorts"

vods:
  highlight: "Edit VODs into highlights"
  export: "To YouTube for SEO"
```

### Content Strategy
```yaml
stream_structure:
  intro: "5-10min chat + setup"
  main_content: "Primary activity (game, etc.)"
  interactions: "Regular chat engagement"
  breaks: "Every 2h for you + viewers"
  outro: "Raid + next stream reminder"

schedule:
  minimum: "3x per week"
  optimal: "5x per week"
  duration: "2-4 hours per stream"
  consistency: "Same times each week"

engagement:
  chat_interaction: "Read + respond regularly"
  alerts: "Celebrate follows/subs"
  commands: "Useful chat commands"
  loyalty: "Points system, rewards"

growth_tactics:
  raids: "Give and receive"
  collabs: "Other streamers"
  clips: "Encourage viewers to clip"
  community: "Discord server"
  cross_platform: "TikTok/YouTube clips"
```

### Twitch-Specific Patterns
```yaml
title_formulas:
  - "[Game] | [Mood/Activity] | [!commands]"
  - "[Achievement Goal] | [Game]"
  - "First time playing [Game]!"
  - "[Event/Challenge] | [Game]"

clip_worthy_moments:
  - "Achievements/wins"
  - "Fails (entertaining)"
  - "Reactions"
  - "Funny chat interactions"
  - "Skill showcases"

community_building:
  - "Discord server"
  - "Emote/badge system"
  - "Channel points rewards"
  - "Subscriber perks"
  - "Regular events"
```

---

## Cross-Platform Strategy

### Repurposing Matrix
```yaml
original_to_platform:
  tiktok_video:
    to_reels: "Direct repost (remove watermark)"
    to_shorts: "Direct repost"
    to_feed: "Screenshot carousel"
    to_stories: "Add interactive elements"

  youtube_long:
    to_shorts: "Best 60s moments"
    to_tiktok: "Clips with hooks"
    to_reels: "Key takeaways"
    to_carousel: "Summary/quotes"

  twitch_stream:
    to_youtube: "Full VOD or highlights"
    to_shorts: "Best clips"
    to_tiktok: "Funny/skill moments"
    to_reels: "Clips with context"

  carousel:
    to_video: "Animated carousel"
    to_tiktok: "Talking head version"
    to_stories: "Slide by slide"
```

### Platform Priority by Goal
```yaml
goals:
  reach_awareness:
    priority: ["TikTok", "YouTube Shorts", "Reels"]
    why: "Algorithmic distribution"

  authority_trust:
    priority: ["YouTube Long", "LinkedIn", "Instagram Feed"]
    why: "Depth + SEO"

  community_loyalty:
    priority: ["Twitch", "Instagram Stories", "Discord"]
    why: "Real-time interaction"

  conversion_sales:
    priority: ["Instagram", "YouTube", "TikTok"]
    why: "Link capabilities + intent"
```

### Timing Coordination
```yaml
posting_schedule:
  tiktok: "6-10AM, 7-11PM daily"
  instagram: "11AM-1PM, 7-9PM daily"
  youtube_shorts: "2-4PM daily"
  youtube_long: "Consistent weekly slot"
  twitch: "Set weekly schedule"

batch_production:
  film_day: "Multiple contents at once"
  edit_day: "All platforms from same shoot"
  schedule: "Schedule week in advance"
  repurpose: "Same content, adapted"
```

---

## Platform Trends 2024-2025

```yaml
emerging_trends:
  tiktok:
    - "Longer content (3-10min)"
    - "Educational deep-dives"
    - "TikTok Shop integration"
    - "Series format"

  instagram:
    - "Broadcast Channels"
    - "Notes feature"
    - "Collaborative content"
    - "Threads integration"

  youtube:
    - "Shorts monetization"
    - "Community posts growth"
    - "Podcast integration"
    - "AI recommendations"

  twitch:
    - "Vertical streaming"
    - "Mobile streaming growth"
    - "Non-gaming content"
    - "Clips for discovery"

adapt_strategy:
  - "Test new features early"
  - "Monitor platform updates"
  - "Follow creator programs"
  - "Adapt to algorithm changes"
```
