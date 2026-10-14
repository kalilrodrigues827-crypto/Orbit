# Orbit - Gerar APK no GitHub pelo celular

1. Extraia o ZIP. Entre na pasta `orbit-android` e envie **o conteúdo dessa pasta**, não a pasta externa, para a raiz do repositorio no GitHub. Inclua `.github/workflows/android-apk.yml`.
2. Na aba **Actions** do repositorio, selecione **Gerar APK do Orbit** e toque em **Run workflow** (ou aguarde a compilacao iniciada pelo push na branch `main`).
3. Quando o job terminar com sucesso, abra a execucao e baixe o artefato **Orbit-Android-APK**.
4. Extraia o ZIP do artefato para encontrar `app-debug.apk` e abra o APK no Android para instalar.

Importante: o ZIP do projeto NAO e o APK. O arquivo do artefato pode vir compactado em outro ZIP.

Caso o GitHub nao mostre Actions no celular, use o navegador com a opcao 'Site para computador'.

Este e um APK debug para testes, sem backend online e sem chamadas reais. Para publicar na Play Store, configure assinatura release, privacidade e identificador definitivo.
