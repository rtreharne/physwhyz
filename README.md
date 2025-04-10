# physwhyz# 🛠 A-Level Physics Platform — 12-Week Build Plan (Pure Django)

**Goal:** Launch a functional MVP in 12 weeks, working ~4 hours/week

---

## ✅ Phase 1: Core System (Weeks 1–4)

### Week 1: Project Setup + Models
- [ ] Set up Django project and `papers` app
- [ ] Create models: `Paper`, `Page`, `MarkScheme`
- [ ] Configure media/static file handling
- [ ] Register models in Django admin

---

### Week 2: PDF Upload + Page Image Conversion
- [ ] Add file upload form (via admin or custom view)
- [ ] Use `pdf2image` to convert PDF pages to images
- [ ] Save each image as a `Page` linked to the `Paper`

---

### Week 3: Text Extraction
- [ ] Use `PyMuPDF` (fitz) to extract text from each page
- [ ] Store extracted text in `Page.text`
- [ ] Show image and text together in the page template

---

### Week 4: Basic Page Viewer
- [ ] Create a page viewer template to display:
  - [ ] Page image
  - [ ] Page number
  - [ ] Extracted text
- [ ] Add next/previous page navigation

---

## ✅ Phase 2: Tagging & Mark Scheme Linking (Weeks 5–8)

### Week 5: Add Topic Tags
- [ ] Create `Tag` model
- [ ] Add many-to-many field to `Page`
- [ ] Update admin to assign tags to pages
- [ ] Display tags in the page viewer template

---

### Week 6: Mark Scheme Upload + Linking
- [ ] Enable Mark Scheme upload via admin
- [ ] Convert mark scheme PDF to images
- [ ] Link question `Page` to corresponding mark scheme page

---

### Week 7: Side-by-Side Viewer
- [ ] Update frontend to display:
  - [ ] Question image
  - [ ] Linked mark scheme image (if exists)
- [ ] Add toggle button to show/hide mark scheme

---

### Week 8: Search + Tag Filtering
- [ ] Add keyword search (using `icontains` on `Page.text`)
- [ ] Add topic filter (filter by tag)
- [ ] Show matching results in the viewer
- [ ] (Optional) Highlight matching search terms

---

## ✅ Phase 3: Custom Sets + Launch (Weeks 9–12)

### Week 9: Bookmarking Pages
- [ ] Add “Bookmark this page” button to viewer
- [ ] Save bookmarked pages in Django session
- [ ] Create “My Set” page to list bookmarked pages

---

### Week 10: Export Set (PDF or Print)
- [ ] Create a printable version of bookmarked pages
- [ ] Add “Print” or “Download PDF” button
- [ ] (Optional) Use `WeasyPrint` for PDF generation

---

### Week 11: UI Polish + Navigation
- [ ] Add top navigation bar (Home, Papers, My Set)
- [ ] Improve spacing, fonts, and mobile layout
- [ ] Add favicon, page titles, and meta tags

---

### Week 12: Deploy MVP
- [ ] Set up deployment (Render/Railway/DigitalOcean)
- [ ] Configure static/media file handling in production
- [ ] Register domain + set up SSL (optional)
- [ ] Test on phone/tablet/desktop
- [ ] Share with beta testers (students/tutors)

---

## 🎯 MVP Deliverables by Week 12

- [ ] Upload papers and mark schemes
- [ ] View questions with text + tags
- [ ] Search + filter by topic
- [ ] Link to mark scheme answers
- [ ] Build and export custom question sets
- [ ] Fully deployed, usable web app

---

**Keep the sprints small. Stay consistent. MVP in 12 weeks. Let's go! 🚀**
