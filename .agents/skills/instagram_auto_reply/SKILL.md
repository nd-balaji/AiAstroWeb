# Instagram Auto-Reply Skill

This skill allows Antigravity to monitor an Instagram post for specific keywords (e.g., "link", "lnk", etc.) and automatically reply to those comments while sending a Direct Message (DM) with specific links.

## Usage

To use this skill, provide the Instagram post URL and the message/links to be sent.

## Logic

1. **Fetch Comments**: Retrieve all comments for the specified post.
2. **Keyword Filtering**: Identify comments that containing keywords like "link", "lnk", or any close variations (e.g., "linnk", "linkk"), even if part of a larger sentence.
3. **Skip Already Replied**: Before acting, check if the comment *already* has a reply from **ANY** account. If it has any reply, skip it.
4. **Rate Limiting**: Perform at most **30 replies per hour** to prevent account flags.
5. **Reply**: For each eligible comment, post the reply "DM sent".
6. **DM**: Send the specific Saranga AI Astro links to the user.

## Configuration

- **Post URL**: `https://www.instagram.com/p/DWEdOv3gXE5/`
- **Keywords**: `link`, `lnk`, `linnk`, `linkk` (and other variations)
- **Reply Text**: `DM sent`
- **DM Text**:
```
Hi! ✨ 

Thanks for your interest in Saranga AI Astro – Your Cosmic Guide. Here are the links to get started:

📱 Android: https://play.google.com/store/apps/details?id=com.saranga.saranga_app

🍎 iOS: https://apps.apple.com/app/id6743130637

We'd love to hear your feedback as you explore your personalized predictions! 🙏

Happy stargazing! 🌙
```

## Tools Required

- `instagram.get_comments`
- `instagram.reply_comment`
- `instagram.send_direct_message`

> [!NOTE]
> The `@samarthakv29/antigravity-instagram-mcp` server is already configured in `/Users/Balaji/.gemini/antigravity/mcp_config.json`.
