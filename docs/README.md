# Auto-Sign Frontend

This is the GitHub Pages frontend for the Auto-Sign application.

## Setup Instructions

The frontend is automatically published to GitHub Pages, but it requires a deployed backend to function.

### Step 1: Deploy the Backend

Deploy the Flask application (app.py) to a hosting service:

- **Render**: https://render.com (recommended for Python apps)
- **Heroku**: https://heroku.com
- **Railway**: https://railway.app
- **PythonAnywhere**: https://pythonanywhere.com

### Step 2: Configure the Backend URL

After deploying the backend, update the `BACKEND_URL` constant in `index.html`:

```javascript
const BACKEND_URL = "https://your-deployed-app-url.com";
```

### Step 3: Commit and Push

Commit the change and push to the `main` branch. GitHub Pages will automatically redeploy the site.

## Testing

Once configured, visit your GitHub Pages site at:
`https://jamarwhitfield.github.io/auto-sign/`

You should be able to:
1. Select a .docx file
2. Click "Process document"
3. Download the processed file with the signature added
