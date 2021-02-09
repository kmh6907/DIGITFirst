The Blithedale Romance Steps
1. First I looked for `&`
2. Then I looked for `&amp`
3. Find `.+`
4. Replace with: `<xml>\0</xml>`
5. Find: `\n{3,}`
6. Replace with: `\n\n`
7. Find: `^ +` to get rid of spaces in front of Roman Numerals.
8. Find: `^(.+?)(\n\n)`
9. Replace with: `<p>\1</p>\2`
10. Find: `<p>([A-Z]+\..+?)</p>`
11. Replace with: `</chapter>\n\n<chapter><title>\1</title>`
11.  