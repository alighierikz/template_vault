---
tags:
  - "#todo"
created: <% tp.file.creation_date() %>
---
<% await tp.file.rename("ToDo "  + tp.date.now("YYYY-MM-DD-dddd") + tp.date.now(" HH-mm-ss")) %>

- [ ]  #todo

## <mark style="background: #FF5582A6;">due today</mark>
```tasks
hide backlink
hide id
hide created date
hide due date
hide scheduled date
due today
# not done

```

## <mark style="background: #FFB86CA6;">due tomorrow</mark>
```tasks
hide backlink
hide id
hide created date
hide due date
hide scheduled date
due tomorrow
# not done
```