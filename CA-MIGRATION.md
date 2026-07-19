# Обновление сертификата (миграция с HuyandexProxy на Project2Proxy)

## Почему нужно действие

Приложение было переименовано. Старый корневой сертификат **HuyandexProxy Root CA**
больше не используется — его нужно удалить вручную, а новый установится автоматически
при первом запуске обновлённой версии.

---

## Шаг 1 — Удалить старый сертификат

1. Нажмите **Win + R**, введите `certlm.msc`, нажмите **OK**
   *(откроется хранилище сертификатов компьютера)*
2. Раскройте: **Доверенные корневые центры сертификации → Сертификаты**
3. Найдите сертификат с именем **HuyandexProxy Root CA**
4. Щёлкните правой кнопкой → **Удалить** → подтвердите

---

## Шаг 2 — Установить новый сертификат

Просто запустите **Project2Proxy.exe** от имени администратора.

Приложение автоматически сгенерирует и установит новый сертификат **Project2Proxy Root CA**.

---

## Проверка

После запуска снова откройте `certlm.msc` →
**Доверенные корневые центры сертификации → Сертификаты** —
должен появиться **Project2Proxy Root CA**.

---

## Если браузер всё равно показывает ошибку сертификата

Перезапустите браузер после установки нового CA.
В Chrome/Edge иногда требуется полный перезапуск (не просто закрыть вкладку).

---

# Certificate Update (migration from HuyandexProxy to Project2Proxy)

## Why action is needed

The application has been rebranded. The old root certificate **HuyandexProxy Root CA**
is no longer used and must be removed manually. The new certificate will be installed
automatically on the first launch of the updated version.

---

## Step 1 — Remove the old certificate

1. Press **Win + R**, type `certlm.msc`, press **OK**
   *(this opens the machine certificate store)*
2. Expand: **Trusted Root Certification Authorities → Certificates**
3. Find the certificate named **HuyandexProxy Root CA**
4. Right-click → **Delete** → confirm

---

## Step 2 — Install the new certificate

Simply run **Project2Proxy.exe** as Administrator.

The application will automatically generate and install the new **Project2Proxy Root CA** certificate.

---

## Verification

After launch, open `certlm.msc` again →
**Trusted Root Certification Authorities → Certificates** —
**Project2Proxy Root CA** should appear in the list.

---

## If the browser still shows a certificate error

Restart the browser after installing the new CA.
Chrome/Edge sometimes require a full restart (not just closing a tab).
