# MOMENT

GitHub Pages package. Root `index.html` is the app. `download.html` is the public presentation/install page, and `terms.html` is the registration agreement.

After deployment:
- App: `https://<account>.github.io/<repo>/`
- Download/install page: `https://<account>.github.io/<repo>/download.html`
- Agreement: `https://<account>.github.io/<repo>/terms.html`

The app is a web app/PWA, not a native Android APK or iOS IPA. On supported browsers the install prompt appears; on iOS use Safari → Share → Add to Home Screen.

Before public launch, review the agreement, add owner/support contacts and publish a complete privacy policy. Configure Supabase Auth Site URL and Redirect URLs to the deployed origin.

## Messenger — первая интеграция

В `index.html` добавлен раздел «Сообщения» с личными и групповыми диалогами, текстовыми сообщениями, реакциями, вложениями и голосовыми сообщениями. Для файлов используется приватное хранилище Supabase `chat-media`; доступ к вложениям выдаётся участникам диалога через временные подписанные ссылки.

Звонки, редактирование/удаление сообщений, приглашения в группы и инструменты модерации ещё не входят в эту первую интеграцию. Перед публичным запуском их нужно реализовать и протестировать отдельно.

Чтобы применить обновление к GitHub Pages, замените файл `MOMENT_GitHubPages/index.html` в репозитории на обновлённый `index.html` из этого архива. Остальные файлы проекта сохранены.
