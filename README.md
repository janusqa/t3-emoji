# setup
$ npx create-t3-app@latest .  // skip nextauth installation

# db
set up db locally or remotely with something like supabase or planetscale
set up db conn string in .evv
set up project with connection to db in /prisma/schema.prisma
after...
$ npx prisma db push
$ npx prisma studio 

# auth
create new app on clerk.dev
choose your integrations.  Google, etc...
$ npm install @clerk/nextjs
From project dashboard get API keys (public and private), save them to .evv
Now add clerkprovider to your _app.tsx. // Note this is for nextjs. Other frameworks will have their own instructions so see the docs

