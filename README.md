# Viikkotehtävä 2 Kotlin (week2)

### Model (domain-paketti)
- **Task.kt** – datamalli tehtävälle (id, title, description, priority, dueDate, done)
- **MockTasks** – valmis testausdata

### ViewModel (viewmodel-paketti)
- **TaskViewModel.kt** – hallitsee sovelluksen tilaa ja logiikkaa
- Käyttää **StateFlow**:ta reaktiiviseen tilan hallintaan
- Toiminnot: addTask(), toggleDone(), updateTask(), removeTask(), filterByDone(), sortByDueDate(), showAll()

### View (view-paketti)
- **HomeScreen.kt** – näyttää tehtävälistan
- **DetailDialog.kt** – tehtävän muokkaus ja poisto
- UI kuuntelee ViewModelin tilaa collectAsState():lla
- Päivitykset näkyvät automaattisesti listassa

## StateFlow
- Reaktiivinen tilan hallintaratkaisu
- Aina aktiivinen, emittoi viimeisimmän arvon heti
- UI päivittyy automaattisesti

## Demovideo

**Viikko3 video: https://youtu.be/4wLQ5KoWOzM**

(Viikko2 video: https://youtu.be/MCC26KozVKk)

(Viikko1 video: https://www.youtube.com/watch?v=QC4-GotNdLk)
