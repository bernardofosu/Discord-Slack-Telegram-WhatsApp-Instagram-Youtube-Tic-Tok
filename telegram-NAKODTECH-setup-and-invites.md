# 📲 Telegram Setup — **NAKODTECH DEVSECOPS ACADEMY**

This gives you a clean, admin-ready Telegram setup with **invite-only joining** using **single-use links**.

---

## 🏗️ Pick your structure
- **Group (recommended for classes):** interactive chat, topics, moderation tools.  
- **Channel (announcements-only):** one‑way broadcast. You can **link a discussion group** to let students reply.

> Tip: Use **both** — a Channel named *“NAKODTECH DEVSECOPS ACADEMY — Announcements”* linked to a Group *“NAKODTECH DEVSECOPS ACADEMY”* for Q&A.

---

## 🚀 Create the Group
**Telegram Mobile/Desktop → New Chat → New Group**  
1) Add at least one contact (you can remove later).  
2) **Name:** `NAKODTECH DEVSECOPS ACADEMY`  
3) **Avatar:** 512×512 logo, **Description:** short mission + rules link.  
4) Open **Group Info → Edit (✏️) → Type** → set **Private**.  
5) **Permissions:** disable “Add Users” for members; only admins can invite.  
6) **Approve New Members:** **ON** (new joins require approval).  
7) **Topics:** **ON** (lets you organize channels inside the group).  
8) (Optional) **Slow Mode**: 5–10s to reduce spam in busy classes.

### 🎛️ Admin roles
**Group Info → Administrators → Add Admin**  
Create roles:
- **Owner** (you) – all rights.  
- **Instructor** – manage messages, topics, invite links, pin messages.  
- **TA** – delete messages, restrict users, pin messages.  
- **Student** – default member (no admin rights).

---

## 🧭 Suggested Topics (inside the Group)
- 📢 **Announcements** *(admins post; lock replies if you want)*  
- 💬 **General / Lobby**  
- ❓ **Q&A**  
- 🧪 **Labs Help**  
- 🔐 **Staff (private)** *(create a separate private group if you need truly private staff chat)*

> Pin a **Start Here** message with syllabus, schedule, and code of conduct.

---

## 📣 Create the Announcements Channel (optional but recommended)
**New Channel → Public or Private**  
1) Name: `NAKODTECH DEVSECOPS ACADEMY — Announcements`  
2) **Link a Discussion Group**: choose your Academy group.  
3) Only admins can post; students discuss in the linked group under each post.

---

## 🔐 Single‑Use Invite Links (per person; free)
You can create **unique links** that **expire after 1 join** and/or after a **time limit**.

**Group Info → Invite Links → Create New Link → (⚙️ Edit link):**
- **Users:** set to **1** (single use).  
- **Expires in:** e.g., **30 minutes** *(your choice)*.  
- **Name the link:** e.g., “Invite — Alice”.  
- **Save → Copy** and email it to that person.

**Behavior:** first person to use it joins (or sends a **Join Request** if approvals are on). After it’s used **once**, the link is **dead**. If they leave later, the link **does not reactivate**.

**Track / revoke:** **Group Info → Invite Links** shows usage; you can delete any link anytime.

> If you need stricter control, keep **Approve New Members = ON** so each join requires your tap to approve.

---

## 🛡️ Moderation & Safety
- **Default permissions:** restrict stickers/links if needed, enable gradually.  
- **Delete & Restrict:** long‑press a message → **Delete** or **Restrict** the user.  
- **Recent Actions log:** **Group Info → Administrators → Recent Actions** to audit bans/edits.  
- **Anti‑spam:** consider adding a lightweight verification bot (CAPTCHA) if you open invites widely.

---

## 🧩 Onboarding — pinned “Start Here” (copy/paste)
```
Welcome to NAKODTECH DEVSECOPS ACADEMY! 🎓

1) Read the rules in Announcements → Pinned.  
2) Introduce yourself in General (role, goals).  
3) Lab questions → Labs Help topic.  
4) Respect others; no spam; keep DMs professional.  
5) Office hours posted weekly.
```
Pin this in the **Announcements** topic and update as the course evolves.

---

## 📌 Quick Checklist
- [ ] Group created, **Private**, **Approve New Members = ON**  
- [ ] Admin roles set (Owner/Instructor/TA)  
- [ ] Topics created (Announcements, General, Q&A, Labs)  
- [ ] Channel (Announcements) linked to the group *(optional)*  
- [ ] **Single‑use invite links** generated & emailed per student  
- [ ] Pinned **Start Here** + rules

---

## ❓FAQ
**Can I lock a link to a specific email?** → Not natively. Use **single‑use + short expiry + approvals**.  
**Can members create invites?** → Turn that **off** in Permissions. Only admins create links.  
**If a student shares their link?** → First click wins; if the wrong account joins, **deny** the join request or **kick** and **revoke** that link.
