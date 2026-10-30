# Wild Rose Studio

Wild Rose Studio is a .NET 10 Blazor WebAssembly site. Run it locally with:

```powershell
dotnet run
```

Open the site root for the public homepage or `?editor=1` for the studio editor. The editor supports live text/photo previews, saving a draft, and publishing the saved content.

## Current storage and launch limitations

Drafts, published content, and uploaded photos are stored in the current browser's `localStorage`. They are not shared with visitors or other devices, and the editor is not password-protected. Uploaded photos are limited to 500 KB. This implementation is suitable for a local prototype, not a production CMS; connect authenticated server-side storage before using the editor to update a public site.

The contact email starts as `hello@example.com`; replace it in the editor before sharing the website.

## Deployment

GitHub Pages deploys automatically when changes are pushed to `main`. The workflow builds the Blazor WebAssembly app with the .NET 10 SDK and publishes the contents of `wwwroot`. The repository must use **GitHub Actions** as its Pages build and deployment source.

The workflow configures the app for the repository URL (`https://baseballr.github.io/WildRoseStudios/`). The existing `netlify.toml` can still be used to deploy to Netlify.
