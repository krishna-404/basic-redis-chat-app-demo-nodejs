# Build
## Backend
1. cd backend
2. pnpm install
3. Update (backend/.env)[backend/.env]
6. pnpm start

## React Native
1. cd whatsapp
2. yarn install
3. Update (whatsapp/env.ts)[whatsapp/env.ts] with backend url
4. npx expo prebuild

### Run prebuild in expo
```bash
npx expo run:ios
npx expo run:android
```
### Build apk
```bash
cd android
./gradlew assembleRelease
```

APK will be at
`whatsapp/android/app/build/outputs/apk/release/app-release.apk`

## Reactjs Frontend
1. Update (backend/client/.env)[backend/client/.env]
2. Update (backend/client/package.json.proxy)[backend/client/package.json.proxy] with your backend url
3. pnpm run build
--- Frontend should be running on your backend base url ---

### Run frontend seperately
1. pnpm run start