# BatchMate Group Exam — starter

This starter includes Firebase email/password admin sign-in (restricted to the supplied admin UID), anonymous student sign-in, admin-managed name/roll roster, MCQ authoring, publishing, student answer submission, and admin attempt review.

## Important
Secure immediate grading must run on a trusted server (for example, a callable Cloud Function). This starter keeps answer keys admin-only and therefore stores submissions for teacher review instead of exposing answers or calculating scores in the browser. Firebase Cloud Functions deployment generally requires the Blaze billing plan. No-PIN name/roll access is not strong identity verification.

## Deploy
- Replace Firestore Rules with `firestore.rules` and Publish.
- Enable Email/Password and Anonymous providers in Firebase Authentication.
- Deploy `public/index.html` to Firebase Hosting. Standard Firebase CLI deployment is `firebase deploy --only hosting`; this needs a CLI-capable environment.
- Sign in using the Email/Password account whose UID is configured in the source.
