# Fashion App

**Course:** MTM4681 — Milestone Submission
**Team:** 11

Fashion App is a mobile application that helps users find clothing. The user takes a photo or uploads one from the gallery, and the app finds the most similar products in a catalog of online retailers, matching color and texture. Users can open a product in the retailer's store and save products to their favorites.

## Team

| Name | Student ID | GitHub |
|---|---|---|
| Halil Akın | 22052039 | [halillakin](https://github.com/halillakin) |
| Melissa Eylül Şen | 22052055 | [melissaeylul03-jpg](https://github.com/melissaeylul03-jpg) |

## Milestone Deliverables

| # | Deliverable | Format | Location |
|---|---|---|---|
| 1 | Design justification (1–2 pages) | PDF | [docs/design-justification.pdf](docs/design-justification.pdf) |
| 2 | User flow diagram | PDF | [docs/user-flow-diagram.pdf](docs/user-flow-diagram.pdf) |
| 3 | Wireframes | Figma | [Wireframes page](https://www.figma.com/design/PiBzrWRanQTBw5xutgAkdA/FashionApp?node-id=0-1) |
| 4 | Mockups | Figma | [Mockups page](https://www.figma.com/design/PiBzrWRanQTBw5xutgAkdA/FashionApp?node-id=1-2379) |
| 5 | Prototype | Figma | [Prototype page](https://www.figma.com/design/PiBzrWRanQTBw5xutgAkdA/FashionApp?node-id=1-2380) (open in Present mode; flow starts at *01 Login*) |
| 6 | Architecture and protocols | PDF | [docs/architecture-and-protocols.pdf](docs/architecture-and-protocols.pdf) |

**Figma access:** the Figma file is shared by link, and anyone with the link can view it, so the instructor does not need a separate invitation.

## Technology

- **Mobile app:** Flutter (Dart)
- **Accounts and data:** Firebase Authentication (email and password) and Cloud Firestore (user profiles and favorites)
- **Image similarity service:** Python with FastAPI, using the FashionCLIP model to turn clothing images into feature vectors and compare them
- **Communication:** the app sends the photo to the service over HTTP (multipart upload) and receives the matching products as JSON

## Repository Structure

```
.
├── README.md
├── docs/
│   ├── design-justification.pdf
│   ├── user-flow-diagram.pdf
│   └── architecture-and-protocols.pdf
└── screenshots/        (screens of the working prototype, supporting material)
```

## Notes

- A working Flutter prototype of the main flow already exists (login, photo selection, similar product results, product details, favorites). Screenshots are provided as supporting material. The milestone itself consists of the design and architecture documents listed above.
- The prototype currently uses a small demo catalog of products from one online retailer.
