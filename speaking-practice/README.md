# Speaking Practice - Organized Structure

This directory contains French speaking practice materials organized by major topics.

## Structure

```
speaking-practice/
├── alimentation/              # Food & nutrition topics
├── collocations/              # Language learning (collocations)
├── environnement/             # Environment & climate
├── reseaux_sociaux/           # Social networks
├── sante/                     # Health topics
├── technologie/               # Technology topics
├── travail/                   # Work-related topics
├── uniforme/                  # Uniform (school & work)
└── vie_privee/                # Privacy topics
```

## Organization

Each topic folder contains:
- **manifest.json**: Lists all subtopics with metadata and paths
- **Subtopic folders**: Each contains:
  - `content.json`: Questions, prompts, and model answers
  - `audio/`: MP3 files for each item

## Manifest.json Format

```json
{
  "topic": "topic_id",
  "title": "Topic Title",
  "level": "B2",
  "subtopics": [
    {
      "id": "subtopic_id",
      "title": "Subtopic Title",
      "contentPath": "speaking-practice/topic_id/subtopic_folder/content.json"
    }
  ]
}
```

All paths in manifest.json files start with `speaking-practice/` for absolute referencing.

## Content.json Format

```json
{
  "id": "topic_subtopic",
  "lang": "fr",
  "level": "B2",
  "topic": "Topic Name",
  "items": [
    {
      "id": "intro",
      "t": "Introduction text",
      "audio": "speaking-practice/topic_id/subtopic_folder/audio/intro.mp3"
    },
    {
      "id": "q1",
      "t": "Question 1 text",
      "s": 45,
      "audio": "speaking-practice/topic_id/subtopic_folder/audio/q1_warmup.mp3"
    },
    {
      "id": "q2",
      "t": "Question 2 text",
      "s": 60,
      "audio": "speaking-practice/topic_id/subtopic_folder/audio/q2_opinion.mp3"
    },
    {
      "id": "q3",
      "t": "Question 3 text",
      "s": 90,
      "audio": "speaking-practice/topic_id/subtopic_folder/audio/q3_nuance.mp3"
    },
    {
      "id": "model",
      "t": "Model answer text",
      "audio": "speaking-practice/topic_id/subtopic_folder/audio/model_answer.mp3"
    }
  ]
}
```

All audio paths in content.json files start with `speaking-practice/` for absolute referencing.

### Item Properties:
- `id`: Unique identifier (intro, q1, q2, q3, model)
- `t`: Text content (question or statement)
- `s`: Speaking time in seconds (only for questions)
- `audio`: Absolute path to audio file starting with `speaking-practice/`

## Topics Overview

### 🍽️ Alimentation (Food)
- Modes de consommation (Consumption patterns)
- Alimentation et santé (Diet & health)

### 📚 Collocations (Language Learning)
- Apprentissage (Learning)
- Méthodes (Methods)

### 🌍 Environnement (Environment)
- Changement climatique (Climate change)
- Gestes quotidiens (Daily actions)
- Responsabilité collective (Collective responsibility)
- Voiture hybride (Hybrid cars)

### 📱 Réseaux Sociaux (Social Networks)
- Vue générale (General overview)
- Réseaux sociaux et jeunes (Social media & youth)
- Réseaux sociaux et vie privée (Social media & privacy)

### 🏥 Santé (Health)
- Allopathie vs Homéopathie
- Chirurgie esthétique (Cosmetic surgery)
- Ondes électromagnétiques et risques sanitaires (EMF health risks)

### 💻 Technologie (Technology)
- Cloud computing
- Publicité sur le web (Web advertising)

### 💼 Travail (Work)
- Discrimination à l'embauche (Hiring discrimination)
- Équilibre vie pro/vie perso - Difficultés, Santé, Solutions
- Télétravail - Vue générale, Décision, Rôles

### 👔 Uniforme (Uniform)
- Uniforme à l'école (School uniform)
- Uniforme au travail (Work uniform)

### 🔒 Vie Privée (Privacy)
- Droit à l'image (Right to image)
