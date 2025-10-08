NeonPlay - Minimal Android Studio project (Kotlin)
-----------------------------------------------
Este é um projeto gerado automaticamente com as funcionalidades básicas:
- Tela de Login (URL, usuário, senha)
- Tela de Categorias (Canais, Filmes, Séries)
- Player com ExoPlayer para reprodução HLS/M3U8
- Tema com cores NeonPlay (escuro + ciano)
- Logo placeholder em drawable (vector)

Como abrir e gerar o APK:
1. Abra o Android Studio (recomendo Arctic Fox ou mais recente).
2. Escolha "Open an Existing Project" e selecione esta pasta (NeonPlay_project).
3. O Android Studio pode solicitar para atualizar o Gradle/Android plugin. Aceite e deixe baixar as dependências.
4. Conecte um dispositivo ou use um emulador e clique em Run (ou Build > Build Bundle(s) / APK(s) > Build APK(s)).

GitHub Actions:
- Existe um workflow em .github/workflows/android-build.yml que compila um APK debug e o disponibiliza como artefato.
- Para usar: crie um repositório, dê push do conteúdo desta pasta e o workflow rodará automaticamente em pushes para main/master ou manualmente via workflow_dispatch.


## GitHub Actions

Push this project to a GitHub repository on branch `main` (or `master`).
The workflow `.github/workflows/android-build.yml` will run and produce an APK artifact named `NeonPlay-debug-apk` that you can download from the Actions run page.

Steps:
1. Create a new empty repository on GitHub.
2. Push the contents of this folder to the repository's `main` branch.
3. Go to the Actions tab on GitHub and open the latest workflow run.
4. Download the artifact `NeonPlay-debug-apk` from the run's summary.

Note: This builds the debug APK. If you want to produce a signed release APK, additional steps are needed to provide a keystore and update the workflow.
