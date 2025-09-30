```mermaid
sequenceDiagram
	participant browser
	participant server

	note right of browser: the SPA is already loaded \nall notes are stored in browser memory.

	note right of browser: users view notes on page\nno request is sent.