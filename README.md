# Nexivion Labs

<p align="center">
  <img src="assets/nexivion-banner.svg" alt="Nexivion Labs" width="100%"/>
</p>

<p align="center">
  <b>Tüm yapay zekâ araçları tek orkestrasyon çatısı altında.</b><br/>
  <i>Every AI tool under one orchestration roof.</i>
</p>

<p align="center">
  <a href="#tr"><b>Türkçe</b></a> &nbsp;·&nbsp; <a href="#en"><b>English</b></a>
</p>

---

<a id="tr"></a>

## Türkçe

İnsan ve yapay zekânın birlikte çalıştığı yeni nesil yazılım sistemleri geliştiriyoruz.

### Sarmal: ajan fabrikası

Sarmal, yapay zekâ ajanlarını tek bir plan etrafında çalıştıran bir orkestrasyon sistemidir. Bir işi plandan başlatır, işi doğru uzman ajana verir, üretilen işi bağımsız bir denetçiye ölçtürür ve insan onayı olmadan hiçbir şeyi yayına almaz.

Sarmal'ın kadrosunda web, Android, iOS ve masaüstü uygulamaları geliştiren yazılım uzmanı ajanlar, otonom sistemler ve Meta ile Google Ads gibi iş otomasyonları yer alır. Amacımız, insanların yapay zekâ araçlarından en yüksek verimi almasını ve otomasyonlarını tek bir yerden kurabilmesini sağlamaktır.

Sarmal bugün açık kaynaklı bir planlama dili, bir motor ve bir VS Code eklentisidir. Masaüstü, web ve mobil uygulamaları da açık bir süreçle, YouTube kanalımızda kayda alınarak inşa ediliyor.

**Açık kaynak depo:** [github.com/nexivion-labs/sarmal](https://github.com/nexivion-labs/sarmal)

<p align="center">
  <a href="https://github.com/nexivion-labs/sarmal">
    <img src="https://img.shields.io/badge/Sarmal-GitHub'da%20incele-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://www.youtube.com/@nexivionlabs">
    <img src="https://img.shields.io/badge/YouTube-%C4%B0n%C5%9Fa%20s%C3%BCrecini%20izle-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/>
  </a>
</p>

#### Neyi çözüyoruz?

Yapay zekâya iş yaptırırken asıl sorun modelin zekâsı değil, niyetin kaybolmasıdır. Plan bir yerde yazılıdır, kod başka bir yere gider ve aradaki farkı kimse görmez. Sarmal projenin niyetini makinenin okuyabildiği bir dille yazdırır ve bir motor sürekli şunu sorar: planın söylediği ile diskteki gerçek hâlâ aynı mı?

```mermaid
flowchart LR
    Insan[İnsan: niyet ve onay] --> Plan[Sarmal planı]
    Plan --> Orkestra[Orkestrasyon]
    Orkestra --> Ajanlar[Uzman ajanlar]
    Ajanlar --> Denetci[Bağımsız denetçi]
    Denetci --> Onay[İnsan onayı]
    Onay --> Teslim[Teslim]
```

---

### Hakkımda

#### Fatih Özgel
**Sistem mühendisi, Nexivion Labs kurucusu**

Tek tek özellikler değil, uçtan uca çalışan yazılım sistemleri kuruyorum. Arka uç mimarisinden yapay zekâ hatlarına, arayüzden altyapıya kadar bütün katmanları birlikte tasarlıyorum.

Çalışma ilkelerim şunlar: önce sistem, sonra özellik; önce mimari ve plan, sonra kod; yapay zekâ bir eklenti değil, sistemin çekirdeğidir; yönetişim ve gözlemlenebilirlik baştan gelir.

---

<a id="en"></a>

## English

We build next-generation software systems where humans and AI work together.

### Sarmal: the agent factory

Sarmal is an orchestration system that runs AI agents around a single plan. It starts every job from the plan, hands the work to the right specialist agent, has an independent reviewer measure the result, and publishes nothing without human approval.

Sarmal's crew includes specialist software agents that build web, Android, iOS and desktop applications, autonomous systems, and business automations such as Meta and Google Ads management. Our goal is to help people get the most out of AI tools and set up their automations from a single place.

Today Sarmal is an open-source planning language, an engine and a VS Code extension. Its desktop, web and mobile apps are being built in the open and recorded on our YouTube channel.

**Open-source repository:** [github.com/nexivion-labs/sarmal](https://github.com/nexivion-labs/sarmal)

<p align="center">
  <a href="https://github.com/nexivion-labs/sarmal">
    <img src="https://img.shields.io/badge/Sarmal-View%20on%20GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://www.youtube.com/@nexivionlabs">
    <img src="https://img.shields.io/badge/YouTube-Watch%20the%20build-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/>
  </a>
</p>

#### What problem do we solve?

When you put AI to work, the real problem is not the model's intelligence but the loss of intent. The plan lives in one place, the code goes somewhere else, and nobody sees the gap between them. Sarmal writes the project's intent in a language machines can read, and an engine keeps asking one question: does what the plan says still match what is on disk?

```mermaid
flowchart LR
    Human[Human: intent and approval] --> Plan[Sarmal plan]
    Plan --> Orchestration[Orchestration]
    Orchestration --> Agents[Specialist agents]
    Agents --> Reviewer[Independent reviewer]
    Reviewer --> Approval[Human approval]
    Approval --> Delivery[Delivery]
```

### About me

#### Fatih Özgel
**Systems engineer, founder of Nexivion Labs**

I build complete software systems that work end to end, not isolated features. I design every layer together, from backend architecture and AI pipelines to the interface and the infrastructure.

My working principles: system first, features second; architecture and plan first, code second; AI is the core of the system, not a plugin; governance and observability come from day one.

---

## Teknolojiler · Tech stack

<p align="center">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white"/>
<img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
<img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
<img src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white"/>
<img src="https://img.shields.io/badge/VS%20Code%20Eklentisi-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white"/>
</p>

---

## Bize ulaşın · Get in touch

Yazılım ya da otomasyon kurmak istiyorsanız bize yazın.<br/>
<i>If you want to build software or automation, write to us.</i>

<p align="center">
<a href="https://nexivionlabs.io"><img src="https://img.shields.io/badge/Web-nexivionlabs.io-8B5CF6?style=for-the-badge"/></a>
<a href="https://www.youtube.com/@nexivionlabs"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/></a>
<a href="https://instagram.com/nexivionlabs"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
<a href="https://x.com/nexivionlabs"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/></a>
<a href="https://www.threads.net/@nexivionlabs"><img src="https://img.shields.io/badge/Threads-000000?style=for-the-badge&logo=threads&logoColor=white"/></a>
<a href="https://www.facebook.com/profile.php?id=61594925343321"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white"/></a>
<a href="https://linkedin.com/in/fatihozgel"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="https://github.com/nexivion-labs/sarmal"><img src="https://img.shields.io/badge/Sarmal-a%C3%A7%C4%B1k%20kaynak-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://github.com/nexivion-labs"><img src="https://img.shields.io/badge/GitHub-nexivion--labs-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="mailto:fatih@nexivionlabs.io"><img src="https://img.shields.io/badge/E--posta-fatih%40nexivionlabs.io-8B5CF6?style=for-the-badge"/></a>
</p>

---

> Yazılımın geleceği satır satır yazılmayacak. Akıllı ajanlarla orkestre edilecek, ilkelerle yönetilecek ve insan onayıyla teslim edilecek.
>
> *The future of software will not be written line by line. It will be orchestrated by intelligent agents, governed by principles and delivered with human approval.*

**Nexivion Labs. İnsan ve yapay zekânın birlikte ürettiği gelecek.**<br/>
*The future built by humans and AI together.*

<p align="center">
  <img src="assets/nexivion-kapak.jpg" alt="Nexivion Labs" width="100%"/>
</p>
