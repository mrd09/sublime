# Short key
**MarkdownEditing to use MarkDown shortkey**
- Install package [MarkdownEditing](https://github.com/SublimeText-Markdown/MarkdownEditing#key-bindings)
- If head with error: Error loading syntax file "Packages/Markdown/Markdown.sublime-syntax": Unable to read Packages/Markdown/Markdown.sublime-syntax
	=> just remove the "Markdown" in "ignored_packages"
- Useful shortkey:
	+ Ctrl + r: quick navigation for all headers.
	+ Ctrl + Shift + PageUp/PageDown: Navigating to header
	+ Shift + Tab 	: Fold/Unfold current section.
	+ Alt + B: Bold
	+ Alt + I: Italic
	+ Select text + Press backtick/Asterisks/underscores/~ : auto wrap with backtick..
	+ Tips to use both Bold and Italic: `**_test_**`
	+ List: Enter at the end of line will trigger auto list order: `* - +`: Use Tab or Shift + Tab: Indent/Unindent
	+ Link: Can jump between bracket: `Ctrl + M`
- Sample config for MarkDown: Preferences/Package Settings/Markdown Editing/Markdown * Settings - User
```
{
	"color_scheme": "Packages/Color Scheme - Default/Mariana.sublime-color-scheme",
	"font_size": 8,
	"ignored_packages":
	[
		"Vintage"
	],
	"theme": "Adaptive.sublime-theme",
	"draw_centered": false,
	"line_numbers": true,
	"gutter": true,
    "margin": 10,
    "word_wrap": "auto",
    "wrap_width": 0,
}
```

**Group multiple folder**
- Step1: Open first folder: File/Open Folder 
- Step2: Add new group: View/Layout/Columns: 2 (Short key: Alt+Shift+2)
- Step3: Minimize the First folder in first side bar
- Step4: Switch to group 2: "Ctrl+2" (Switch back to group 1: Ctrl+1)
- Step5: Open second folder: File/Open Folder -> drag the folder to sidebar

**File Advance Operation**
- Press "Ctrt + Shift +P": Install Plugin: [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements)
- Key Binding/User/ : Set hot key for desired operation:
```
[
	{ "keys": ["ctrl+alt+c"], "command": "side_bar_copy_name" },
	{ "keys": ["alt+p"], "command": "side_bar_copy_path" }
]
```

**Comment short key**
- Press "Ctrl + /" to comment code

**Search for odd/even line**
```
1. Find: Ctrl+F
2. If regular expressions are not already enabled, enable them: Alt+R
3. Type in the expression .*\n.*\n
4. Find all: Alt+Enter
5. Press left arrow to get rid of the selections, leaving just the cursors: ←
6. You now have a cursor at the start of every odd-numbered line. If you wanted even-numbered lines, press down: ↓
```

**Search in all files in a project+folder+... in Sublime Text 3**:
- Press "Ctrl + Shift +f"
	+ Find: "key word". Ex: elasticsearch:
	+ Where: "Path want to search or project...". Ex: ~/knowledge/qa_eq
- Trick in Find: ```<project>,<current file>,<open files>,<open folders>,-*.yml,-*.md```
- Double Click for jump to file
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

**Place cursor**
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

**Code Folding**
	Ctrl + Shift + [: Fold (Minimize)
	Ctrl + Shift + ]: Unfold

**Moving, Jump**

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


