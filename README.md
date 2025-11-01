# MedNexus-AI-Driven-Patient-Health-Management-Platform

🩺 Project Concept
MedNexus is a full-stack healthcare platform designed to connect patients, doctors, and diagnostic labs in a secure, data-driven, and AI-assisted ecosystem. It solves common healthcare issues like scattered patient records, inefficient report management, and the lack of personalized, AI-driven insights.

✨ What We've Achieved (So Far)
This project has successfully established a secure, multi-role, and data-rich environment.

Full-Stack Secure Authentication: A complete multi-role login system (Patient, Doctor) has been built using NestJS, Passport.js, and JWT. The React frontend is secured with protected routes that redirect unauthorized users.

Role-Based Access Control (RBAC): The backend is secured with custom RolesGuards, ensuring that only users with the 'Doctor' role can create prescriptions or view other patients' data.

Complete Clinical Workflow:

Doctors can log in, search for patients by ID, view their complete medical history, write new digital prescriptions, and add new health records (both as JSON vitals and as file uploads).

Patients can log in, view their read-only dashboard, see the list of prescriptions written for them, and review all health records (including files) added by their doctor.

Cloud File Storage: Integrated Cloudinary for handling file uploads. Doctors can upload PDF lab reports or images, which are stored securely in the cloud. The patient dashboard correctly displays a "Download" link for these files.

Integrated AI Microservice: A separate Python (FastAPI) microservice successfully connects to the Google Gemini API. The NestJS backend can securely call this service, sending it a patient's health data and receiving a generative AI-driven health summary in return.

Analytics & Visualization: Implemented Recharts on the Doctor Dashboard to create interactive line charts that visualize a patient's vital signs (e.g., cholesterol, blood pressure) over time from their health records.

🚀 Future Roadmap (In Progress)
This project is actively under development. The next steps will focus on implementing the remaining core features to complete the platform's vision:

Real-Time Chat & Consultations (F5): Implement a secure, real-time patient-doctor chat module using Socket.io.

E-Prescription PDF Generation (F3): Add a service to the NestJS backend to generate a downloadable PDF (with a QR code) for prescriptions, rather than just displaying the JSON data.

At-Rest Encryption (F6): Implement AES-256 encryption for the HealthRecord.data JSON field to ensure all sensitive health information is encrypted within the database.

Expanded Roles (F1): Build the dedicated dashboards and API endpoints for the Lab/Clinic Admin (for uploading test results) and the System Admin (for user verification).


💻 Tech StackLayerTechnologyFrontendReact, TypeScript, Vite, Mantine UI, Recharts, AxiosBackend (API)NestJS (Node.js), TypeScript, Passport.js, JWT, PrismaBackend (AI)Python, FastAPIDatabasePostgreSQL (managed with Docker)File StorageCloudinary APIAI APIGoogle Gemini


🚦 Project Status
This project is actively under development. The core architecture and primary features are functional. Future development will focus on implementing the remaining roadmap features before the platform is deployed.
