Render 배포 설정

Static Site 설정값
- Root Directory: frontend
- Build Command: corepack enable && corepack prepare pnpm@10.15.1 --activate && pnpm install --no-frozen-lockfile && pnpm run build
- Publish Directory: dist

환경변수
- VITE_CONTACT_API_URL=https://hiddenpc.onrender.com/api/contact

주의
- frontend 폴더 안의 pnpm-lock.yaml 과 package.json 이 달라 frozen lockfile 에러가 날 수 있어 --no-frozen-lockfile 를 사용하도록 구성되어 있습니다.
- 기존 DB/메일 서버는 hiddenpc.onrender.com 을 그대로 사용합니다.
