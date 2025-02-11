# Using Cline and Sonnet Efficiently

## Steps to Structure Your Workflow

1. **Define a Clear Goal**  
   - Ensure you have a well-defined objective and update project-goals.md.

2. **Create a Plan**  
   - **Prompt AI** to generate a structured plan and save it in your `cline_docs` folder.
   - ```
     Read the documents in the 'cline_docs/' directory, paying special attention to project-goals.md. Create a detailed and structured project plan that includes timeline, milestones, resources needed, key deliverables, risk assessments, and success metrics. Save this comprehensive plan as project-plan.md in the cline_docs directory. Use Markdown formatting with clear section headers, bullet points, and task hierarchies for optimal readability.
     ```

3. **Break Down the Goal into Subtasks**  
   - **Prompt AI** to break the goal into incremental subtasks.  
   - Add them as a list in your plan, marking each as **TODO**, **DOING**, or **DONE**.
   - ```
     Review the documents in the cline_docs directory. Break the plan into tasks, each task being marked as TODO, DOING, DONE as its being completed. It should be lists added to the plan.md
     ```

4. **List and Validate Assumptions**  
   - **Prompt AI** to generate a list of assumptions that need validation before implementation.  
   - Add them as tasks (**TODO**, etc.) in your plan.  
   - Validate assumptions before proceeding.
   - ```
     Review the documents in the cline_docs directory. Generate a list of assumptions that need validation before we can begin implementation. Add them as tasks (TODO) in the plan.
     ```

5. **Write the Code**  
   - **Prompt AI** to generate the initial code.  
   - Once functional, commit it to a feature branch.
   - ```
     Review the documents in the cline_docs directory. We're going to work on the TODO list and complete any items in the TODO status and the DOING status. The do not have to be completed in order, but we should follow an order that makes sense. All actions should consider that you may fail at any time, we we need to maintain a status as we go along in the task list. You should update an item that you're working on as DOING as the first action and save the file. If there are tasks that I must complete outside of coding tasks, you should prompt for me to do them and then confirm I have finished them before continuing. Your final task should be marking something as DONE when it is complete. This is all in Task Tracking section of the plan.md. Do not try to complete too much at one time because it will overwhelm you.
     ```

6. **Check Complexity**  
   - **Prompt AI** to analyze cyclic complexity to ensure the code remains modular and maintainable.

7. **Write Tests**  
   - **Prompt AI** to generate tests with parameters starting at zero, then one, and so on.

8. **Troubleshoot Hard Problems**  
   - If encountering difficulties:  
     1. **Prompt AI** to generate an **architecture document**.  
     2. **Prompt AI** to list five possible reasons the implementation may not be working, based on concerns about the approach.

9. **Manage Context Limitations**  
   - If you run out of context, start a new Cline task.  
   - Begin by **prompting AI** to read your updated documentation before continuing.
