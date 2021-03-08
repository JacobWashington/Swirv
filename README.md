# Swirv

![Swirv Logo](./assets/images/logo.png)

## Description

Swirv is a distributive story-telling platform, where every reader can branch from an author's storyline to spin their own tale.

## Demand

Traditionally, an author's greatest responsibility has been to give their readers the full story, to leave no rock unturned. This responsibility, however, curtails the author's ability to give some of their greatest ideas life. Too many brilliant, unfinished stories have never reached readers because an author must commit themselves to the stories they can end. This diservice, to both authors and readers, is out of line with the natural ways in which stories form and develop — dynamically and collaboritively. By allowing every reader the opportunity to contribute to a story, or branch from a storyline at any point to forge a new journey, Swirv realigns the ancient art of storytelling with nature.

### Vocab

**Anomaly**
: created when a user branches from an existing episode or storyline, creating an *alternate storyline* to the existing

**The Great Attractor**
: a database table designed to allow users to submit stories anonymously, without disturbing another user's ability to branch from that story

## User Stories

**MVP**

- As a user, I want to create a profile
- As a user, I want to create a new storyline
- As a user, I want to create a new episode in a storyline
- As a user, I want to edit my episodes and storyline
- As a user, I want to branch from another user's episodes and storylines
- As a user, I want to offer episodes and storylines to _The Great Attractor_

**Added Features**

- As a user, I want to create collections of stories to my profile
- As a user, I want to add authors, episodes, and storylines to my favorites
- As a user, I want to add episodes and storylines to "Read Later"
- As a user, I want to comment on episodes
- As a user, I want to rate episodes, storylines, and authors
- As a user, I want to _offer_ storylines to _The Great Attractor_
- As a user, I want to set the genre of my storylines

## Database Architecture

![Swirv DB Architecture V5](./assets/images/databaseDiagramV5.png)

**Database Edge-Cases**
- User1 deletes episode or storyline branched by User2. In this case, User1 will not actually delete the storyline/episode from the database, but will waive ownership of the content. *The Great Attractor* then becomes the owner, granting User1 anonymity without jeopardizing the branch created by User2.

## Future Development

- [ ] Tips: Users can tip an author of episodes they especially enjoyed, or to show appreciation for their favorite storylines
- [ ] 3rd Party Branching: With a URL, users can branch from 3rd party sources. Our code will then target the URL and scrape relevant content, displaying it with a reference to the source  
