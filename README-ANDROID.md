# Orbit Android — projeto pronto para compilar

O Orbit 0.2 foi adaptado para Capacitor. **Este pacote contém código-fonte, não um APK pronto.**

## Requisitos
- Node.js 20 ou superior
- Android Studio com Android SDK e Java 17 ou superior
- Internet na primeira instalação de dependências

## Passo a passo (computador)

```bash
npm install
npm run build
npx cap add android
npx cap sync android
npx cap open android
```

No Android Studio, aguarde a sincronização do Gradle. Escolha **Build > Build Bundle(s) / APK(s) > Build APK(s)**. O APK de debug costuma ficar em `android/app/build/outputs/apk/debug/app-debug.apk`.

Ou, com Android SDK configurado, execute:

```bash
cd android
./gradlew assembleDebug
```

No Windows use `gradlew.bat assembleDebug`.

## Para instalar no celular
Transfira `app-debug.apk` para o Android, abra o arquivo e autorize a instalação de aplicativos dessa fonte, se solicitado. Para distribuição pública, gere um build assinado e revise segurança, política de privacidade e requisitos da Play Store.

## Limitações
- Os dados permanecem apenas no armazenamento local do aplicativo.
- Não há chat online, chamadas reais ou contas remotas.
- O appId `com.orbit.community` é provisório; altere antes da publicação.
- Se mudar o appId após criar a plataforma Android, será necessário ajustar o projeto nativo.
