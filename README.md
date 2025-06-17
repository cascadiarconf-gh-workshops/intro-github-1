# Intro GitHub for R Users 2025 - Test Fundamental Skills with 'GutHub'

> **Notes:**  
> ⚠️ This workshop is a work-in-progress and is subject to frequent change.\
> 🎓 This workshop reinforces self-paced learning from a curated [GitHub Basics](./github-basics.md) self-paced learning track and prepares you for the intermediate github workshop.  
> 🛑 Follow best practices and GitHub Flow while completing the tasks.  
> 📚 Refer to [GitHub Docs]([https://docs.github.com/](https://docs.github.com/en/get-started)), use our workshop Slack channels, or discuss with your peers for guidance.

## **Workshop Scenario**

You and your team are contributing to a collaborative Cascadia R Conference cookbook called [**GutHub**](https://github.com/cascadiarconf-gh-workshops/GutHub), where everyone shares their favorite recipes using [Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github) in a GitHub repository. Your goal is to **submit a Markdown-formatted recipe**, [review contributions](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews) from others, and navigate through the [GitHub Flow](needs.link.here) to merge your changes.

To complete your task, you will:
- Create a new branch and add your recipe in [Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
- Submit a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) (PR) for review.
- [Review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews) another participant’s pull request.
- Resolve any [merge conflicts](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github) that arise.
- Successfully [merge](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request) your recipe into the main cookbook.

You anticipate the following challenges:
- Formatting your recipe correctly in GitHub Markdown.
- Understanding the GitHub Flow for contributions.
- Resolving conflicts if multiple people modify the same file.

🎯 Precision is important in cooking and using GitHub! Follow the workflow task directions very carefully and use your GitHub skills to **collaborate, review, and merge recipes efficiently!**

**Good luck!**

## **Workshop Tasks**

### **Task 0. Setup**
1. Navigate to the [**GutHub**](https://github.com/cascadiarconf-gh-workshops/GutHub) repository on GitHub. We recommend keeping these instructions and the GutHub repo open in separate tabs.
2. **Create a new branch** for your contribution. Name it `yourinitials-recipe`.
  - Example: `ynh-brazilian-beans`
3. **Ensure you are not working on `main` directly!** All changes should be in a separate branch.

---

### **Task 1. Create Your Recipe in Markdown**
1. With your branch active, Navigate to the `recipes/` folder in the repository.
2. Click the `Add file` button and name the file with your initials, the name of your dish, followed by the `.md` file extension e.g. `ynh-brazilian-beans.md`
  > ⚠️ A lot of people forget to add the `.md` part here!
3. Copy the template found in the cookbook here: [GutHub Template Recipe ](needs.link.here)
4. Format your recipe using Markdown:
  ```md
  ---
  title: Brazilian Beans
  author: Yourna Mehere
  date: "2025-04-28"
  categories: [side dish, dip, black beans]
  description: "A simple, tasty recipe for black beans"
  image: "./images/ynh-brazilian-beans.jpg" or leave empty quotes for now like ""
  ---

  <p align="center">
    <img src="./images/ynh-brazilian-beans.jpg" alt="Brazilian Beans" width="300"/>
  </p>
  
  # Brazilian Beans and Rice
  
  ## Ingredients
  - 1 cup black beans
  - 2 cups cooked rice
  - 1 onion, diced
  - 2 cloves garlic, minced
  - 1 tsp cumin
  - Salt and pepper to taste
  
  ## Instructions
  1. Soak the black beans overnight or use canned beans.
  2. Sauté onions and garlic in a pan.
  3. Add beans, cumin, salt, and pepper; simmer for 15 minutes.
  4. Serve over rice and enjoy!
  ```
5. **Commit your changes** to your branch.

---

### **Task 2. [Optional] Add an image for your recipe**

#### Option 1: Upload an image
This process will be very similar to the process above, but instead of `Add file` → `Create new file`, you'll `Add file` → `Upload file` to upload an image
- `Add file` → `Upload file` and upload an image file (.jpg or .png) to the `recipes/images/` folder with the same name as your recipe i.e. `ynh-brazilian-beans.jpg`
- Modify the `image: "./images/ynh-brazilian-beans.jpg"` and `img src="./images/ynh-brazilian-beans.jpg"` in the template with the filename of your uploaded image

#### Option 2: Use an image from the web
If you'd rather go a simpler route, just use an image URL from somewhere else on the internet. Just note that this image might disappear in the future!
- Copy the web URL of the image you want
- replace the image path in the YAML (between the two `---` lines) of your recipe `image: "./images/ynh-brazilian-beans.jpg"` with `image: your-url-goes-here.com`
- replace the path and alt text in the `<img src="./images/ynh-brazilian-beans.jpg" alt="Brazilian Beans" width="300"/>` with your image URL and alt text describing the image.
---

### **Task 3. Open a Pull Request (PR)**
1. Navigate to the **GutHub repository** on GitHub.
2. Click **New Pull Request** and select your branch (`yourname-recipe`) as the source.
3. **Title your PR**: `Added Brazilian Beans Recipe` (or your dish name).
4. In the description, briefly explain your contribution and what the filenames of your recipe (and image if including one) are so your reviewer can find them.
5. Finish opening the PR and ask for someone to review your work by [assigning a reviewer](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews).

---

### **Task 4. Review a Peer’s Recipe**
1. Review **at least one other PR** from a teammate.
2. Leave **constructive feedback** in comments if you notice anything wrong or not working quite right.
3. Suggest improvements if necessary (e.g., formatting, filenames, missing steps).

> 📣 Reviewers can use this checklist to help identify potential problems with recipes under review:
> - [ ] Did they name their recipe with `.md` extension in the file name?
> - [ ] Is the name the expected format e.g. `initials-recipe-name.md`?
> - [ ] Does the recipe appear to use the [GutHub Template Recipe ](https://effective-adventure-z2o86yg.pages.github.io/template-recipe.html)?
> - [ ] Did they update the YAML frontmatter in their recipe file? i.e. `title:`, `author:`, `categories:`, image etc.
> - [ ] Did they include an image in their recipe and can you find that image in the `/recipes/images` folder?
> - [ ] Does the image have a `.jpg` or `.png` extension?
> - [ ] When you go to their branch in the `code` tab and open their recipe markdown file, can you preview it? Does it look ok?
> - [ ] If everything looks ok, review the PR and 'Approve'
> - [ ] If something needs fixing, communicate with your reviewee or ask for assistance

And finally,

4. Approve the PR when your reviewee has finished adjusting to their recipe submission.

---

### **Task 5. Resolve a Merge Conflict (if applicable)**
1. If multiple people edit the same file (e.g., `README.md`), GitHub may show a **merge conflict**.
2. Click **Resolve Conflicts** in the PR.
3. Edit the file to manually merge both contributions.
4. Once resolved, commit the changes and complete the merge.

---

### **Task 6. Merge Your Recipe into Main**
- Once your PR is approved and conflicts are resolved:
  - Click **Merge Pull Request**.
  - Delete your branch after merging.

🎉 **Congratulations! You’ve successfully contributed to GutHub!** 🎉

Your contributions will take a few minutes to appear in the cookbook. Check back soon to:
- Validate your submission rendered properly. Do you see any issues? How might you fix them?
- If you need to fix something, start the GitHub flow again: create a branch, make your changes, open a PR, ask for a review, merge
- Help others if you are all done!

## Key Takeaways
This wasn’t just a fun workshop — you just built something powerful, reusable, and real.

- ✅ You created a version-controlled knowledge product using just Markdown and GitHub Flow — no coding required.
- 🤝 You practiced collaborative contribution and peer review, just like real development teams.
- 🧱 You saw how templates, structure, and automation can scale team knowledge, not just code.
- ⚙️ Behind the scenes, you used tools that power real-world systems:
  - YAML frontmatter to organize metadata in your submissions
  - GitHub Actions automates the cookbook publishing with your contributions
  - Static site generation (Quarto and GitHub Pages) make it all visible

This exact pattern can power team playbooks, data portfolios, documentation hubs, and more. Here are some examples:
- [PCH Informatics Hub (private, not accesisble outside demo)](https://cuddly-adventure-n862rpv.pages.github.io/)
- [RHINO R Package (private, not accessible outside demo)](https://refactored-potato-b0d33d79.pages.github.io/)
- [GeoHUB Playbook for Developers (private, not accessible outside demo)](https://github.com/DOH-EPI-Coders/geohub-playbook)
- [A Personal Solutions Library](https://doh-sre1303.github.io/Help-articles/)

### What's next?
🧠 You now have the foundation to build shared resources and collaborate with clarity. [Placeholder for Intermediate GitHub Workshop]

<!-- In [Workshop 2: Migrating Existing Projects to GitHub](https://github.com/DOH-EPI-Coders/github-basics-workshop-2), you’ll take real (but safe) files from a simulated network drive project and learn how to:
- Reorganize and clean up messy project folders with intuitive structures 💾
- Identify and protect sensitive data before committing it to GitHub 🔐
- Create clean, portable, and team-ready GitHub repositories 🗂️
- Use .gitignore, branches, and issues to manage code history and collaboration 🧰

⚙️ Workshop 2 is less about learning GitHub — and more about learning how to modernize, document, and protect the work your team already does every day. You’ll practice responsible migration, improve file hygiene, and get one step closer to mastering collaborative work with code and data.
-->
