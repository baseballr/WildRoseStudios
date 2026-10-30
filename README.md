# Wild Rose Studio

Wild Rose Studio is a .NET 10 Blazor WebAssembly site. Run it locally with:

```powershell
dotnet run
```

Site content lives in the code: `Pages/Home.razor` (homepage, contact email) and `Pages/Portfolio.razor` (collections).

## Deployment

GitHub Pages deploys automatically when changes are pushed to `main`. The workflow builds the Blazor WebAssembly app with the .NET 10 SDK and publishes the contents of `wwwroot`. The repository must use **GitHub Actions** as its Pages build and deployment source.

The workflow configures the app for the repository URL (`https://baseballr.github.io/WildRoseStudios/`). The existing `netlify.toml` can still be used to deploy to Netlify.
