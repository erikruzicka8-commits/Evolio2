# evolio2

Samostatný zdroj doplňků a doplněk pro uživatelem zadaný účet Evolia Efry (tenant efry). Původní doplněk evolio se nemění.

## Obsah

- .claude-plugin/marketplace.json: místní zdroj s jediným doplňkem evolio2.
- plugins/evolio2/.claude-plugin/plugin.json: identita nového doplňku.
- plugins/evolio2/.mcp.json: 11 samostatně pojmenovaných HTTP serverů Evolia.
- plugins/evolio2/skills/evolio2-search/SKILL.md: pokyny pro práci výhradně formou vyhledávání a čtení.

## Důležitá omezení

Instalace konfigurace není důkazem funkčního přihlášení. Bez přihlášení testovaná adresa serveru spisů odpověděla HTTP 401; to neověřuje existenci ani dostupnost firemního účtu Efry pro konkrétního uživatele.

Některé servery Evolia nabízejí také zapisovací nástroje. Přiložená dovednost zakazuje jejich použití asistentem, ale tato konfigurace technicky neodebírá oprávnění k zápisu. Před tvrzením, že je přístup technicky jen pro čtení, je nutné ověřit skutečná oprávnění na straně Evolia nebo doložené vynucení omezení.

Konfigurace neobsahuje hesla, tokeny ani přístupové klíče. Bezpečné přihlášení nelze nahrazovat vložením tajných údajů do těchto souborů nebo chatu.

## Podklady

- https://docs.codexis.ai/codexis-ai-2-0/manual/doplnky/
- https://evolio.cz/mcp/
- Nápověda dostupného příkazu cdxctl marketplace add potvrzuje podporu zdroje typu local. Webový formulář na snímku přijímá Git URL, nikoli místní cestu ani přímou MCP URL.
