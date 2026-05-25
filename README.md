# FlowDrop — Free Automation Workflow Ideas

A beautiful, searchable library of 45+ battle-tested automation workflows across 13 platforms and use cases.

## 🚀 Deploy to Netlify

### Option 1: Drag & Drop (Easiest)
1. Go to [app.netlify.com](https://app.netlify.com)
2. Drag the `index.html` file directly into the Netlify drop zone
3. Your site is live in seconds

### Option 2: Git Integration (Recommended)
1. Push this repo to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial FlowDrop deployment"
   git remote add origin https://github.com/YOUR-USERNAME/flowdrop.git
   git push -u origin main
   ```

2. Connect to Netlify:
   - Go to [app.netlify.com](https://app.netlify.com)
   - Click "New site from Git"
   - Select your GitHub repo
   - Build command: (leave empty)
   - Publish directory: `.`
   - Deploy!

3. Set up auto-deploys: Any push to main triggers a new deployment

### Option 3: Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy
```

## 📋 What's Inside

- **45+ Workflows** across CRM, Marketing, Support, HR, Ops, AI, and more
- **13 Platform Categories**: HubSpot, Salesforce, Zendesk, n8n, Make, Zapier, OpenAI, etc.
- **Real Step-by-Step Flows**: Each workflow includes detailed steps, not just theory
- **Difficulty Levels**: Beginner, Intermediate, Advanced
- **Live Search & Filtering**: Find exactly what you need in seconds
- **Zero Dependencies**: Pure HTML + vanilla JS — nothing to install

## 🎨 Customization

### Change Branding
Edit the color variables in the `<style>` section:
```css
:root {
  --accent: #00E5FF; /* Change to your brand color */
  --text: #E8EAF0;
  --bg: #0C0E14;
  /* ... more colors ... */
}
```

### Add More Workflows
Add to the `FLOWS` array in the `<script>` section:
```javascript
{
  id: 46,
  cat: 'crm',
  platform: 'HubSpot',
  icon: '🎯',
  diff: 'easy',
  steps: 4,
  saves: 123,
  title: 'Your Workflow Title',
  desc: 'Your workflow description',
  tags: ['Tag 1', 'Tag 2'],
  flow: [
    { t: 'Step 1 Title', d: 'Step 1 description' },
    { t: 'Step 2 Title', d: 'Step 2 description' },
    // ... more steps
  ]
}
```

### Add New Categories
Add a new category chip in the HTML and add a color to the CSS.

## 🤖 Future Enhancements

- [ ] AI-powered workflow generator (describe your goal → get a custom workflow)
- [ ] Community submissions portal
- [ ] Email newsletter with new workflows
- [ ] GitHub integration for workflow versioning
- [ ] API to programmatically fetch workflows

## 📊 Analytics

Add Google Analytics, Plausible, or your favorite analytics provider before `</body>`.

---

**Built with ☕ for automation professionals.**
