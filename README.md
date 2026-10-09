# JPGFORMAT.

Independent creative platform with Zane Karate at `/karate-zane/`.

## Deploy

Import these files to a new GitHub repository and connect it to a **new** Vercel project named `jpgformat`. Select `Other` as the framework and the repository root as the root directory. The `vercel.json` rewrites delegate `/karate-zane/` and its resources to the existing Zane Karate Vercel site.

**Important:** The existing Zane project currently uses Vercel authentication protection on its Vercel deployment addresses. The `/karate-zane/` rewrite may require Vercel authentication and cannot be considered publicly live until Zane has a public custom domain or its protection settings are revised, and cross-project rewrite behavior is tested. Do not disable protection without explicitly reviewing the impact.

Zane's site uses root-relative asset paths for page rendering and routing must be checked carefully. CSS `url('assets/...')` is relative to the stylesheet path proxied under `/karate-zane/`; anchor links remain on the subpage.

Once the new project is publicly accessible, attach the purchased JPGFORMAT domain to the new project in Vercel Project → Settings → Domains.
