# Current Scoring Weights (from xai-org/x-algorithm)

**Source**: `home-mixer/params/param.rs`  
**Last synced from upstream**: 2026-09-24

> Important: These weights multiply the *predicted probability* of each action (or continuous values like dwell time). They do **not** multiply raw engagement counts. A high report weight does not mean “1 report cancels X likes.”

## Positive Weights

| Action | Parameter | Default Weight | Notes |
|--------|-----------|----------------|-------|
| Share via Copy Link | `ShareViaCopyLinkWeight` | **20.0** | Highest single positive weight |
| Reply | `ReplyWeight` | **5.0** | Base reply weight |
| Bidirectional Follow Reply Boost | `BidirectionalFollowReplyWeightBoost` | **15.0** | Added on top of ReplyWeight when mutual follow + original post → effective ~20 |
| Share via DM | `ShareViaDmWeight` | **5.0** | |
| Quote | `QuoteWeight` | **5.0** | |
| Follow Author | `FollowAuthorWeight` | **4.0** | |
| Share | `ShareWeight` | **2.0** | |
| Retweet | `RetweetWeight` | **1.0** | |
| Like / Favorite | `FavoriteWeight` | **0.5** | |
| Click | `ClickWeight` | **0.4** | |
| Open Link | `OpenLinkWeight` | **0.2** | |
| Video Open | `VideoOpenWeight` | **0.07** | |
| Photo Expand | `PhotoExpandWeight` | **0.05** | |
| Dwell (binary) | `DwellWeight` | **0.05** | |
| Quoted Click | `QuotedClickWeight` | **0.05** | |
| Continuous Dwell Time | `ContDwellTimeWeight` | **0.004** | |
| Post Unexplored | `PostUnexploredWeight` | **0.02** | |
| Profile Click | `ProfileClickWeight` | **0.0** | Currently off |
| VQV | `VqvWeight` | **0.0** | Currently off |
| Quoted VQV | `QuotedVqvWeight` | **0.0** | Currently off |
| Cont Click Dwell | `ContClickDwellTimeWeight` | **0.0** | Currently off |
| Bidirectional Follow Dwell Boost | `BidirectionalFollowDwellWeightBoost` | **0.0** | Currently off |

## Negative Weights

| Action | Parameter | Default Weight | Notes |
|--------|-----------|----------------|-------|
| Report | `ReportWeight` | **-234.0** | Strongest negative |
| Mute Author | `MuteAuthorWeight` | **-58.8** | |
| Not Interested | `NotInterestedWeight` | **-43.2** | |
| Block Author | `BlockAuthorWeight` | **-31.2** | |
| Not Dwelled | `NotDwelledWeight` | **-0.02** | Small penalty for being scrolled past |

## Key Insights for Creators
- **Highest leverage positive signals**: Copy-link shares, replies (especially with mutual follows), quotes, DM shares, and follows.
- Likes are relatively weak (0.5).
- Negative signals are extremely powerful because baseline probabilities are low; the model still needs them to influence ranking.
- Author diversity decay, out-of-network discount, and new-author boosts are applied *after* the weighted sum (see scoring code).

## How to Keep This Updated
1. Pull latest `home-mixer/params/param.rs` from upstream.
2. Re-extract the `param!(...Weight...)` lines.
3. Update the tables above and the “Last synced” date.
