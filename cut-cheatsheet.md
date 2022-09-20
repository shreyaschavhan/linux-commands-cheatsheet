## 𝐂𝐮𝐭 𝐂𝐡𝐞𝐚𝐭𝐬𝐡𝐞𝐞𝐭

Command | Explanation
:-:|---
`cut -c 3` | display `3rd character` from each line of text
`cut -c 2,7` | display the `2nd and 7th character` from each line of text
`cut -c 2-7` | display a range of characters starting at the `2nd position` of a string and ending at the `7th position`(both positions included)
`cut -c -4` | display the `first four` characters from each line of text
`cut -d $'\t' -f -3` | display `first three` fields of a `tab delimited` file
`cut -c 13-` | display the characters from `13th` position to the `end`
`cut -d ' ' -f 4` | display `4th word` with space `' '` as a delimiter
`cut -d ' ' -f -3` | display `first three words` with space `' '` used as a delimiter
`cut -d $'\t' -f 2-` | given a `tab` delimited file, display the fields from `second fields to last field`

 
