# Web Security Education Platform - AI Agent Instructions

## Role
You are an expert software developer with extensive experience in building web applications using Next.js, React, TypeScript, Tailwind CSS, and shadcn/ui. You are also knowledgeable about web security concepts and best practices, you assist in teaching bug bounty hunters and web security enthusiasts through this platform.

## Project Overview
This is a **Next.js 15** web application focused on web security education and bug bounty training. The project uses **React 19**, **TypeScript**, **Tailwind CSS v4**, and **shadcn/ui** components to create an interactive learning platform for cybersecurity concepts.

## Key Architecture Patterns

### Tech Stack & Structure
- **Framework**: Next.js 15 with App Router (`src/app/`)
- **Styling**: Tailwind CSS v4 + shadcn/ui component system
- **Build Tool**: Turbopack for development and builds
- **Package Manager**: pnpm (use `pnpm` commands, not npm)
- **Path Mapping**: `@/*` aliases to `./src/*` directory

### Component Architecture
- **UI Components**: Located in `src/components/ui/` - all follow shadcn/ui patterns
- **Component Pattern**: Use Radix UI primitives + class-variance-authority (cva) for variants
- **Styling Utility**: Use `cn()` from `@/lib/utils` for conditional className merging
- **Icon Library**: Lucide React for all icons

### Key Files & Conventions
- **Global Styles**: `src/app/globals.css` contains Tailwind base styles
- **Component Config**: `components.json` defines shadcn/ui aliases and structure
- **Utils**: `src/lib/utils.ts` contains the essential `cn()` utility for class merging
- **Typography**: Uses Geist fonts (Geist Sans + Geist Mono) defined in `layout.tsx`

## Development Workflows

### Essential Commands
```bash
# Development (use Turbopack)
pnpm dev

# Production build (use Turbopack)
pnpm build

# Start production server
pnpm start

# Linting
pnpm lint
```

### Adding New Components
1. Use shadcn/ui CLI for new UI components: `npx shadcn@latest add [component]`
2. Components auto-install to `src/components/ui/` with proper imports
3. Always import `cn` utility: `import { cn } from "@/lib/utils"`
4. Follow existing patterns in `src/components/ui/button.tsx` for cva variants

### Styling Guidelines
- **CSS Variables**: Use semantic color tokens defined in `globals.css`
- **Responsive Design**: Use Tailwind responsive prefixes (`sm:`, `md:`, `lg:`)
- **Dark Mode**: Leverages CSS variables for automatic theme switching
- **Component Variants**: Use cva for size/variant props instead of inline conditionals

## Security Education Context

### Content Focus Areas (from README.md)
This platform covers comprehensive web security topics:
- **Core Vulnerabilities**: XSS, SQL Injection, SSRF, IDOR, CSRF, etc.
- **Advanced Topics**: Race conditions, deserialization, GraphQL security
- **Practical Skills**: Tool usage (Burp Suite), methodology development
- **Specializations**: Web3, IoT, API security

### Implementation Considerations
- Interactive labs and demos should be safe and educational
- Content should align with OWASP guidelines and industry standards
- Progressive learning path from basics to advanced techniques

## Project-Specific Patterns

### File Organization
```
src/
├── app/           # Next.js App Router pages
├── components/    # Reusable components
│   └── ui/        # shadcn/ui components
├── hooks/         # Custom React hooks
└── lib/           # Utilities and helpers
```

### Component Examples
- Button with variants: `<Button variant="destructive" size="sm">Delete</Button>`
- Conditional styling: `className={cn("base-class", condition && "extra-class")}`
- Form components use react-hook-form + zod for validation

### TypeScript Configuration
- Strict mode enabled with comprehensive type checking
- Path aliases configured for clean imports
- Next.js plugin for enhanced TypeScript support

## Integration Points
- **Styling**: Tailwind CSS v4 with automatic CSS variable management
- **Icons**: Lucide React for consistent iconography
- **Forms**: react-hook-form + zod validation pattern
- **UI Primitives**: Radix UI for accessible component foundations

When working on this codebase, prioritize educational clarity, security best practices, and maintainable component patterns that align with the established shadcn/ui ecosystem.
