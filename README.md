<div align="center">

<img src="https://raw.githubusercontent.com/shashank03-dev/shashank03-dev/main/assets/banner.jpg" alt="All you ever need is a passion to follow" width="100%" />

<br/>
<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=15&pause=1100&color=E6A93F&center=true&vCenter=true&width=820&lines=I+build+AI+agents+and+the+backends+they+run+on;GovBot%3A+WhatsApp+%2B+LangGraph%2C+answering+real+govt+queries;MotionCode%3A+drop+in+a+UI+clip%2C+get+GSAP+or+Framer+code+back;Wrote+a+relational+database+in+C.+B-trees%2C+no+libraries.;Bengaluru%2C+India.+Building+mostly+for+home.)](https://github.com/shashank03-dev)

<br/>

<a href="https://linkedin.com/in/shashank3162">
  <img src="https://img.shields.io/badge/LinkedIn-0A0D14?style=for-the-badge&logo=linkedin&logoColor=E6A93F" alt="LinkedIn" />
</a>
&nbsp;
<a href="mailto:shashankgowda3162@gmail.com">
  <img src="https://img.shields.io/badge/Email-0A0D14?style=for-the-badge&logo=gmail&logoColor=E6A93F" alt="Email" />
</a>
&nbsp;
<a href="https://govbot-fawn.vercel.app">
  <img src="https://img.shields.io/badge/GovBot-live%20%E2%86%97-E6A93F?style=for-the-badge&labelColor=0A0D14" alt="GovBot live" />
</a>
&nbsp;
<a href="https://motioncode.live">
  <img src="https://img.shields.io/badge/MotionCode-live%20%E2%86%97-E6A93F?style=for-the-badge&labelColor=0A0D14" alt="MotionCode live" />
</a>
&nbsp;
<img src="https://komarev.com/ghpvc/?username=shashank03-dev&style=for-the-badge&color=E6A93F&labelColor=0A0D14&label=views" alt="profile views" />

</div>

---

## whoami

I'm Shashank, an engineer in Bengaluru. Most of what I build sits in two places: AI agents that do something useful for ordinary people, and the lower-level systems underneath them. I tend to keep going until a thing is actually deployed and someone other than me is using it.

```jsonc
{
  "i_build"     : "AI agents + the backends they run on",
  "shipped"     : ["GovBot (live)", "MotionCode (live)"],
  "for_fun"     : "a relational DB engine in C: B-tree index, query parser, page I/O",
  "currently_on": ["multi-agent design", "NVIDIA's deep-learning track", "storage internals"],
  "one_rule"    : "if it isn't deployed, it doesn't count",
  "ping_me_for" : ["agent systems", "hard backend problems", "anything built for India"]
}
```

---

## Things I've shipped

<details open>
<summary><b>🤖 GovBot</b> &nbsp;·&nbsp; WhatsApp-first AI for Indian government services &nbsp;&nbsp;<code>● live</code></summary>
<br/>

Government portals are hard to use, and most people would rather just ask a question in a chat. GovBot lets a citizen message on WhatsApp in plain language. A LangGraph multi-agent setup figures out the intent, runs a RAG pipeline over government documents I scrape with Playwright, and sends back a clear answer in seconds. There's a Next.js operator dashboard for watching sessions and managing the knowledge base.

| Layer | Stack |
|---|---|
| Agents | LangGraph |
| Backend | FastAPI |
| Vectors | ChromaDB |
| Scraping | Playwright |
| Data | Supabase |
| Frontend | Next.js 15 |
| Channel | Meta WhatsApp Cloud API |
| Hosting | Railway + Vercel |

🔗 [govbot-fawn.vercel.app](https://govbot-fawn.vercel.app)

</details>

<details>
<summary><b>🎬 MotionCode</b> &nbsp;·&nbsp; Turn a UI clip into production motion code &nbsp;&nbsp;<code>● live</code></summary>
<br/>

Record a short clip or GIF of a UI animation and MotionCode reads the motion: easing, timing, transforms, opacity. It turns that into a normalized motion spec and starter code for CSS, GSAP, or Framer Motion, so you stop guessing easing curves by hand. Built on Next.js 16 with Supabase (Postgres + RLS) and Gemini doing the analysis. Free beta, with a per-user daily quota.

`Next.js 16` · `TypeScript` · `Gemini` · `Supabase` · `GSAP` · `Framer Motion`

🔗 [motioncode.live](https://motioncode.live)

</details>

<details>
<summary><b>🌾 AgriAI (kisaan)</b> &nbsp;·&nbsp; Crop diagnosis and yield prediction for smallholder farmers</summary>
<br/>

A farmer photographs a sick crop and gets a diagnosis back, with a spoken answer for anyone who would rather listen than read. Disease detection runs on GPT-4o vision, with a TFLite model for offline use where the network drops out, XGBoost for yield prediction, and TTS for the voice side. Built in a 36-hour hackathon and aimed squarely at Indian agriculture.

`GPT-4o Vision` · `TFLite (offline)` · `XGBoost` · `TTS` · `FastAPI` · `Docker`

</details>

<details>
<summary><b>💊 MedStock AI</b> &nbsp;·&nbsp; Inventory and demand forecasting for healthcare supply</summary>
<br/>

Hospitals run out of the wrong things at the wrong time. MedStock AI tracks medical stock in real time, forecasts demand, flags expiring batches, and handles urgent supply requests across multiple hospitals and departments, with dashboards and alerts for the people running it.

`TypeScript` · `AI forecasting` · `Real-time` · `Multi-tenant`

</details>

<details>
<summary><b>🗄️ nano_database</b> &nbsp;·&nbsp; A relational database engine written from scratch in C</summary>
<br/>

No SQLite, no libraries, no safety net. A hand-rolled B-tree index, a custom tokenizer and query parser, page-based disk I/O, and manual memory management, all in C, because I wanted to know what actually happens when you type `SELECT *`. Reading about databases is one thing. Building one teaches you the parts the articles skip.

`C` · `B-tree` · `Query parser` · `Page I/O` · `Manual memory`

</details>

<details>
<summary><b>🔊 ai_voice_detection</b> &nbsp;·&nbsp; Telling synthetic speech from real human audio</summary>
<br/>

A classifier that separates AI-generated speech from genuine recordings. Feature extraction uses MFCC coefficients, spectral centroid, and zero-crossing rate, with a binary classifier trained on labeled audio. Works straight off raw audio files.

`Python` · `scikit-learn` · `Librosa` · `MFCC` · `Spectral features`

</details>

---

## How I build

**AI systems** &nbsp; `Python` · `LangGraph` · `FastAPI` · `ChromaDB` · `Playwright` · `OpenAI` · `Gemini` · `Claude`

**Web** &nbsp; `Next.js 16` · `React` · `TypeScript` · `Tailwind` · `Supabase` · `PostgreSQL`

**Close to the metal** &nbsp; `C` · `B-trees` · `Storage engines` · `Linux`

**Mobile** &nbsp; `Flutter` · `Dart` · `Firebase`

**Infra** &nbsp; `Docker` · `Vercel` · `Railway` · `Google Cloud` · `Git`

<div align="center"><br/>
<img src="https://skillicons.dev/icons?i=python,ts,nextjs,react,fastapi,c,dart,flutter,postgres,supabase,docker,linux,git,figma&theme=dark&perline=7" alt="tech stack" />
</div>

---

## The numbers

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=shashank03-dev&show_icons=true&hide_border=true&bg_color=0A0D14&title_color=E6A93F&icon_color=E6A93F&text_color=8B95A6&count_private=true&rank_icon=github" alt="GitHub stats" />
&nbsp;&nbsp;
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shashank03-dev&layout=compact&hide_border=true&bg_color=0A0D14&title_color=E6A93F&text_color=8B95A6&langs_count=8" alt="Top languages" />

<br/><br/>

<img src="https://streak-stats.demolab.com?user=shashank03-dev&hide_border=true&background=0A0D14&stroke=6FB2C9&ring=E6A93F&fire=E6A93F&currStreakLabel=E6A93F&sideLabels=8B95A6&dates=8B95A6&currStreakNum=F0E9DA&sideNums=F0E9DA" alt="GitHub streak" />

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=shashank03-dev&bg_color=0A0D14&color=F0E9DA&line=E6A93F&point=6FB2C9&area_color=15110A&area=true&hide_border=true" alt="Contribution graph" />

</div>

---

<div align="center">

<sub><i>Leap ahead, lap by lap. 🏁</i></sub>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0D14,60:15110A,100:5a3d12&height=110&section=footer" alt="" />

</div>
