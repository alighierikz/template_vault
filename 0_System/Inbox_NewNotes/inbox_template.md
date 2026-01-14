<%* let filetype = await tp.system.suggester(["ToDo", "shoppinglist", "your_Choice", "rootnote"], ["ToDo", "shoppinglist", "your_Choice", "rootnote"], false, "Which template do you want to use?") _%>
<%-* if (filetype === "ToDo") { _%> 
<% tp.file.include("[[todo_template]]") %> 
<%_* } else if (filetype === "shoppinglist") { _%>
<% tp.file.include("[[shoppinglist_template]]") %>
<%_*} else if (filetype === "your_Choice") { _%>
<% tp.file.include("[[your_Choice_template]]") %>
<%-* } else if (filetype === "rootnote") { _%>
<% tp.file.include("[[rootenote-template]]") %>
<%-* } else { _%>
<% tp.file.cursor(1) %>
<%* } -%>

