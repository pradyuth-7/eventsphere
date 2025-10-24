# EventSphere - Event Management Platform

EventSphere is a modern, full-featured event management platform that enables users to discover, create, and manage events seamlessly. Built with a focus on user experience and accessibility, EventSphere provides both event organizers and attendees with powerful tools to connect and collaborate.

## ✨ Features

### For Event Attendees
- **User Authentication**: Secure login and signup with role-based access
- **Event Discovery**: Browse and search events with advanced filtering by category
- **Event Registration**: Easy registration for events with confirmation notifications
- **Event Details**: View comprehensive event information including date, time, location, and organizer details
- **Event Feedback**: Leave ratings and feedback for attended events
- **User Profile**: Manage personal information and view registered events

### For Event Organizers
- **Event Creation**: Create and publish events with detailed information
- **Event Management Dashboard**: View all created events with statistics
- **Registration Tracking**: Monitor attendee registrations and event capacity
- **Event Analytics**: Track event performance and attendee engagement
- **Event Editing**: Update event details and manage event information
- **Event Deletion**: Remove events when needed

### General Features
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Vibrant UI**: Colorful, modern interface with smooth interactions
- **Real-time Updates**: Instant feedback on user actions
- **Data Persistence**: All data stored locally using browser localStorage
- **Search & Filter**: Powerful search across event titles, descriptions, and locations
- **Category Filtering**: Filter events by category (Technology, Sports, Music, etc.)
- **Sorting Options**: Sort events by date, popularity, or registration count

## 🛠️ Tech Stack

### Frontend
- **React 19** - UI library
- **Next.js 16** - React framework with App Router
- **TypeScript** - Type-safe JavaScript
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - High-quality React components
- **Lucide React** - Beautiful icon library

### Storage
- **localStorage** - Client-side data persistence (no backend required)

## 📋 Project Structure

\`\`\`
eventsphere/
├── app/
│   ├── page.tsx                 # Homepage
│   ├── layout.tsx               # Root layout
│   ├── globals.css              # Global styles
│   ├── dashboard/
│   │   ├── page.tsx             # Organizer dashboard
│   │   └── create/
│   │       └── page.tsx         # Create event page
│   ├── events/
│   │   └── page.tsx             # Events browsing page
│   ├── profile/
│   │   └── page.tsx             # User profile page
│   ├── feedback/
│   │   └── [eventId]/
│   │       └── page.tsx         # Event feedback page
│   └── loading.tsx              # Loading state
├── components/
│   ├── auth-modal.tsx           # Authentication modal
│   ├── event-list.tsx           # Event listing component
│   ├── events-dashboard.tsx     # Dashboard component
│   ├── create-event-form.tsx    # Event creation form
│   ├── dashboard-layout.tsx     # Dashboard layout
│   ├── toaster.tsx              # Toast notifications
│   └── ui/                      # shadcn/ui components
├── hooks/
│   └── use-auth.tsx             # Authentication hook
├── index.html                   # Standalone HTML version
└── README.md                    # This file
\`\`\`

## 🚀 Getting Started

### Option 1: Run as Next.js Project

#### Prerequisites
- Node.js 18+ installed
- npm or yarn package manager

#### Installation

1. **Clone the repository**
   \`\`\`bash
   git clone https://github.com/yourusername/eventsphere.git
   cd eventsphere
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   \`\`\`

3. **Run the development server**
   \`\`\`bash
   npm run dev
   \`\`\`

4. **Open in browser**
   - Navigate to `http://localhost:3000`
   - The app will automatically reload on code changes

### Option 2: Run as Standalone HTML

1. **Open the HTML file**
   - Simply open `index.html` in your web browser
   - Or use VS Code Live Server extension:
     - Right-click on `index.html`
     - Select "Open with Live Server"

2. **No installation required**
   - All functionality works with just the HTML file
   - Data persists in your browser's localStorage

## 📖 Usage Guide

### Getting Started as a Student/Attendee

1. **Sign Up**
   - Click "Sign Up" on the homepage
   - Enter your email and password
   - Select "Student" as your role
   - Click "Sign Up"

2. **Browse Events**
   - View featured events on the homepage
   - Click "View All Events" to see the complete event list
   - Use search to find specific events
   - Filter by category to narrow results

3. **Register for Events**
   - Click on an event to view details
   - Click "Register" button
   - Confirm your registration
   - View your registered events in your profile

4. **Leave Feedback**
   - After an event, click "Leave Feedback"
   - Rate the event (1-5 stars)
   - Add your comments
   - Submit feedback

### Getting Started as an Organizer

1. **Sign Up as Organizer**
   - Click "Sign Up" on the homepage
   - Enter your email and password
   - Select "Organizer" as your role
   - Click "Sign Up"

2. **Create an Event**
   - Go to Dashboard (click your name in header)
   - Click "Create New Event"
   - Fill in event details:
     - Event name
     - Description
     - Date and time
     - Location
     - Category
     - Capacity
   - Click "Create Event"

3. **Manage Events**
   - View all your events in the dashboard
   - See registration statistics
   - Edit event details
   - Delete events if needed

4. **Track Registrations**
   - Monitor attendee count
   - View registration status
   - Track event popularity

## 🎨 Design Features

- **Vibrant Color Scheme**: Blue, green, purple, and orange gradients
- **Responsive Layout**: Mobile-first design that works on all devices
- **Smooth Animations**: Hover effects and transitions for better UX
- **Accessibility**: WCAG compliant with proper contrast ratios
- **Modern Typography**: Clean, readable fonts with proper hierarchy

## 💾 Data Storage

EventSphere uses browser localStorage for data persistence:
- **Users**: Stored with hashed passwords (demo only)
- **Events**: Complete event information and metadata
- **Registrations**: User event registrations and status
- **Feedback**: Event ratings and user comments

All data is stored locally in your browser and never sent to external servers.

## 🔐 Security Notes

This is a demo application using localStorage. For production use:
- Implement proper backend authentication
- Use secure password hashing (bcrypt, argon2)
- Add HTTPS encryption
- Implement proper authorization checks
- Use a real database (PostgreSQL, MongoDB, etc.)
- Add rate limiting and input validation

## 🤝 Contributing

Contributions are welcome! Here's how to contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🐛 Known Limitations

- Data is stored locally and will be lost if browser cache is cleared
- No real email notifications (simulated in UI)
- No backend server or database
- Single-device usage (data doesn't sync across devices)

## 🚀 Future Enhancements

- Backend API integration
- Real database storage
- Email notifications
- Social sharing features
- Advanced analytics dashboard
- Event recommendations
- User messaging system
- Payment integration for paid events
- Calendar integration
- Mobile app version

## 📞 Support

For issues, questions, or suggestions, please open an issue on GitHub or contact the development team.

## 🙏 Acknowledgments

- Built with [Next.js](https://nextjs.org/)
- UI components from [shadcn/ui](https://ui.shadcn.com/)
- Icons from [Lucide React](https://lucide.dev/)
- Styling with [Tailwind CSS](https://tailwindcss.com/)

---

**Happy event managing! 🎉**
