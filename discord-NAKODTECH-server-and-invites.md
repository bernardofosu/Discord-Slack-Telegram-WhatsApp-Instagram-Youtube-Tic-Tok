# 🚀 Discord Server Setup — **NAKODTECH DEVSECOPS ACADEMY**

## 🏗️ Create the server
1. Open Discord → left sidebar **+** → **Create My Own** *(matches your first screenshot)*.  
2. Pick **For a club or community** *(second screenshot)*.  
3. **Server name:** `NAKODTECH DEVSECOPS ACADEMY` → *(optional)* upload a **512×512** logo → **Create**.  
4. Right-click the server icon → **Server Settings → Overview** to tweak icon, description, etc.

---

## 🧰 Enable “Community” features (recommended for academies)
**Server Settings → Community → Enable Community** → follow the prompts:
- Set **Rules/Guidelines** channel and **Community Updates** channel.
- Turn on **Membership Screening** and set **Default notifications = Only @mentions**.

---

## 🧑‍🤝‍🧑 Core roles (permissions baseline)
**Server Settings → Roles:**
- **Admin** *(you)* – full permissions, **require 2FA** for mods.
- **Instructor**
- **TA**
- **Student**
- *(Optional)* **Alumni**

💡 Tip: disable **@everyone** from @mentioning @everyone; keep **Manage Channels** to Admin/Instructor only.

---

## 🗂️ Channel layout (copy/paste)
### 📢 **INFO**
- `#announcements` *(read-only for Admin/Instructor)*  
- `#rules`  
- `#start-here`  

### 💬 **GENERAL**
- `#lobby`  
- `#introductions`  
- `#q-and-a`  

### 🎓 **COURSES**
- `#devops-101`  
- `#cloud-aws`  
- `#security-fundamentals`  

### 🧪 **LABS**
- `#lab-help`  
- `#lab-status`  

### 🛠 **TOOLS**
- `#build-status` *(for GitHub/webhooks)*  
- `#resources`  

### 🔒 **STAFF (private)**
- `#instructors`  
- `#ta-room`  

### 🔊 **VOICE**
- **Lecture Hall** *(Voice)*  
- **Office Hours** *(Voice)*  
- *(Optional)* **Stage** channel for large talks

🔏 Make **INFO** read-only by removing **Send Messages** for **@everyone**, allow it for **Instructor/Admin**.

---

## 🛡️ Safety & moderation (fast setup)
**Server Settings → Safety Setup / AutoMod:**
- Enable **Spam** & **Profanity** filters *(tune to your culture)*.
- **Verification level:** *Medium* or *High* for public invites.
- **Require 2FA** for moderator actions *(Server Settings → Moderation)*.

---

## 🔗 Invites & onboarding
- Right-click server name → **Invite People** → **Edit Invite link** → set **Never expire** and limit **max uses** if needed.  
- **Server Settings → Onboarding (or Welcome Screen):** suggest `#start-here`, `#announcements`, `#lobby`.

---

# 🔐 Single-use invite links (FREE plan)
### ✅ What you can / ⚠️ can’t do
- ✅ Create an invite that **expires after 1 use** *(and/or after a time window).*  
- ✅ Email that link to a specific person.  
- ⚠️ You **cannot** lock an invite to a specific **email** natively. Any Discord account that clicks it first can use it. Use **1-use + short expiry + moderation**.

### 🧭 Make a single-use invite (manual)
1. Open any text channel → **Invite** *(or right-click channel → Invite People)*.  
2. Click **Edit invite link**.  
3. Set:  
   - **Expire After:** e.g., **30 minutes** *(or your choice)*  
   - **Max Uses:** **1**  
   - **Grant Temporary Membership:** **Off** *(so they aren’t auto-kicked)*  
4. **Generate** → **Copy** → email that link. After they join once, the link is **dead**.

### 🔒 Hardening so only admins can create invites
- **Server Settings → Roles → @everyone → disable “Create Invite.”**  
- Give **Create Invite** only to **Admins**.  
- Audit or revoke: **Server Settings → Invites** *(see who made what, uses left, revoke any link).*

### 🧰 Optional: add light verification
- **Server Settings → Moderation → Verification level = Medium or High.**  
- Community servers: enable **Membership Screening** *(agree to rules before chatting).*

### 🤖 Automate one-use links (bulk sending) *(optional)*
Use a bot to generate unique one-use links per person, then email them yourself:
```py
# discord.py (bot must have Create Invite on a channel)
invite = await channel.create_invite(max_uses=1, max_age=1800, unique=True, temporary=False)
# send invite.url via your email tool
```

---

## 📌 Quick checklist
- [ ] Community enabled & rules set  
- [ ] Roles created (Admin/Instructor/TA/Student/Alumni)  
- [ ] Channels created & **INFO** read-only  
- [ ] AutoMod + 2FA for mods  
- [ ] Single-use invite links configured for onboarding
