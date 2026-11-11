# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] POST /sessions returns a session_id
- [ ] At least 3 relevant citations per side are stored
- [ ] Response latency <2 seconds
- [ ] Each side has ≥5 distinct argument nodes
- [ ] Every argument includes a non‑empty citations list
- [ ] Arguments are stored and retrievable via GET /sessions/{id}/arguments
- [ ] Chat UI shows alternating turns
- [ ] Critique is generated within 2 seconds
- [ ] User can request a summary of strengths/weaknesses
- [ ] Set up repo, Docker, CI
- [ ] Define PostgreSQL schema + pgvector index
- [ ] Implement FastAPI endpoints for session CRUD
- [ ] Integrate LangChain with public web search (SerpAPI mock)
- [ ] Build ResearchAgent to store embeddings
- [ ] Create ArgumentAgent using CrewAI to produce structured arguments
- [ ] Design LangGraph state machine for turn‑based flow
- [ ] Implement CriticAgent (feedback generation)
- [ ] Connect Redis cache for low latency
- [ ] Develop React chat UI
- [ ] Write unit & integration tests (pytest, httpx)
- [ ] Configure GitHub Actions for Docker image push
- [ ] Deploy to Railway/Render with PostgreSQL add‑on
- [ ] Unit tests for each FastAPI route (pytest)
- [ ] Mocked LangChain retrieval tests to verify citation count
- [ ] LangGraph workflow unit tests with simulated states
- [ ] Integration test: full session lifecycle from creation to critique
- [ ] Load test 20 concurrent sessions using locust to verify latency
- [ ] Dockerfile builds multi‑stage image (Python runtime)
- [ ] docker‑compose.yml defines api, postgres, redis services
- [ ] GitHub Actions workflow builds image, runs tests, pushes to Docker Hub
- [ ] Deploy on Railway (free tier) linking managed Postgres and Redis

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
