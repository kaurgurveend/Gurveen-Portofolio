# PRD — Portofolio QA & Project Management

> **Dokumen:** Product Requirements Document (v0.3)
> **Tanggal:** 22 September 2026
> **Status:** Final draft v2 — berdasarkan feedback pemilik (kurangi kesan AI, balance QA-PM, hapus section yang tidak perlu)

---

## 1. Ringkasan

| Item | Keterangan |
|---|---|
| **Nama Produk** | Portofolio pribadi — Gurveender Jeet Kaur |
| **Tipe** | Single-page website, clean & profesional |
| **Audiens** | Recruiter / hiring manager untuk posisi **QA** dan **Project Management** (intern/entry level) |
| **Gaya desain** | Soft pastel, clean, profesional, mobile-friendly, **tanpa emoji**, copy ringkas |
| **Pemilik** | Gurveender Jeet Kaur — SWE student, Universitas Gadjah Mada |
| **Bahasa situs** | **English** |
| **Kontak** | gurveenderjeetkaur@gmail.com · linkedin.com/in/gurveenderjeetkaur · github.com/kaurgurveend |

### Positioning (balance, tidak berat sebelah)
> Pemilik punya pengalaman kuat di **Project Management** (SRS/BISREQ, planning, koordinasi tim) dan sedang aktif sebagai **QA** (automation + manual testing). Portofolio menampilkan **dua sisi dengan bobot setara** — bukan QA-first, bukan PM-first. Recruiter QA melihat bukti testing; recruiter PM melihat dokumentasi & koordinasi.

---

## 2. Log Keputusan

| # | Keputusan |
|---|---|
| D1 | Bahasa situs: **English** |
| D2 | Positioning: **QA & PM seimbang** (tidak ada frasa "main focus") |
| D3 | Dental: peran **QA + PM**, dengan detail per peran |
| D4 | SIMATKUL: project **ongoing**, peran QA |
| D5 | Link Notion/Drive: **placeholder** (untuk SIMATKUL, PM drive Dental, AIS) |
| D6 | Project ditampilkan: 5 kartu (Dental, SIMATKUL, AIS, Veen Moda, Evently) |
| D7 | **Tidak ada** hero stats (17+ automated dst.) dan metrik box di kartu |
| D8 | **Tidak ada** section About dan Experience ("My journey so far") — sudah tercakup di CV |
| D9 | **Tidak ada emoji** di seluruh halaman; copy ringkas & natural (hindari pola teks khas AI) |
| D10 | Setiap kartu project **bisa diklik** → membuka detail modal berisi peran (as QA / as PM), pencapaian singkat, dan link (GitHub, bug report, Notion/Drive) |
| D11 | Tidak ada garis/timeline dekoratif |
| D12 | **Koreksi tools:** automation = **Playwright**, Jira, Notion. **Selenium, TestRail, dan Trello dihapus** (tidak dipakai). PM tools = Jira, Notion, MS Office/Excel |
| D13 | **Semua garis penghubung/pemisah dihapus** dari desain (nav, section, modal, dsb.) — hanya dibedakan lewat warna latar & shadow |

---

## 3. Struktur Halaman (single page)

1. **Nav** — nama, menu (Skills, Projects, Contact), tombol Download CV
2. **Hero** — nama besar di atas, role line, 1–2 kalimat ringkas, foto, CTA
3. **Skills** — dua panel sejajar: Quality Assurance & Project Management (tags)
4. **Projects** — 5 kartu + filter; klik kartu → **detail modal** (peran, link, tautan dokumentasi)
5. **Contact** — email, LinkedIn, GitHub, WhatsApp + form
6. **Footer**

---

## 4. Konten Project (final + detail modal)

### P1. Tentang Dental — E2E Automated Testing *(featured)*
- Badge: QA · Automation + PM | Status: PPPL Final Project, 2026
- Card: *"End-to-end automated testing of a dental clinic Android app with Cucumber BDD + Appium. 17 scenarios, 6 bugs found."*
- **Modal — as QA:** test case Login/Register/Profile (Page Object, step definitions, feature files); 17 skenario; 6 bug (1 critical: keamanan ganti password); bug report terstruktur.
- **Modal — as PM:** koordinasi tim 3 orang via branch; pembagian tugas & integrasi; dokumentasi PM di Drive (placeholder).
- **Links:** GitHub repo, bug_report.md, Drive PM (placeholder).

### P2. SIMATKUL — Course Management System *(ongoing)*
- Badge: QA · Functional Testing | Status: In Progress
- Card: *"QA for an active academic system that manages courses and assignments."*
- **Modal — as QA:** test case fungsional & UAT; tracking & pelaporan bug; dokumentasi di Notion/Drive.
- **Links:** Notion (placeholder), Drive (placeholder).

### P3. AIS — Academic Information System
- Badge: Project Management | Status: University project
- Card: *"Led planning and requirements for a university information system."*
- **Modal — as PM:** SRS & BISREQ; C4 + use case & activity diagram; requirement gathering & koordinasi stakeholder.
- **Links:** Docs (placeholder).

### P4. Veen Moda — Textile Stock Management
- Badge: PM · Full-Stack | Status: Shipped
- Card: *"Stock management system for a fabric store built with Laravel."*
- **Modal — as PM:** merencanakan build cycle & prioritas fitur. **as Dev:** implementasi Laravel (PHP, Blade, MySQL).
- **Links:** GitHub.

### P5. Evently — Virtual Event Organizer
- Badge: Full-Stack Development | Status: Shipped
- Card: *"Web app to create, manage, and join virtual events."*
- **Modal — as Dev:** event registration, ticketing, host management, participant feedback.
- **Links:** GitHub.

---

## 5. Aturan Copywriting (anti "AI vibes")

1. **Tanpa emoji** di teks visual.
2. **Tanpa statistik mencolok** (17+ skenario, jumlah bug) di hero/card — cukup disebut wajar dalam 1 kalimat di bagian teks project.
3. Kalimat **pendek & faktual**: apa yang dibuat, peran, hasil. Hindari frasa marketing kosong ("passion for...", "thrives at the intersection of...").
4. Tidak ada dekorasi garis/timeline.
5. Bahasa Inggris formal namun santai, natural.

---

## 6. Teknologi & Deploy

Mockup: HTML/CSS/JS statis. Final: vanilla HTML/CSS/JS atau Next.js; deploy GitHub Pages / Vercel (rekomendasi `gurveender.github.io`).

---

## 7. Aset yang Dibutuhkan (cocok dengan apa yang akan dikirim)

### Dokumen & bukti kerja — per project
| Project | Dokumen yang dibutuhkan | Status |
|---|---|---|
| **Dental (QA)** | Bug report & hasil test (link GitHub sudah ada) | ✅ Terpasang |
| **Dental (PM)** | Link Drive PM: https://drive.google.com/drive/folders/1EfZAvEr1rVuz1b4Zk1KzWG0Py_WpkP8r | ✅ Terpasang |
| **SIMATKUL (QA)** | Drive: https://drive.google.com/drive/folders/1XpW9iEZFjrbBQbZUiFbvhh-Swofxw0uE | ✅ Terpasang |
| **SIMATKUL (Notion)** | Test Plan: https://app.notion.com/p/Test-Plan-SIMATKUL-3d6d16b4122b8186a36bfba121ceab98 | ⚠️ Belum public (harus Share → Anyone with link) |
| **AIS (PM)** | Google Drive (SIA Mobile): https://drive.google.com/drive/folders/1e7DUeeaCI9b7JcUTW-FPrr254dWP5LPX (berisi SRS, Use Case, Timeline, UAT, MVP) | ✅ Terpasang |
| **Foto & CV** | File lokal: `design/assets/photo.jpeg` + `design/assets/CV_Gurveender_Jeet_Kaur.pdf` | ✅ Terpasang (hero + tombol Download CV) |
| **WhatsApp** | +62 812-6948-4827 (`wa.me/6281269484827`) | ✅ Terpasang |

### Umum
- [ ] **Notion**: aktifkan "Anyone with the link", copy ulang link dari menu Share (bukan tombol Copy dari app)
- [ ] Link Drive sudah "Anyone with the link" ✅ (terverifikasi terbuka)
- [ ] (Opsional) fork repo Dental ke akun `kaurgurveend`

> Format pengiriman bebas: ketik link di chat, atau screenshot + link. Aku akan tempel semua link ke kartu project & modal.

---

## 8. Acceptance Criteria

1. Konten English, ringkas, tanpa emoji.
2. 5 kartu project dengan detail modal yang berfungsi + tampil peran QA & PM.
3. Semua tautan berfungsi (kontak, GitHub, LinkedIn, CV, docs).
4. Responsive mobile.
5. Deploy di URL publik.

---

## 9. Roadmap

| Fase | Kegiatan | Output |
|---|---|---|
| 0 | PRD + mockup (v2 by feedback) | ✅ |
| 1 | Kirim link Notion/Drive asli + foto + CV | Konten 100% final |
| 2 | Development | Website fungsional |
| 3 | Deploy | Link live |
| 4 | Optimasi | Polishing |

---

## 10. Open Questions

1. Link Notion/Drive asli — kapan bisa dikirim?
2. Repo Dental dipindah/fork ke akun `kaurgurveend`?
3. Foto profesional tersedia?