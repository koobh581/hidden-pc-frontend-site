# Render 배포 안내

이 버전은 Render Static Site 배포용으로 peer dependency 충돌 원인이던 `@builder.io/vite-plugin-jsx-loc`를 제거했습니다.

설정값:

```
Root Directory: frontend
Build Command: corepack enable && corepack prepare pnpm@10.15.1 --activate && pnpm install --no-frozen-lockfile && pnpm run build
Publish Directory: dist
```

환경변수:

```
VITE_CONTACT_API_URL=https://hiddenpc.onrender.com/api/contact
```
