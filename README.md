# database-week-8
My Student Records Database
I built this to manage a small school’s student data — think of it as a simple but solid backend for tracking who’s enrolled, what they’re studying, how they’re doing, and what they’ve paid.

I used real Kenyan names (like Brian Wekesa, Festus Mwakeli, Wanjiru Otieno) because that’s the context I had in mind. Everything is stored in four clean tables:

students: Name, contact info, and current grade level
courses: Subjects offered (Math, Biology, Kiswahili, etc.)
enrollments: Connects students to courses and saves their grades
payments: Keeps track of fees paid (in KES)
The relationships just make sense:

One student → many payments
One student ↔ many courses (and vice versa)
I didn’t add indexes or fancy extras — the focus was on getting the structure right so the data stays consistent and easy to query.

If you load this into MySQL, you’ll have 100 students ready to go, each with real enrollments and payment history. You can look up anyone, check their grades, or see their payment status with a simple query.

It’s not a full app — just the database layer. But it’s built to be the reliable foundation for one.