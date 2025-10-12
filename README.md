# MoviesDatabase API

## API Overview
The **MoviesDatabase API** provides a comprehensive collection of movie, TV show, and actor information. It includes data such as YouTube trailer URLs, awards, biographies, cast and crew details, and more.  
The database holds information for over **9 million titles** (movies, series, and episodes) and **11 million actors and crew members**.  
Recent titles are updated weekly, while ratings and episodes are updated daily to ensure accuracy.

---

## Version
**Current Version:** 1.0

---

## Available Endpoints

### Titles
- **GET /titles** — Returns a list of titles based on optional filters or sorting parameters.  
- **GET /x/titles-by-ids** — Retrieves multiple titles by a list of IMDb IDs.  
- **GET /titles/{id}** — Returns detailed information about a specific title.  
- **GET /titles/{id}/ratings** — Retrieves rating and vote information for a title.  
- **GET /titles/series/{id}** — Returns episodes for a given series.  
- **GET /titles/seasons/{id}** — Returns the number of seasons for a given series.  
- **GET /titles/series/{id}/{season}** — Returns episodes for a specific season.  
- **GET /titles/episode/{id}** — Returns detailed information about a specific episode.  
- **GET /titles/x/upcoming** — Retrieves a list of upcoming titles.

### Search
- **GET /titles/search/keyword/{keyword}** — Searches titles using a keyword.  
- **GET /titles/search/title/{title}** — Searches for titles by name, with an option for exact matches.  
- **GET /titles/search/akas/{aka}** — Searches for titles by alternative names (AKAs).

### Actors
- **GET /actors** — Returns a list of actors based on filters or pagination.  
- **GET /actors/{id}** — Returns detailed information about a specific actor.

### Utils
- **GET /title/utils/titleType** — Returns available title types.  
- **GET /title/utils/genres** — Returns available genres.  
- **GET /title/utils/lists** — Returns available predefined title lists.

---

## Request and Response Format

### Example Request
```bash
GET /titles/tt0111161?info=base_info
