# Здача WS7

## Дані

- Роль: dev
- Команда: property-workflows
- GitHub-логін: vhrytsyndyshynquitcode
- Ваше репо: https://github.com/vhrytsyndyshynquitcode/property-workflows
- SHA: 8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a
- Репо вимог PM: https://github.com/solomchaak/property-workflows-spec
- Прод-URL: https://property-workflows-one.vercel.app

## PM

—

## Розробник

- Рядок «Вимоги:» з `docs/conformance.md` на SHA: Вимоги: https://github.com/solomchaak/property-workflows-spec · джерело: issues · знімок 2026-10-26
- PR «Оновлення вимог» зі зрізом 2 (A): https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/12
- PR «Оновлення вимог» після уточнень PM (A): /requirements-sync 2026-10-26: Вимоги актуальні (issues solomchaak/property-workflows-spec#1, #2, #3, #19, #20 — `updatedAt` збігається зі знімком; на питання #32 і #33 PM ще не відповів)
- Питання в репо PM (A; щонайменше 2, з них щонайменше 1 — власне issue): https://github.com/solomchaak/property-workflows-spec/issues/32, https://github.com/solomchaak/property-workflows-spec/issues/33
- PR «Специфікація» з `add-<зріз2>` (A): https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/14
- Дизайн-система — PR (B): https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/13
- Дизайн-система — `DESIGN.md` і джерело (B): https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/DESIGN.md · джерело: AI-чат: Claude Code (Claude Opus 5.5)
- Дизайн-система — прогін `architecture` на `main` (B): https://github.com/vhrytsyndyshynquitcode/property-workflows/actions/runs/40300003406
- Знімки «до/після» (B): https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-before-runs-light.png, https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-after-runs-light.png (також `login` і `home`, світла й темна теми: `docs/img/ws7-before-*`, `docs/img/ws7-after-*`)
- Зміна `impl-<зріз2>` (C): https://github.com/vhrytsyndyshynquitcode/property-workflows/tree/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/openspec/changes/archive/2026-10-26-impl-template-versions
- PR-и задач «Реалізація» (C; щонайменше 2): https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/16, https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/17, https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/18, https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/19 — рев'ю CodeRabbit до merge мають https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/13 (дизайн-система) і https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/19; на #16–#18 CodeRabbit не встиг до merge, їхній код перевірено й виправлено в #19
- Мутаційна перевірка — червоні прогони (C; щонайменше 2): https://github.com/vhrytsyndyshynquitcode/property-workflows/actions/runs/40295115497 (AC-EDITOR-08: `save_template_version` без перевірки ролі), https://github.com/vhrytsyndyshynquitcode/property-workflows/actions/runs/40295378603 (AC-EDITOR-02: політика робочої копії `using (true)`); зелений після revert — https://github.com/vhrytsyndyshynquitcode/property-workflows/actions/runs/40295702568
- ADR (D): https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/decisions/0001-template-versions-draft-and-immutable-versions.md, https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/decisions/0002-design-system-shadcn-tokens.md
- Архітектурне правило, крім `check:design` (D): job «Секретний ключ лише на сервері» (`scripts/check-server-boundary.mjs`) у `.github/workflows/architecture.yml` — червоний прогін на коміті-порушенні (Supabase-клієнт із `SUPABASE_SECRET_KEY` поза `admin.ts`): https://github.com/vhrytsyndyshynquitcode/property-workflows/actions/runs/40299502181, PR https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/17
- Акаунти для PM (E): pm-admin@example.test (admin), pm-manager@example.test (manager)
- Скріни за ролями (E): https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-role-admin-edit.png, https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-role-admin-versions.png, https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-role-manager-template.png, https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-role-manager-edit-denied.png, https://github.com/vhrytsyndyshynquitcode/property-workflows/blob/8a4ef1a586c2c953eda50fe7c81757f8f1cf5a6a/docs/img/ws7-role-manager-versions-denied.png (повний набір — PR https://github.com/vhrytsyndyshynquitcode/property-workflows/pull/18)
- AC зрізу 2 (E): AC-DSYS-01 (реалізовано), AC-DSYS-02 (реалізовано), AC-DSYS-03 (реалізовано), AC-DSYS-04 (реалізовано), AC-EDITOR-01 (реалізовано), AC-EDITOR-02 (реалізовано), AC-EDITOR-03 (реалізовано), AC-EDITOR-04 (реалізовано), AC-EDITOR-05 (реалізовано), AC-EDITOR-06 (реалізовано), AC-EDITOR-07 (реалізовано), AC-EDITOR-08 (реалізовано), AC-EDITOR-09 (реалізовано)
- Відхилення від PM (E): не надходило

## Бонус

—
