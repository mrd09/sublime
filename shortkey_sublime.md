Short key

Open file under cursor by double click: install plugin:
- [Install ref](https://gist.github.com/Suor/1344471)
- Key Binding: Subl 3: keep open_file_at_cursor -> Save
- Place cursor at file path then double click 

Search in all files in a project+folder+... in Sublime Text 3:
- Press "Ctrl + Shift +f"
	+ Find: "key word". Ex: elasticsearch:
	+ Where: "Path want to search or project...". Ex: ~/knowledge/qa_eq
- Trick in Find: <project>,<current file>,<open files>,<open folders>,-*.yml,-*.md
- Result file:
```
Searching 83 files for "elasticsearch:" (regex)

/home/mrd09/knowledge/qa_eq/group_vars/qa_eq:
  560    content_packs_backup_dir: /var/backups/contentpacks
  561  
  562: elasticsearch:
  563    host: "{{ groups['elasticsearch'][0] }}"
  564    port_http: 9200

1 match in 1 file
```

Place cursor
  1. Place cursor at beginning and at the end of the range of text
	Place cursor at the beginning of the text selected in your mind
	"Press ctrl + left-click" at "the end of the line"
	=> will select the text with 2 cursor at the beginning and the end of text

  2.1. Place cursor at end/beginning of multiple lines:	(method 1)
	Select all line want to place cursor
	Press "ctrl + shift + l" : Place multiple cursor at the end of each line
	  => If want to place at the beginning Press Home
  2.2. Place cursor at end/beginning of multiple lines:(method 2)
  	Press "shift + Right-click" then let go when text select desired

Code Folding
	Ctrl + Shift + [: Fold (Minimize)
	Ctrl + Shift + ]: Unfold

Moving, Jump

	Ctrl + P: jump to any file(header, title)

	Ctrl + G: jump to line

	Ctrl + F: search

	Crrl + Shift + T: ReOpen the recently close file

	Ctrl + PageUp/PageDown: switch between files

	F12: Jump to definition

	Alt + - : Jumpback where last cursor is

	Shift + Alt + - : Switch backward before use "Alt + -"

	Ctrl + Home: Jump to beginning of file

	Ctrl + End: Jump to end of file

	Ctrl + M: Jump to Matching Bracket

Selection

	Shift + Right mouse: Column/Vertical selection

	Ctrl + D: Bôi đen từ hiện tại

Capitialization

	Ctrl + K then Ctrl + U right away: Upper case the selection word

	Ctrl + K then Ctrl + L right away: Lower case the selection

Delete Word

	Ctrl + K then Ctrl + K right away: delete to the end of line

	Ctrl + K then Ctrl + Backscape right away: delete to the beginning of line

	Ctrl + Backscape: delete one word backward

	Ctrl + Delete: delete one word forward

Line
	Ctrl + ] :Unindent(thụt tab dòng)

	Ctrl + [: indent(xóa thụt tab dòng)

	Ctrl + Enter: Thêm một dòng trống bên dưới (cursor cần ở đầu dòng)

	Shift + Enter: Thêm một dòng trống bên trên (cursor cần ở đầu dòng)

Build and Run code
	Ctrl + Shift + B: First time running: Build with: ..
	Ctrl + B: Build

