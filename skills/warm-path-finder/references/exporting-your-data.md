# How to give the skill your data (LinkedIn, Gmail, contacts)

`warm-path-finder` finds warm intro paths from data you **own and authorize** —
never by scraping. Here's exactly how to hand it that data. This is a user-facing
guide: founders can follow it directly.

---

## 1. Export your LinkedIn connections (the authorized way)

There is **no way (and no permission) to read your LinkedIn network through an
API**, and scraping LinkedIn breaks their terms and can get your account banned.
The legitimate route is to export your own connections — LinkedIn gives you a CSV
of everyone you're connected to.

### Steps (do this on a desktop browser — easier than the app)

1. Sign in to **linkedin.com** on a computer.
2. Top-right, click your photo (**Me**) → **Settings & Privacy**.
3. Left menu → **Data Privacy**.
4. Under *How LinkedIn uses your data*, click **Get a copy of your data**.
5. Choose **"Want something in particular? Select the data files you're most
   interested in"** → tick **Connections**.
6. Click **Request archive** (re-enter your password if asked).
7. LinkedIn emails you a download link. The **Connections** file is usually ready
   in **~10 minutes** (a full archive can take up to 24h).
8. Open the email → **Download archive** → unzip → open **`Connections.csv`**.

### What's in the file

Columns: `First Name, Last Name, URL, Email Address, Company, Position,
Connected On`.

- The **Email Address** column is **often blank** — LinkedIn only includes it if
  that connection chose to share their email. That's fine: **name + company +
  position is enough** to match people against your target firms and their
  portfolio companies.

### Hand it to the skill

In Claude Code, give it the file — drag `Connections.csv` into the chat, or tell
Claude the file path. Then ask: *"cross-reference my LinkedIn connections against
\<target firm\> and its portfolio, and find warm paths."* The skill matches:
- people **at** the target firm,
- **portfolio founders** of the firm (the strongest introducers),
- people who share the target person's **company or school**.

> Privacy: this is your own data. The file lists your network's names/companies —
> keep it local, and delete it when you're done if you prefer.

---

## 2. Gmail (your existing relationships)

If your Gmail is connected to your Claude session, the skill can search **your
own inbox** for people already linked to a target firm — past threads, shared
recipients, intros you've received. An existing email thread *is* a warm path.

- The skill searches **whichever Gmail account is connected** to your session.
  If you have more than one Google account, make sure the connected one is where
  your investor/founder relationships actually live.
- It only **reads** to find connections; it never sends anything without you.

---

## 3. Contacts

Export your Google/phone contacts (Google Contacts → Export → CSV) and hand that
over too, for the same name/company matching. Quick win, often overlooked.

---

## The line this never crosses

- ✅ Your **own** exported LinkedIn CSV, your Gmail, your contacts — authorized.
- ✅ **Public** info (X bios, firm team pages, portfolio, podcasts).
- ❌ Reading your LinkedIn graph via API or scraping (not possible / against ToS).
- ❌ Guessing or buying anyone's private email to mass-contact.

---

## 中文版:怎么把数据交给这个 skill

这个 skill 只用**你本人授权**的数据找暖路径,绝不爬取。

### 一、导出你的领英好友(唯一合规的方式)

**没有 API、也没有权限**能读你的领英关系链;爬领英违反条款、会被封号。正路是
**你自己导出**——领英会给你一份好友 CSV。

**步骤(用电脑浏览器,比 App 简单):**
1. 电脑上登录 **linkedin.com**。
2. 右上角点你的头像(**Me**)→ **Settings & Privacy(设置与隐私)**。
3. 左侧 → **Data Privacy(数据隐私)**。
4. 找到 **Get a copy of your data(获取你的数据副本)**。
5. 选 **"Want something in particular…"** → 勾选 **Connections(人脉)**。
6. 点 **Request archive(请求归档)**(可能要再输一次密码)。
7. 领英会邮件发你下载链接,**Connections 文件一般 ~10 分钟**就好(完整归档最多 24 小时)。
8. 打开邮件 → **Download archive** → 解压 → 打开 **`Connections.csv`**。

**文件里有什么**:姓名、领英主页 URL、邮箱(**常为空**,只有对方选择公开才有)、
公司、职位、连接时间。**邮箱空没关系**——姓名+公司+职位就够用来比对目标机构了。

**交给 skill**:在 Claude Code 里把 `Connections.csv` 拖进对话(或告诉它文件路径),
然后说:*"拿我的领英好友跟 \<目标机构\> 及其被投公司比对,找暖路径。"*
它会匹配:在该机构的人、该机构**投过的创始人**(最强引荐人)、和目标同公司/同校的人。

### 二、Gmail(你已有的关系)

连上 Gmail 后,skill 能搜**你自己的邮箱**,找出早就和目标机构有往来的人。
注意:搜的是**当前连进会话的那个 Gmail 账号**,多账号的话确认连对了。它只读不发。

### 三、通讯录

Google 通讯录 → 导出 CSV,一起给它,同样做匹配。

### 红线

✅ 你**自己导出/授权**的领英CSV、Gmail、通讯录;✅ **公开**信息(X、官网团队页、portfolio)。
❌ API/爬虫读领英关系链;❌ 猜/买私人邮箱去群发。

> 中国场景:领英在华已基本停服,关系链在**微信/脉脉/校友**里——见
> `zh-talk-tracks.md`。
