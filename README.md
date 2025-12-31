-
# 🚀 Com publicar a GitHub Pages

1. **Pujar el codi a GitHub**: Crea un repositori nou i puja tots els fitxers.
2. **Configurar Google Cloud**:
   - Ves a la teva consola de Google Cloud.
   - Afegeix `https://el-teu-usuari.github.io` a la llista de **Authorized JavaScript Origins**.
3. **Activar GitHub Pages**:
   - Al teu repositori de GitHub, ves a **Settings > Pages**.
   - A **Build and deployment > Source**, selecciona **GitHub Actions**.
4. **Deploy**:
   - Quan facis un `push` a la branca `main`, el fitxer `.github/workflows/deploy.yml` s'encarregarà de tot.
   - Podràs veure el progrés a la pestanya **Actions**.

### Nota sobre l'API Key de Gemini
Com que GitHub Pages és un entorn estàtic, qualsevol clau d'API que estigui al codi (o s'injecti en el build) serà visible per l'usuari final. Per a una aplicació d'estudi professional, et recomanem:
- Assegurar-te que la teva API Key de Google Cloud té **restriccions d'aplicació** (només acceptar peticions des del teu domini de GitHub Pages).
