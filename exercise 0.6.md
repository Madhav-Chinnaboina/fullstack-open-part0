```mermaid
	sequenceDiagram
	participant browser
	participant server

	Note right to browser: SPA already loaded\nnotes stored in browser memory

	browser->>server:POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
	activate server
	server-->>browser:[{"message":"note created"}]
	deactivate server

	Note right of browser:browser update page dynamically\n New notes created without page reload