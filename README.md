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
