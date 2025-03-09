# Octaview: Streamlining Hiring with Seamless Integration

Octaview is a B2B SaaS platform designed to revolutionize the hiring process. It provides a comprehensive suite of tools for managing job listings, candidate applications, interviews, and more, all seamlessly integrated into your existing company website.

## Key Features:

- **Effortless Integration**: Embed Octaview's job application UI directly into your website using our easy-to-install npm package.
- **Centralized Job Management**: Create and manage job listings through a user-friendly dashboard.
- **Automated Candidate Management**: Streamline the application process and automate candidate communication with email notifications at each stage.
- **Efficient Interview Scheduling**: Schedule interviews with ease and manage candidate availability.
- **Integrated Video Interviewing**: Conduct remote interviews with built-in video conferencing and collaborative code editing.
- **Collaborative Code Editor**: Utilize Monaco Editor with Yjs for real-time collaborative code editing during technical interviews.
- **API Key Validation**: Each request is validated using an API key for added security.
- **Secure Payment Processing**: Integrate with Stripe for secure token-based payments. Each applicant submission costs one token.
- **Robust Infrastructure**: Built on a scalable and reliable architecture utilizing AWS, GCP, Vercel, and other leading technologies.

## Architecture Overview:

![Alt text](https://octaview-data.s3.ap-south-1.amazonaws.com/images/diagram-export-3-6-2025-9_53_04-PM.png)


## Technical Details:

- **Frontend**: React, JS/TS Library
- **Backend**: Express.js (Node.js)
- **Database**: PostgreSQL (Submission Storage), MongoDB Atlas (CRUD Operations)
- **Job Queue & Cache**: Redis
- **Video Interviewing**: Yjs Signaling Server (AWS EC2), Judge (GCP Compute Engine)
- **Cloud Providers**: AWS (EC2, S3), GCP, Vercel
- **Payment Gateway**: Stripe
- **Authentication**: API Key-based, Stripe for token-based payments

## Related Repositories

Here are some key repositories related to the Octaview project:

1. **[Octaview-library](https://github.com/mammenmathewz/octaview-client-pkg)**  
   This repository contains the core npm package that enables companies to integrate Octaview's job application UI seamlessly into their websites.

2. **[Octaview-backend](https://github.com/mammenmathewz/OCTAVIEW)**  
   The backend server that powers Octaview. Built with Express.js, it handles candidate applications, job management, API key validation, and integrates with other services like Stripe for secure payment processing.

3. **[Octview-cloud-compiler](https://github.com/mammenmathewz/octview-cloud-compiler)**  
   This repository contains the video interviewing platform for Octaview, which includes real-time collaborative code editing with Monaco Editor and Yjs for technical interviews.

4. **[octaview-frontend-ui](https://github.com/mammenmathewz/OCTAVIEW-CLIENT)**  
   The React-based frontend that powers the user interface for job applications, candidate management, and interview scheduling.

5. **[Crdt-signaler-yjs](https://github.com/mammenmathewz/crdt-signaler-yjs)**  
   A repository for setting up and integrating the CRDT signaling server using Yjs, which powers real-time collaborative editing and communication during video interviews.

## Installation and Integration:

### 1. Install the npm package:

```bash
npm install octaview-library
```
### 2. Integrate the library into your website:
```
import Octaview from 'octaview-library';

// Initialize Octaview with your API key
const octaview = new Octaview('YOUR_API_KEY');

// Render the job application UI
octaview.render('#octaview-container');
```
### 3. Configure API Key Authentication:
Obtain your API key from the Octaview dashboard.
Use the API key for authentication when integrating the library.

### 4. Secure Payment Integration (Stripe):
Each applicant submission costs one token. Integrate Stripe’s payment gateway for secure payment handling.

## Getting Started:
-Sign up for an Octaview account:
 Visit [coctview.tech] to create your account.

-Create and manage job listings:
 Use the Octaview dashboard to add and manage your job openings.

-Integrate the library into your website:
 Follow the installation and integration steps outlined above.

 Start hiring!

## License:
  [Your License]

## Support:
For any questions or support, please contact us at [mammen999@gmail.com].

