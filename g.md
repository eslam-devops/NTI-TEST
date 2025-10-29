## Git Commands Quick Notes

**Check Global Config**

```
git config --global user.email
git config --global user.name
```

**Start Git in Folder**

```
git init
```

**Create README file**

```
echo "# CICD-PROJECT" >> README.md
```

**Add Files**

```
git add .
```

**Commit Changes**

```
git commit -m "Initial commit"
```

**Connect Local Repo with GitHub Remote**

```
git remote add origin <URL>
```

**Rename Branch to main**

```
git branch -M main
```

**Push for the first time**

```
git push -u origin main
```


تمام ✅
لو عندك **ريبو محلي (local)** وعايز تربطه بريبو موجود على GitHub (remote)،
بنستخدم الأمر ده:

---

## 🔗 ربط الريموت بالـ local repo

```bash
git remote add origin <URL>
```

مثال عندك أنت 👇

```bash
git remote add origin https://github.com/eslam-devops/NTI-TEST.git
```

---

## ✅ بعد الربط أول Push لازم يبقى كده:

```bash
git branch -M main
git push -u origin main
```

* `-M main` → يخلي اسم الفرع الأساسي `main`
* `-u` → يربط الفرع المحلي بالفرع الريموت
  علشان بعد كده تقدر تعمل:

  ```bash
  git push
  git pull
  ```

  بدون كتابة اسم الريموت والفرع

---

## 🔍 أشوف الريموتات المرتبطة بالريبو

```bash
git remote -v
```

هيرجع لك:

```
origin  https://github.com/... (fetch)
origin  https://github.com/... (push)
```

---

### 🔥 تلخيص سريع

| المهمة                      | الأمر                         |
| --------------------------- | ----------------------------- |
| ربط الريبو المحلي بالريمووت | `git remote add origin <URL>` |
| تغيير الفرع الرئيسي لـ main | `git branch -M main`          |
| أول push للريمووت           | `git push -u origin main`     |
| عرض الريموتات               | `git remote -v`               |

---

لو تحب…
نعمل معًا الخطوات دي على ريبو جديد وتنفّذها بيدك؟ 🚀

