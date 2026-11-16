# CareFirst Clinic | Online Appointment Booking 🩺

A modern online appointment booking system for a medical clinic. Patients select a consultation type, choose a date and an available time slot, and book their visit in under a minute. Clinic staff manage all appointments from a built-in admin dashboard.

**Live Booking Page:** https://carefirst-booking.vercel.app/
**Admin Dashboard:** https://carefirst-booking.vercel.app/admin.html

> Demo note: The admin page is currently public (no login) for demonstration. Secure staff login with Supabase authentication will be added in the next version.

---

## 📌 The Problem

Clinics often handle appointments by phone or front-desk registers. Patients wait on hold, schedules overlap, and no-shows go unnoticed. Staff spend hours on manual scheduling that could be automated.

## ✅ The Solution

CareFirst Clinic Booking provides a clean online appointment system:
- Patients see clear consultation types with price and duration
- Only free slots are shown, with weekends automatically closed
- Overlapping appointments are blocked, so the doctor's schedule stays accurate
- Staff can confirm, complete or cancel appointments in one click
- Service prices and durations can be updated from the admin panel

---

## ✨ Features

### Patient Booking Page
- Consultation type selection with price and duration
- Date picker (past dates are blocked)
- Live time slots (booked and past slots are disabled automatically)
- Overlap protection for longer consultations (like dental checkups)
- Weekend closure handled automatically
- Patient form with name, phone, email and notes
- Success popup with a reference code

### Admin Dashboard
- Summary cards: today's appointments, pending, confirmed and completed revenue
- Search by patient name, phone or reference code
- Filter by status (Pending, Confirmed, Completed, Cancelled)
- Change appointment status from a dropdown
- View full appointment details
- Delete appointments (with confirmation popup)
- Edit consultation prices and durations (saved and shown on the booking page)

---

## 🛠️ Tech Stack

- **HTML5** and **CSS3** (Tailwind CSS via CDN, custom styles)
- **Vanilla JavaScript** (no framework)
- **Lucide Icons**
- **Poppins** and **Inter** fonts (Google Fonts)
- **LocalStorage** for data persistence
- **Vercel** for hosting

---

## 📂 Project Structure

carefirst-booking/
├── index.html # Patient booking page
├── admin.html # Admin dashboard
├── css/
│ └── styles.css # Theme, booking UI and admin styles
├── js/
│ ├── app.js # Clinic config, slot engine and booking logic
│ └── admin.js # Admin dashboard logic
└── README.md


---

## ⚙️ How to Customize for Another Clinic

All clinic details are in one place: the `CONFIG` block at the top of `js/app.js`.

- `name`, `type`, `tagline`, `phone`, `address`
- `openTime`, `closeTime` and `slotMinutes` (appointment slot length)
- `closedDays` (0 = Sunday, 6 = Saturday)
- `accent`, `accentSoft`, `accentDark` (brand colors)
- `services` (consultation name, duration, price, description)

---

## 🚀 Getting Started

1. Open the live booking page link above.
2. Choose a consultation, pick a date and a time slot.
3. Enter your details and confirm.
4. Open the admin link to see the appointment appear instantly.

---

## 🔭 Future Improvements

- Supabase database and secure staff login
- SMS or WhatsApp reminders to patients
- Doctor selection and multiple clinic branches
- Online payment for consultation fees
- Patient history and follow-up reminders

---

## 👨‍💻 Author

**Daniyal Dynihmind**
Vibe Coder and Full-Stack Builder | Karachi, Pakistan

- GitHub: [@Daniyal-Dynihmind](https://github.com/Daniyal-Dynihmind)
- Open for freelance and client projects

If you like this project, give it a ⭐ on GitHub!
