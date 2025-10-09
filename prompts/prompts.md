# Prompts

## Prompt to create project instructions
What instructions would you give a claude code project to have it act as a staff level engineer assisting me on a project [description of project]?

^^^output is then pasted into claude as instructions to guide overall project 

## Follow up prompt once project instructions inserted
Following the project instructions, please lay out a migration plan for [website] Keep in mind, I am not particularly technical and will rely on claude code to help guide me through deployment of the migrated application.

### Restarting claude code session 
Review the last session in claude.md and the launch checklist. What's the most critical item for getting [project name] live? Think hard.

### Committing migration project 
Create a detailed session summary including:
- What we built/modified
- Why we made specific technical choices  
- Any issues encountered and solutions
- Updated launch checklist: What remains to deploy live at [website]
  - Blockers vs nice-to-haves
  - Estimated effort for remaining items
  - Priority order for next session
- Update claude.md with session summary
- Update README.md ONLY if there are significant changes to project structure, setup, or features
- Commit as "docs: [your summary]" and push

### Discovery
Explore my code base. I'd like to prepare this Astro site to replace the website that's currently being served on [website] (which is built on wordpress). What other considerations should I make before deploying this via Vercel? Beyond deploying via Vercel what other todo's do I have to have this site replace the current [website]? Don't make changes yet, just give me a comprehensive audit.

Current status of my Astro site is contained in the claude.md file. 