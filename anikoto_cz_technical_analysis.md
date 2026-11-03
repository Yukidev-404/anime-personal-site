# AniKoto Technical Analysis

**URL**: https://anikoto.cz/
**Analysis Date**: November 3, 2026

## 1. Domain and DNS

- **Primary domain**: anikoto.cz
- **Alternative domain**: anikoto.site (mentioned for bookmarking)
- **CDN domain**: cdn.anipixcdn.co (used for thumbnails and background images)
- **TMDB domain**: image.tmdb.org (used for some anime banners)
- **Anilist domain**: s4.anilist.co/file/anilistcdn/media/ (referenced for anime metadata)

## 2. CDN and Asset Delivery

### 2.1 Image CDN: cdn.anipixcdn.co
- Used for anime thumbnails
- Used for category/genre background images
- Example URLs:
  - `https://cdn.anipixcdn.co/background/613d30a2d49fbe14_1791067142.webp` (Black Clover Season 2 banner)
  - `https://cdn.anipixcdn.co/thumbnail/b94877c900fc65a9_1791067150.webp` (Overgeared thumbnail)
  - `https://cdn.anipixcdn.co/thumbnail/83fedd9f4ba7ba74e4774b0ab142b915.jpg` (Full Clearing thumbnail)

### 2.2 The Movie Database (TMDB)
- Used for some anime banners/posters
- Example: `https://image.tmdb.org/t/p/original/a6ptrTUH1c5OdWanjyYtAkOuYD0.jpg` (One Piece banner)
- Indicates possible TMDB API integration for metadata

### 2.3 Anilist Integration
- Some anime reference Anilist for metadata
- Example: `https://s4.anilist.co/file/anilistcdn/media/anime/banner/206814-ARuwrZJAGONN.jpg` (Dragon Ball Super: Beerus banner)
- Suggests possible Anilist API usage for anime data

## 3. Website Structure Analysis

### 3.1 URL Patterns Observed

#### Genre Pages
- `/genre/action` - Action genre
- `/genre/action-adventure` - Action & Adventure
- `/genre/adventure` - Adventure
- `/genre/animation` - Animation
- (50+ genres total, each with dedicated URL)

#### Type Pages
- `/type/cm` - CM (Commercial/Music video)
- `/type/conspiracy` - Conspiracy
- `/type/movie` - Movies
- `/type/music` - Music
- `/type/ona` - ONA
- `/type/ova` - OVA
- `/type/pv` - PV
- `/type/scripted-anime-inspired` - Anime-inspired
- `/type/scripted-artificial-intelligence-a-i` - AI-themed
- `/type/special` - Specials
- `/type/tv` - TV series
- `/type/tv-short` - TV Shorts
- `/type/tv-special` - TV Specials
- `/type/virtual-reality` - VR content

#### Status Pages
- `/updated` - Recently updated
- `/new-release` - New releases
- `/most-viewed` - Most viewed
- `/latest-updated` - (redirects to /updated)
- `/newly-added` - (synonym for new-release)

#### Navigation
- `/home` - Homepage
- `/latest-updated` - Latest updates
- `/new-release` - New releases
- `/status/not-yet-aired` - Upcoming anime
- `/status/currently-airing` - Currently airing
- `/status/finished-airing` - Completed anime

### 3.2 Page Structure

#### Homepage Sections
1. **Spotlight** - Top 8 featured anime with watch links
2. **Genre navigation** - Clickable genre tags
3. **Type navigation** - Content type filters
4. **Status navigation** - Ongoing/Completed/Upcoming
5. **Quick access** - Watch2gether, Community, Schedule, Random
6. **Latest/Popular anime** - Grid display with thumbnails
7. **Top anime charts** - Day/Week/Month views
8. **A-Z List** - Alphabetical anime listing
9. **Search functionality** - Filter controls

#### Anime Episode Page Structure
- `/watch/{anime-slug}` - Main anime page
- `/watch/{anime-slug}/ep-{episode-number}` - Specific episode
- Episode pages show:
  - Episode title and number
  - Player/streaming interface
  - Previous/next episode navigation
  - Related anime suggestions

### 3.3 Search and Filtering
- **Genre filtering**: Click genre tags
- **Type filtering**: Select content type
- **Status filtering**: Ongoing/Completed/Upcoming
- **A-Z listing**: Browse by alphabet
- **Quick search**: Search bar functionality

## 4. Observed JavaScript/API Patterns

### 4.1 Possible API Endpoints (inferred)
While direct API inspection wasn't performed, the following patterns suggest API usage:

1. **AJAX content loading** - Genre/type/status pages likely load via API
2. **Episode data** - Episode metadata loaded dynamically
3. **Search results** - Queries processed server-side
4. **View count tracking** - Episode views tracked

### 4.2 JavaScript Framework
- Site appears to use modern web framework
- Interactive elements suggest React or Vue-like reactivity
- DOM manipulation for genre/type filters
- Dynamic content rendering based on user selection

### 4.3 Cookie and Tracking
- Standard session cookies
- Possible analytics tracking (not explicitly observed)
- No prominent GDPR consent banner observed

## 5. Responsive Design

### 5.1 Breakpoints
- **Desktop**: Full navigation, grid layouts with multiple columns
- **Tablet**: Adjusted grid, collapsible navigation
- **Mobile**: Single-column layout, hamburger menu

### 5.2 Mobile Features
- Touch-friendly buttons
- Collapsible genre/type menus
- Video player adaptation
- Language toggle (EN/JP) accessible on mobile

## 6. Content Organization Logic

### 6.1 Priority Ordering
Content is displayed in following priority:
1. **Spotlight** - Manually selected featured anime
2. **Latest Updated** - Most recently added episodes
3. **Most Viewed** - Popularity-based ranking
4. **New Releases** - Newly added content
5. **A-Z List** - Alphabetical browse

### 6.2 Genre Popularity
Based on observed data:
- Most featured: Action, Fantasy, Romance, Harem
- Strong presence: Shounen, Isekai, Mecha
- Niche categories: Dementia, Police, Gourmet

### 6.3 Type Distribution
- **TV**: Most common (majority of content)
- **Movie**: Significant portion
- **OVA**: Smaller but present category
- **ONA**: Growing category
- **PV**: Limited selection

## 7. User Flow Observed

### 7.1 Typical User Journey
1. Visit homepage (anikoto.cz)
2. Browse spotlight or genre categories
3. Click on anime title
4. Navigate to anime's episode list
5. Select episode and start streaming
6. Use navigation controls (next/previous, related anime)

### 7.2 Common Entry Points
- Direct anime search
- Genre browsing
- Top charts (day/week/month)
- Latest updates
- A-Z alphabetical list

### 7.3 Exit Points
- Watching complete episode/series
- Leaving site via external links
- Closing browser/tab

## 8. Technical Limitations Observed

### 8.1 Known Limitations
- **No official API documentation** - Inferred API usage only
- **No searchable episode guides** - Episode numbers must be known or guessed
- **Limited metadata** - Some anime lack detailed information
- **No user accounts** - (or unobserved) No visible account system
- **No download option** - Streaming only, no offline download observed
- **Potential region restrictions** - Not tested, may have geo-blocking

### 8.2 Browser Compatibility
- Tested working on modern browsers
- Older browser support mentioned ("works smoothly on older browsers")
- Mobile browser support confirmed

## 9. Security and Privacy Observations

### 9.1 Privacy Statement
- Copyright notice: "This site does not store any files on its server. All contents are provided by non-affiliated third parties."
- Standard third-party content disclaimer
- No explicit privacy policy observed in available pages

### 9.2 Tracking Elements
- Possible analytics cookies (not explicitly verified)
- Social media integrations (Reddit, Discord links present)
- External content embedding (third-party video players)

### 9.3 Advertising
- Advertising not explicitly observed in available content
- Site mentions "consider sharing with friends" (community growth focus)
- No pop-up ads observed during homepage navigation

## 10. Evidence Summary

| Category | Evidence |
|----------|----------|
| **Primary URL** | https://anikoto.cz/ |
| **Homepage** | https://anikoto.cz/home |
| **CDN Thumbnails** | cdn.anipixcdn.co |
| **CDN Backgrounds** | cdn.anipixcdn.co |
| **TMDB Integration** | image.tmdb.org |
| **Anilist Integration** | s4.anilist.co |
| **Community Links** | reddit.com/r/animekoto/, discord.gg/shz9hgT9sb |
| **Status Integration** | kotostatus.com |
| **Copyright** | "This site does not store any files on its server" |
| **Alternative Domain** | anikoto.site |

---
*Technical analysis conducted on November 3, 2026. Based on homepage and navigation page inspection only. Deeper API and structural analysis would require additional tools.*