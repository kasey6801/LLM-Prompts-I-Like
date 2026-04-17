Create and refine a new prompt for the LLM Prompts I Like collection.

The user has provided a topic or focus area: $ARGUMENTS

Follow these steps exactly:

1. Draft a high-quality prompt based on the topic/focus area provided. Present it clearly to the user.

2. Ask the user: "Would you like to refine this, or does it look good to save?"

3. Iterate on the prompt with the user until they approve it. Common refinements include: adjusting tone, adding constraints, specifying output format, adding context, or narrowing scope.

4. Once the user approves the final prompt, collect the remaining fields one at a time:
   - **Title**: Suggest one based on the topic; ask the user to confirm or change it
   - **Version**: This is a new prompt, so suggest `1.0`. Ask the user to confirm.
   - **Intended Use**: What is this prompt designed to accomplish? (one sentence — suggest one based on the topic)
   - **Tool Used**: What tool or model was used to help generate or refine this prompt? (e.g., Claude Sonnet 4.6, manual, etc.)
   - **Tags**: 1–3 descriptive tags (comma-separated)

5. The **Original Prompt** is the user's initial request ($ARGUMENTS), and the **Modified Prompt** is the final approved version.

6. Present a preview of the complete file and ask the user to confirm before saving.

7. Once confirmed, write the file to `/Users/kcharles/ClaudeDev/CC_LLM_Prompts_I_Like/` using this format:
   - Filename: `YYYY-MM-DD_short-slug_v<version>.md` (use today's date, derive slug from title)
   - Content:
     ```
     ---
     title: "<title>"
     version: "<version>"
     date: YYYY-MM-DD
     tags: [tag1, tag2]
     ---

     ## Intended Use
     <intended use>

     ## Original Prompt
     <original prompt>

     ## Tool Used
     <tool used>

     ## Modified Prompt
     <modified prompt>
     ```

8. After writing the file, run:
   ```bash
   cd /Users/kcharles/ClaudeDev/CC_LLM_Prompts_I_Like && git add <filename> && git commit -m "Add: <title> v<version>" && git push
   ```

9. Confirm to the user that the prompt was saved and pushed to GitHub.
