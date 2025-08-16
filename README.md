
# Citizen-Alert — Netlify (Git + Functions)

## Déploiement
1. Crée un repo Git et pousse tous ces fichiers à la racine.
2. Netlify → Add new site → Import from Git.
3. Build settings :
   - Publish directory: `web`
   - Functions directory: `netlify/functions`
4. Déploie → teste `/api/health` et `/api/incidents`.

## Endpoints
- GET /api/health
- GET /api/incidents
- POST /api/submit-incident
- POST /api/moderate

## Persistance
Ces fonctions sont des mocks. Branche une DB (Supabase/Neon) dans `submit-incident.js` / `moderate.js`.
