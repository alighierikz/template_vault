<%* let filetype = await tp.system.suggester(["Book Note", "Watering", "Project Note", "rootnote"], ["Book Note", "Watering", "Project Note", "rootnote"], false, "Which template do you want to use?") _%>
<%-* if (filetype === "Book Note") { _%> 
<% tp.file.include("[[Book Note Template]]") %> <% tp.file.move("/030 Media/031 Books/" + tp.file.title) %>
<%_* } else if (filetype === "Watering") { _%>
<% tp.file.include("[[general_template_watering]]") %>
<%_*} else if (filetype === "Project Note") { _%>
<% tp.file.include("[[Project Note Template]]") %>
<%-* } else if (filetype === "Rootnote") { _%>
<% tp.file.include("[[rootnote-template]]") %>
<%-* } else { _%>
<% tp.file.cursor(1) %>
<%* } -%>

