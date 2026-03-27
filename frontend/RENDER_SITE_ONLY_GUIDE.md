Render Static Site 설정

Root Directory: frontend
Build Command: corepack enable && corepack prepare pnpm@10.15.1 --activate && pnpm install --no-frozen-lockfile && pnpm run build
Publish Directory: dist

중요:
- frontend/pnpm-lock.yaml 파일은 제거되어 있습니다.
- Render가 새 lockfile 없이 설치를 진행하므로 ERR_PNPM_OUTDATED_LOCKFILE 오류를 피할 수 있습니다.
- 환경변수: VITE_CONTACT_API_URL=https://hiddenpc.onrender.com/api/contact
