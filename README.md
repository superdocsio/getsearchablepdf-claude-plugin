# GetSearchablePDF for Claude

GetSearchablePDF turns scanned PDFs and images (PNG, JPEG) into searchable PDFs,
so you can search, select and copy their text. A panel in the conversation shows
progress and then a **Download** button for each file, up to 10 at a time.

Only the pages without text go to OCR. Pages that already have text are left as
they are and cost nothing. If an old scan has a wrong text layer, ask Claude to
run OCR anyway to replace it.

This plugin connects Claude to the GetSearchablePDF service at
`https://mcp.getsearchablepdf.com/mcp` and adds a skill that guides Claude through
converting files. It works in Claude chat, Cowork and Claude Code.

## Try it

Ask, for example:

- "Make a PDF searchable."
- "OCR this scan so I can copy its text."
- "Turn this photo of a receipt into a searchable PDF."

Fictional sample files are at
[getsearchablepdf.com/assistants](https://getsearchablepdf.com/assistants#samples).

## Sign in and pages

The first time Claude uses GetSearchablePDF, it asks you to connect your
GetSearchablePDF account. Sign in, or create an account, and allow access.

Conversions use the same page balance as the website: each page that needs OCR
uses one page. Your plan sets the largest file you can convert. Ask Claude
"How many GetSearchablePDF pages do I have left?" to see your balance and limits.

Claude chooses the file in the panel's picker. To let Claude send an attached file
itself, allow `mcp.getsearchablepdf.com` under **Settings → Capabilities → Code
execution and file creation → Network access**.

## Your data

- Only the files you attach or choose are sent to GetSearchablePDF.
- Files and their searchable versions are deleted after 60 minutes.
- Your files are never used for training.

See the [privacy policy](https://getsearchablepdf.com/privacy) and
[terms of service](https://getsearchablepdf.com/terms).

## Install in Claude Code

```sh
claude plugin marketplace add superdocsio/getsearchablepdf-claude-plugin
claude plugin install getsearchablepdf@getsearchablepdf
```

## Support

Email [getsearchablepdf@gmail.com](mailto:getsearchablepdf@gmail.com), or see
[getsearchablepdf.com/assistants](https://getsearchablepdf.com/assistants).
GetSearchablePDF is made by Superdocs.
