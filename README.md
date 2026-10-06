# NSCET Alumni Network – Launch page
Static site: play promo video, then "Launch App" -> https://nscetalumni.pages.dev/

## Publish on GitHub Pages
git init -b main && git add -A && git commit -m "NSCET Alumni launch page"
gh repo create nscet-alumni-launch --public --source=. --push
gh api -X POST repos/:owner/nscet-alumni-launch/pages -f "source[branch]=main" -f "source[path]=/"
# Live at https://<your-username>.github.io/nscet-alumni-launch/
