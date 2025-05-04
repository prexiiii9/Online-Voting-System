E-Vote is a secure and user-friendly online voting platform tailored for Barangay elections. The system ensures integrity by enforcing one vote per registered user, providing real-time result updates, and maintaining transparency through audit logs. Voters can cast votes for Barangay Captain, Sangguniang Kabataan (SK) Chairman, and up to seven Councilors.

Features
✅ User Registration & Authentication – Voters register using verified email or unique voter ID.
✅ Candidate Management – Admins can add or edit candidates, upload photos, and define platforms.
✅ One Vote Per Account – Prevents multiple voting from a single account.
✅ Secure Voting – Implements encryption for vote integrity.
✅ Real-Time Results – Automatic vote tallying and updates.
✅ Audit Logs – Tracks all vote-related actions for transparency.
✅ Responsive Design – Accessible via desktop, tablet, and mobile.

 Project Structure
E-Vote/
├── public/               # Static assets (images, index.html)
├── src/                  # Application source code
│   ├── components/       # Reusable React/Vue components
│   ├── pages/            # Page-level components (Homepage, Login, Register)
│   ├── services/         # API calls, Auth logic
│   ├── context/          # Authentication context or Redux store
│   └── App.js            # Main app configuration
├── backend/              # Node.js/Express or Laravel backend
│   ├── controllers/      # Request logic (Vote, Auth, Users)
│   ├── models/           # DB Models (Users, Votes, Candidates)
│   ├── routes/           # API endpoints
│   └── server.js         # Server entry point
├── database/             # SQL Scripts or Firebase rules
├── README.md             # Project documentation
├── package.json          # Project dependencies
└── .env                  # Environment variables

Voting System Logic
Voter registers/logs in using email or voter ID.
System checks if user has already voted:
✅ If NO, voting page loads.
❌ If YES, show: "You have already voted."
