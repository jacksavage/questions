# Random Questions

A simple GitHub Pages site that displays random questions from a text file. Click anywhere on the page to see a new question.

## Features

- Displays one random question at a time
- Click anywhere to get a new question
- Keyboard support (Space or Enter key)
- Mobile-friendly design
- Clean, minimal interface inspired by Claude's web UI

## Files

- `index.html` - The main webpage with embedded CSS and JavaScript
- `questions.txt` - Text file containing questions (one per line)

## Usage

Simply open the site and click anywhere to see a new random question. You can also press the Space bar or Enter key to get a new question.

## Deployment

### GitHub Pages (Recommended)

1. Push this repository to GitHub
2. Go to Settings → Pages
3. Select "Deploy from a branch" and choose your main branch
4. Your site will be available at `https://yourusername.github.io/your-repo-name`

### Netlify (With Preview Deployments)

1. Connect your GitHub repository to [Netlify](https://netlify.com)
2. Netlify will automatically deploy your site and create preview deployments for pull requests
3. Each PR will get a unique preview URL for testing

### Local Development

To test locally:

```bash
# Using Python (if installed)
python -m http.server 8000

# Using Node.js
npx serve -s . -l 3000

# Using PHP (if installed)
php -S localhost:8000
```

Then visit `http://localhost:8000` (or the port shown in your terminal).

## Preview Deployments

This repository includes GitHub Actions workflows that will:

1. **For Pull Requests**: Comment on PRs with instructions for local testing
2. **For Main Branch**: Deploy to GitHub Pages automatically

To enable automatic preview deployments:

1. **Netlify**: Connect your repo to Netlify for automatic PR previews
2. **Vercel**: Connect your repo to Vercel for automatic PR previews
3. **GitHub Pages**: Enable Pages in your repository settings

## Customization

To add your own questions, edit the `questions.txt` file and add one question per line.