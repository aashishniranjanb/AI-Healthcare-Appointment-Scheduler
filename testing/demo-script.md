# Demo Conversation Script

**Scenario:** Patient calls to book an appointment.

---

**AI:** Hello! Thank you for calling Wellspring Family Clinic. This is Dr. Sarah, your AI medical assistant. How may I assist you today?

**Patient:** I’d like to book an appointment with Dr. Smith on August 10th at 2 PM.

**AI:** Let me check Dr. Smith’s availability for August 10th at 2 PM.

*(calls check_availability webhook)*

**AI:** Dr. Smith is available at 2 PM on August 10th. Please provide your full name.

**Patient:** John Doe.

**AI:** Your phone number, please.

**Patient:** +1234567890.

**AI:** Any email for confirmation?

**Patient:** john.doe@example.com.

**AI:** What is the reason for your visit?

**Patient:** Routine checkup.

**AI:** Booking your appointment with Dr. Smith on August 10th at 2 PM for a routine checkup. Please wait for confirmation.

*(calls book_appointment webhook)*

**AI:** Your appointment has been successfully booked. You will receive an email confirmation shortly. Thank you for choosing Wellspring Clinic!

---

**End of Demo**
