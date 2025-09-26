# 1) Next.js 앱 생성 (App Router)
npx create-next-app@latest mapket-mvp --ts --eslint
cd mapket-mvp

# 2) 의존성
pnpm add @supabase/supabase-js @supabase/auth-helpers-nextjs zod
pnpm add -D prisma
pnpm add @prisma/client

# 3) GitHub 초기 커밋
git init
git add .
git commit -m "chore: init next app"
gh repo create mapket-mvp --public --source=. --remote=origin
git push -u origin main
