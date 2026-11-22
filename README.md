# Две работы для MGIMO AI Challenge 2026

[Открыть демо «Пульс деканата»](https://mgimo-puls-dekanat.netlify.app)

| Трек | Архив с исходным кодом и инструкцией | SHA-256 |
| --- | --- | --- |
| МегаФон · ИИ-агент продуктовой стратегии | [Скачать ZIP](https://github.com/albert-epstein-ai/mgimo-ai-challenge-2026/releases/download/submission-2026-11-22/megafon-product-strategist-agent.zip) | `c4e5c758d77563e92e3e22750910a01d0c7cf864cf11d2cc21f9e8a17346e470` |
| МГИМО · «Пульс деканата» | [Скачать ZIP](https://github.com/albert-epstein-ai/mgimo-ai-challenge-2026/releases/download/submission-2026-11-22/puls-dekanat-booking.zip) | `1b0fcb297f62f105c41bb9486483e09dbf4722ebff6f4e6ba1cce92ac5f08f9d` |

## Своя база данных для «Пульса деканата»

Чтобы развернуть сервис в своём аккаунте Cloudflare, распакуйте архив, откройте каталог `puls-dekanat` и выполните `npm ci`. Войдите в свой аккаунт командой `npx wrangler login`, затем создайте базу командой `npx wrangler d1 create puls-dekanat-db`. В файле `wrangler.jsonc` подставьте полученный `database_id` вместо нулевого UUID в привязке `DB`. Примените схему к своей базе командой `npm run db:schema:remote`. Остальные шаги запуска описаны в README внутри архива.
