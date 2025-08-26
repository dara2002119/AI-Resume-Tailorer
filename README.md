# AI Resume Tailor  

**AI Resume Tailor** is a Python tool that takes a **Markdown-formatted resume** and a **job description**, uses GPT to tailor the content with role-specific keywords and measurable results, and exports a **polished one-page Word resume** with custom formatting.  

✨ Designed for ATS-friendliness and recruiter readability.  

---

## Features  

- 🔹 **AI-powered tailoring**: Aligns your resume with a job description using GPT.  
- 🔹 **Markdown input**: Keep your resume clean, portable, and version-controlled.  
- 🔹 **One-page guarantee**: Optimized spacing and formatting to fit within a single page.  
- 🔹 **Custom Word output**:  
  - Name in **blue, centered, 14pt**  
  - Contact line **centered, 11pt** under name  
  - Body text in **Times New Roman, 11pt**  
  - Compact bullets and section headers for maximum content density  
- 🔹 **ATS-friendly**: No tables, images, or tricky layouts.  

---

## How It Works  

1. **Input**:  
   - A Markdown resume (`resume.md`)  
   - A job description (plain text)  

2. **Processing**:  
   - Cleans up Markdown (spacing, bullets, headings)  
   - Passes resume + JD into GPT with a tailored prompt (limits word count, bullets, and roles)  
   - Ensures all sections (Education, Skills, Experience, Projects) are preserved  

3. **Export**:  
   - Uses `pypandoc` + `python-docx` to apply a custom Word template  
   - Formats name and contact info centered at the top  
   - Outputs a **one-page `.docx` file** ready to submit  

---
