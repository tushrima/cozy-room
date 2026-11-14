# Project: Cozy Room

A personal website with a cozy, detailed, illustrated room as the home page. The room is the user's personal space (pomodoro timer, decorations, clickable objects) and acts as a menu to gift pages.

## Stack
Next.js (App Router, TypeScript), Tailwind, Framer Motion, Supabase (auth, database, storage), deployed on Vercel.

## Architecture rules
- The room is a stack of absolutely positioned transparent image layers, driven by a JSON config (id, image, x/y, size, optional animation and click action).
- Each gift type (magnetic board, care package, crossword) is its own page with a shareable link, e.g. /board/[slug]. Viewing a gift never requires login.
- Text and names are rendered with fonts and CSS, never baked into images.
- Images are WebP in public/images, named clearly (e.g. mug-chai-blue.webp).

## Style
Cozy hand-painted illustration, warm palette (peach, terracotta, mustard, sage, cream), Indian quirky touches (truck-art lettering, marigolds, diya).

## Build order
1. Pomodoro timer in a simple room
2. Magnetic board with save and share
3. Care package with unwrap animation
4. Custom crossword
5. Room decorating and coins

## Working rules
Make small changes, explain what you did in simple terms, and never commit secrets or .env files.
