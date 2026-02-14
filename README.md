# Jan-Drishti – AI-Native Civic Intelligence System

**Challenge Track:** [Student Track] AI for Communities, Access & Public Impact

**Jan-Drishti** is an AI-first governance intelligence layer that transforms unstructured citizen inputs (voice, photo, text) into verified, structured, and actionable signals for government departments. Instead of another complaint portal, it uses AI to verify issues, auto-route to correct departments, detect infrastructure risk patterns, and provide real-time citizen feedback.

## Problem Solved
- Fragmented governance: Citizens navigate multiple portals (CPGRAMS, UMANG, state systems) without knowing which department owns their issue
- Digital exclusion: Rural, elderly, low-literacy citizens excluded by language barriers and smartphone requirements
- Reactive systems: No early warning for infrastructure risks, spam filtering, or pattern detection

## Key Features
- Voice-first in 22 Indian languages (Bhashini + Amazon Transcribe)
- Computer vision verification (Amazon Rekognition) for infrastructure damage
- AI auto-routing to correct departments (Amazon Bedrock Claude 3.5)
- Geo-clustering for pattern detection and early warnings
- SMS/IVRS access for non-smartphone users
- SLA auto-escalation with Step Functions
- Seamless integration with CPGRAMS/UMANG via APIs

## Team Name
**Torvia Systems**

| Member     | Role                  |
|------------|-----------------------|
| Sharaj MM  | Team Lead             |
| Dharnesh   | AI/ML Specialist      |
| Athitya    | Full Stack Developer  |
| Barath M   | DevOps & Integration  |

## Documentation
- [Requirements Specification](requirements.md)
- [System Design & Architecture](design.md)

## Tech Stack
AWS Serverless + AI/ML:
├── Amazon Bedrock (Claude 3.5) – AI Triage & Routing
├── Amazon Rekognition – CV Verification
├── Bhashini + Transcribe – 22 Languages
├── Lambda + Step Functions – Workflows
├── Aurora/DynamoDB/S3 – Data Layer
└── QuickSight – Real-time Analytics

## Architecture Overview
![Simplified Architecture](AWS_Diagram.png)

## Expected Impact
- 80%+ auto-routing accuracy (vs 40% manual)
- 70% reduction in routing time
- 40%+ voice/assisted-mode usage from excluded communities
- Early infrastructure risk detection preventing failures

## Pilot Scope
- 1 city/district
- 2 flows: Civic infrastructure + Non-emergency police complaints
- Live integration with local PWD/Police systems

## Security & Compliance
- AES-256 encryption at rest
- TLS 1.3 in transit
- SHA-256 evidence hashing
- Full audit trail with CloudTrail
- IAM least privilege + RBAC

---

Built for AWS AI for Bharat Hackathon – Student Track  
Transforming governance through AI augmentation, not replacement.
