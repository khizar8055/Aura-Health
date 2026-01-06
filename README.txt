## Aura Health – Smart Healthcare Management App

Aura Health is a full-stack, multi-role healthcare management application built with Flutter and Firebase. It connects patients, doctors, and administrators in a single platform, covering the complete journey from onboarding and appointment booking to consultation, feedback, and system administration.

The app uses a unified dark–gold design system, smooth animations, and role-based navigation to deliver a modern, production-ready experience.

---

## Core Features

### Multi‑Role Access

- **Patient** – search doctors, book appointments, chat, run AI symptom checks, rate doctors, and manage their profile.
- **Doctor** – manage appointments, view patient history, chat with patients, track ratings, and configure clinic details.
- **Admin** – oversee patients, doctors, appointments, ratings, and complaints via a dedicated admin dashboard and tools.

---

## Patient Module

- **Role-based onboarding** with patient login/signup and persistent sessions.
- **Dashboard** with greeting, quick stats, and shortcuts (find doctor, appointments, chat, AI, settings).
- **Doctor search** by name, specialization, city, with cards showing photo, rating, specialization, and fee.
- **Appointment booking** flow with doctor selection, date/time slot, visit reason, and fee preview.
- **Appointment management** for Pending, Approved, Today, Tomorrow, and History states.
- **AI Symptom Checker** with offline and online modes (Flutter UI + Flask API integration).
- **Secure chat** with doctors (text + image messages) using Firebase Realtime Database.
- **Notifications** for appointment updates, reminders, and chat events.
- **Ratings & feedback** after completed consultations (1–5 stars + optional comment).
- **Complaints** against doctors, routed to the admin module.
- **Profile & settings** for personal info, contact details, preferences, and logout.

---

## Doctor Module

- **Doctor authentication** with PMDC-based signup and login.
- **Dashboard** with daily schedule, upcoming appointments, and key stats.
- **Appointment management** to approve/reject requests and mark visits as completed.
- **Patient list** built automatically from appointment history, with quick search.
- **Patient history** screens for reviewing previous consultations.
- **Chat with patients** in real time (mirrored chat experience from the doctor side).
- **Ratings overview** with average rating and detailed feedback entries.
- **Clinic management** (clinic name, address, timings, fee, and image).
- **Doctor settings** for profile edits, preferences, and logout.

---

## Admin Module

- **Admin login** and secure access to the admin tools.
- **Admin dashboard** showing:
	- Total patients and doctors.
	- Pending doctor approvals.
	- Today’s and total appointments.
	- Recent system activities.
- **Doctor management** with pending/active tabs, full details, approval, and deletion.
- **Patient management** with searchable list and expandable detail cards.
- **Global appointment view** across all doctors and patients with filters (All, Today, Tomorrow, Pending, Approved, Completed).
- **Rating and feedback oversight** to review and moderate all doctor ratings.
- **Complaints management** with views for all, from patients, and from doctors.
- **Admin drawer** with avatar, quick navigation, and logout.

---

## AI Symptom Checker

- **Offline mode** with a lightweight embedded model for basic symptom analysis.
- **Online mode** using a Python + Flask API and a trained ML model for richer predictions.
- User-friendly symptom selection and results, always encouraging follow-up with a qualified doctor.

---

## Real‑Time Chat & Notifications

- One‑to‑one chat between patients and doctors with:
	- Real-time message updates.
	- Image attachments for reports and prescriptions.
- Role-specific notification centers:
	- Patients – appointment status, reminders, chat events.
	- Doctors – new requests, schedule reminders, new ratings.
	- Admin – new signups, complaints, and system activity.

---

## UI & Design

- **Dark + gold theme** implemented via a shared design system.
- **Consistent branding** with a shared app image (imageapp.png) across welcome, auth, and admin views.
- Smooth entrance and transition animations (via `animate_do` and Flutter animations).
- Responsive layouts that scale well on different device sizes.

---

## Tech Stack

- **Frontend**: Flutter (Dart), Material Design, custom theming.
- **Backend**: Firebase Realtime Database.
- **AI Service**: Python, Flask, scikit‑learn (online symptom checker).
- **Storage & Media**: Image upload service (e.g., ImgBB) for profile, clinic, and chat images.
- **Local Storage**: SharedPreferences for session and preference persistence.
- **Packages** (core):
	- `firebase_core`, `firebase_database`, `firebase_auth`
	- `google_fonts`, `animate_do`, `flutter_animate`
	- `image_picker`, `http`, `shared_preferences`


---

**Developed by Khizar Lodhi using Flutter**
*Last updated: January 6, 2026*
