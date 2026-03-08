# Device Compliance SaaS

Enterprise-grade device compliance verification platform for remote workforce.

## Features

- 🖥️ **Hardware Verification** - CPU, RAM, monitors, webcam, BIOS validation
- 🌐 **Network Testing** - Download/upload speed and latency measurements
- 📍 **Location Rules** - Geographic restrictions with VPN detection
- 🏢 **Multi-Tenant** - Secure client isolation with Row Level Security
- 📊 **Real-time Dashboard** - Live compliance monitoring and reporting
- 🔧 **Windows Agent** - Native C# agent for system data collection

## Tech Stack

- **Frontend**: Next.js 15, React 18, TypeScript, Tailwind CSS, shadcn/ui
- **Backend**: Supabase (PostgreSQL + Auth + RLS)
- **Agent**: C# .NET 8.0 for Windows

## Getting Started

```bash
# Install dependencies
bun install

# Set up environment variables
cp .env.example .env.local

# Run development server
bun dev
```

## Environment Variables

```
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
SUPABASE_SERVICE_ROLE_KEY=your-service-key
```

## Project Structure

```
├── src/
│   ├── app/                 # Next.js App Router pages
│   │   ├── dashboard/       # Admin dashboard
│   │   ├── download/        # Agent download portal
│   │   └── api/             # API routes
│   ├── components/          # React components
│   └── lib/                 # Utilities and Supabase client
├── windows-agent/           # Windows compliance agent (C#)
└── supabase/               # Database schema
```

## License

MIT
