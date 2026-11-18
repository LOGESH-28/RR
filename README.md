# Pressure Lab (static site)

Plain HTML, no build step, no dependencies, no external requests.

Files
- index.html: the dashboard (all data is embedded)
- Pressure_Players_Methodology.pdf: full methodology report, linked from the page
- vercel.json: optional settings (clean URLs, basic headers)

Deploy on Vercel (CLI)
1. Install Node.js, then run: npm i -g vercel
2. cd pressure-lab
3. vercel          (log in, then answer the prompts: no framework, no build command, output directory ".")
4. vercel --prod   (prints the public production URL)

Deploy on Vercel (GitHub)
1. Create a GitHub repository and upload these files so that index.html is at the repository root.
2. In Vercel: Add New > Project > import the repository.
3. Framework Preset: Other. Build Command: leave empty. Output Directory: leave empty. Deploy.

Common problem: the HTML file must be named index.html and sit at the project root, or Vercel shows a 404.
