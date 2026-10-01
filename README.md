# Career Decisions Made on Vibes, Not Data

A decision-support analysis of the public Levels.fyi compensation survey. It helps job seekers and career switchers choose which skill to build, which company to target, and whether to stay or move.

## The Problem

Job seekers and career switchers make two high-stakes decisions: which skill to invest in and which company to target. Most rely on anecdotes, recruiter pitches, and outdated salary chatter.

Levels.fyi collects self-reported compensation at scale, but the raw survey data is messy:

- Inconsistent company names
- 1,809 unique "level" labels
- Free-text job tags
- No built-in answer to "so what should I actually do?"

This project turns that raw signal into a clear analysis.

## Questions This Project Answers

### Which skill?

Job tags like "ML / AI" and "Distributed Systems" pay roughly 15 to 20% more than "Web Development" or "DevOps". By how much exactly, and is the gap worth a re-skilling bet?

### Which company?

Total compensation varies widely by company and by the mix of base, stock, and bonus. The companies that pay the most are not always the ones that keep people the longest.

### Stay or hop?

52% of the dataset are "hoppers" (below-median tenure). Does changing jobs more often actually pay more, or is that a myth?

## Goal

Clean a noisy 62K-row public survey, build decision-relevant features, and train models that quantify these trade-offs instead of guessing at them.

## Approach

1. **Clean** the raw survey: standardize company names, group the 1,809 level labels, and normalize job tags.
2. **Engineer features** that matter for decisions, such as pay mix (base, stock, bonus) and tenure group (hopper vs. non-hopper).
3. **Model** the trade-offs for skill, company, and tenure.
4. **Report** findings in plain language so they are useful without a data science background.

## Data

- **Source:** Levels.fyi public compensation survey (self-reported)
- **Size:** about 62,000 rows
- **Known issues:** inconsistent company names, 1,809 unique level labels, free-text job tags

## Limitations

- Compensation is self-reported, so it may contain errors or selection bias.
- Results show association, not cause. A higher-paying skill tag does not guarantee a higher offer for any one person.




