# Кибер-Сфера 3D: Неоновый Рывок

Браузерная 3D-игра (один файл `index.html` + треки `track1.mp3` … `track5.mp3`).

**Играть онлайн:** [https://olleala2023.github.io/cyber-sphere-3d/](https://olleala2023.github.io/cyber-sphere-3d/)

**Репозиторий:** [github.com/Olleala2023/cyber-sphere-3d](https://github.com/Olleala2023/cyber-sphere-3d)

---

## Как залить изменения на GitHub

После правок в папке проекта откройте PowerShell (или терминал в Cursor) и выполните:

```powershell
cd "d:\Game\Игра для Рады"

git status
git add -A
git commit -m "Кратко: что изменили"
git push
```

Через 1–3 минуты сайт на GitHub Pages обновится (деплой идёт из ветки `main` через Actions).

### Если `git push` просит логин

- Используйте **Personal Access Token** вместо пароля: [GitHub → Settings → Developer settings → Personal access tokens](https://github.com/settings/tokens).
- Либо один раз настройте **Git Credential Manager** в Windows — после этого push будет без ввода каждый раз.

### Полезные команды

| Команда | Зачем |
|--------|--------|
| `git status` | Что изменилось, что попадёт в коммит |
| `git diff` | Посмотреть правки в файлах |
| `git log -3 --oneline` | Последние коммиты |

### Что не коммитить

В `.gitignore` уже указаны `.env` и похожие файлы с секретами. **Не добавляйте ключи API** в репозиторий.

---

## Первичная настройка (уже сделана)

Если понадобится клонировать проект на другой компьютер:

```powershell
git clone https://github.com/Olleala2023/cyber-sphere-3d.git
cd cyber-sphere-3d
```

GitHub Pages: **Settings → Pages → Source: GitHub Actions** (workflow `.github/workflows/pages.yml`).

---

История версий игры — в [CHANGELOG.md](CHANGELOG.md).
