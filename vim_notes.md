# Change Modes
Change from INSERT to NORMAL ```⎋``` ```<esc>``` 
Chage from NORMAL to COMMAND ```:```

---

# Command Mode

## Quit ```:q```

## Write & quit ```:wq```

## Replace 
```:%s/<word_to_replace>/<replace_with_this>```

Example: replace "Hello" with "Hi" and ask for confirmation
```:%s/Hello/Hi/c```

## Go to line ```:<line_number>l```

Example: go to line 7
```:7l```

---

# Normal Mode

### Insert at beginning of line ```I```
If indented, the cursor will move before the first character after the indent.

## Insert at end of line ```A```

## Insert right of cursor ```a```

## Insert left of cursor ```i```

## Go to end of line ```$```

## Go to beginning of line 
Will go to the beginning even if indented ```0```
Will go to the first character after indentation ```^```

## Go to beginning/end of word
Beginning moving left ```b```
Beginning moving right ```w```
End moving right ```e```
For WORDS instead of words use capital letters
(WORDS are only separated by whitespace, while additional characters separate words)

## Go to the first non blank character on the next line ```+```

## Go to the first non blank character on the previous line ```-```

## Delete current word and enter insert mode ```ciw```

## Delete from cursor to beginning of word and enter insert mode ```cb```

## Delete current line ```dd```
acts like cut (the line is copied)

## Go to the last line ```G```

## Go to the first line ```gg```

## Search
```/``` then search term
After ```enter``` use ```n``` to move to next result

## Insert line above/below
The cursor will move to the new line in ```INSERT``` mode
Above ```O```
Below ```o```

## Copy/yank entire line ```yy```

## Paste ```p```

## Alternative for ```:wq```: ```ZZ```

## Search for the word that the cursor is on ```*```
Go to the previous occurence ```N```
Go to the next occurence ```n```

Replace example:
1. ```*``` to find all the words
2. ```ciw``` to delete the word
3. Type a new word in
4. ```⎋```
5. ```n``` or ```N``` to go other search results
6. ```.``` for each result to change the word

## Replace a character ```r```

---

# Visual Mode

## Select with direction keys ```v``` 
direction and beginning and end of line keys can be used

## Select word then copy ```viw``` ```y```

# Visual Block Mode

## Comment
Example: (using '#' as the comment)
1. ```<ctrl-v>``` to enter visual block mode
2. ```I``` (shift + i) to insert at the beginning of the line
3. ```# ``` comment symbol and a space
4. ```Esc```

## Uncomment
Example: (using '#' as the comment)
1. ```<ctrl-v>``` to enter visual block mode
2. ```l``` to expand the selection to 2 columns
           (to remove the comment symbol and space)
3. ```x``` to delete the selection
