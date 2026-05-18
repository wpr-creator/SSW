# SSW — World History

A two-semester World History course covering Western political thought through globalization and the information revolution.

## Course Schedule

| Day | Title | Standards | EQ | Status |
|-----|-------|-----------|-----|--------|
| Semester 1 Day 1 | Roots of Western Political Thought | 10.1 | How did ancient Greek, Roman, and Judeo-Christian ideas create the foundation for modern democracy? | Coming Soon |
| Semester 1 Day 2 | Democratic Revolutions | 10.2 | What ideas pushed people to overthrow their governments, and did those ideas survive? | Coming Soon |
| Semester 1 Day 3 | The Industrial Revolution | 10.3 | How did industrialization change where people lived, how they worked, and what they believed? | Coming Soon |
| Semester 1 Day 4 | New Imperialism | 10.4 | Why did powerful nations take over weaker ones, and what did colonized people do about it? | Coming Soon |
| Semester 1 Day 5 | Causes of World War I | 10.5 pt 1 | How did rivalry, nationalism, and one assassination pull the entire world into war? | Coming Soon |
| Semester 1 Day 6 | Fighting WWI | 10.5 pt 2 | What was it actually like to fight in WWI, and why did so many people die? | Coming Soon |
| Semester 1 Day 7 | The Human Cost of WWI | 10.5 pt 3 | Who paid the highest price in WWI, and how did the war change culture and society? | Coming Soon |
| Semester 1 Day 8 | Nationalism and the Long Road to WWI | 10.2 pt 2 and 10.5 bridge | How did nationalism spread across Europe, get repressed, and finally explode into the 20th century? | Coming Soon |
| Semester 1 Day 9 | Final Exam | — | — | Coming Soon |
| Semester 2 Day 1 | The Failed Peace After WWI | 10.6 | How did the peace after WWI plant the seeds for the next war? | Coming Soon |
| Semester 2 Day 2 | Rise of Totalitarian Governments | 10.7 | How do democracies collapse, and what do dictators do once they have power? | Coming Soon |
| Semester 2 Day 3 | Causes and Start of World War II | 10.8 pt 1 | How did the world let Hitler build an empire before anyone stopped him? | Coming Soon |
| Semester 2 Day 4 | Fighting WWII and the Holocaust | 10.8 pt 2 | How did WWII become the deadliest conflict in human history? | Coming Soon |
| Semester 2 Day 5 | Post-War World and Cold War Origins | 10.9 pt 1 | How did the end of WWII immediately create a new global conflict between former allies? | Coming Soon |
| Semester 2 Day 6 | Cold War Conflicts Around the World | 10.9 pt 2 | How did the U.S.-Soviet rivalry drag other countries into real wars? | Coming Soon |
| Semester 2 Day 7 | Decolonization and Nation-Building | 10.10 | What challenges did newly independent nations face, and did independence deliver what people hoped for? | Coming Soon |
| Semester 2 Day 8 | Globalization and the Information Revolution | 10.11 | How have technology and global economic integration changed what it means to live in the modern world? | Coming Soon |
| Semester 2 Day 9 | Final Exam | — | — | Coming Soon |

## File Naming Convention

HTML lesson files follow this pattern (zero-padded lesson numbers):

- Regular lessons: `SSW_S1L01.html` through `SSW_S1L08.html`
- Final exam: `SSW_S1L09_Final.html`
- Semester 2 uses `S2` instead of `S1` (e.g. `SSW_S2L01.html`, `SSW_S2L09_Final.html`)

## Image Folder and Naming Convention

Lesson images live under `images/` organized by semester and lesson:

```
images/
  S1/
    L01/
    L02/
    ...
    L08/
  S2/
    L01/
    ...
    L08/
```

Name image files: **`{Semester}{Lesson}_DescriptiveName.jpg`**

Example: `images/S1/L01/S1L01_Constitution.jpg`

See [images/README.md](images/README.md) for full details.

## Flipping a Lesson Live

On `index.html`, each day is a card with class `day-card`. The lesson link is already in place. To publish a lesson:

1. Open `index.html`
2. Find the card for that day
3. Add the class **`live`** — change `class="day-card"` to `class="day-card live"`

That is the only change required. Locked cards (without `live`) appear grayed out with a lock icon and are not clickable. Live cards use full styling, a hover effect, and link to the lesson HTML file.
