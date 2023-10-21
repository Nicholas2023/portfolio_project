# CreatorsHub: Empowering Content Creators and Enthusiasts :smile:

CreatorsHub is a dynamic platform designed for content creators and enthusiasts alike. This repository contains the MVP specifications, architecture, APIs, data model, user stories, and mockups for the CreatorsHub project.

## Table of Contents
- [Architecture](#architecture)
- [APIs and Methods](#apis-and-methods)
- [Data Model](#data-model)
- [User Stories](#user-stories)
- [Mockups](#mockups)

## Architecture

![System Architecture](link-to-architecture-diagram)
The system architecture comprises front-end and back-end components. CreatorsHub utilizes React.js for the user interface, communicating seamlessly with the Django backend through REST APIs. PostgreSQL is the chosen database, hosted on AWS for scalability and reliability.

## APIs and Methods

### API Routes for Web Client

#### `/api/podcasts`
- `GET`: Retrieve a list of podcasts.
- `POST`: Upload a new podcast.

#### `/api/interviews`
- `GET`: Retrieve a list of interviews.
- `POST`: Upload a new interview.

#### `/api/comics`
- `GET`: Retrieve a list of comics.
- `POST`: Upload a new comic.

### Endpoints/Functions for Other Clients

#### Podcast Class
```javascript
// Constructor(year, month, title, audioUrl)
// Creates a new podcast object.
getDuration()
// Returns the duration of the podcast.
```

#### Interview Class
```javascript
// Constructor(year, month, interviewer, interviewee)
// Creates a new interview object.
getTranscript()
// Returns the transcript of the interview.
```

#### Comic Class
```javascript
// Constructor(title, author, imageUrl)
// Creates a new comic object.
getGenre()
// Returns the genre of the comic.
```

### 3rd Party APIs
- **AWS S3 API**
  - `PUT /podcasts/{podcastId}`: Uploads a podcast file to AWS S3.
  - `PUT /interviews/{interviewId}`: Uploads an interview audio file to AWS S3.
  - `PUT /comics/{comicId}`: Uploads a comic image file to AWS S3.

## Data Model

![Data Model](link-to-data-model-diagram)
The database includes tables for podcasts, interviews, and comics. Each table contains fields such as ID, Title, Author, Audio URL, and Image URL, ensuring efficient data storage and retrieval.

## User Stories

### User Story 1: Content Upload
As a content creator, I want to upload my podcasts, interviews, and comics, providing a seamless experience and reaching a broader audience.

### User Story 2: User Discovery
As a user, I want to discover diverse content, filtering podcasts, interviews, and comics based on genres and authors, enhancing my entertainment choices.

### User Story 3: Content Management
As a content creator, I want a dedicated dashboard to manage my uploaded content, including editing, deleting, and tracking engagement metrics.

## Mockups

![Mockup 1](link-to-mockup-1)
![Mockup 2](link-to-mockup-2)

---

CreatorsHub is an exciting project aiming to bring creators and consumers together. Stay tuned for updates as we work on building this platform! For any questions or collaborations, feel free to contact us.

*Happy Creating! 🚀*
