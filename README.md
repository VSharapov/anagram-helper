# anagram-helper
Bridge the gap between two near-anagrams

## Demo
[https://vsharapov.github.io/anagram-helper/](https://vsharapov.github.io/anagram-helper/)

## The idea
I have two phrases that are _not_ anagrams but I want them to be.

My current method is to "cancel out" letters in a text editor, e.g:

```
                    Phrase 1: eternal September
Phrase 1 but not in Phrase 2: naleembe

Phrase 2 but not in Phrase 1: ddio
                    Phrase 2: reddit repost
```
Now I need words that "cancel out" the leftovers.

For example adding "did" to the top would leave only 'o' bringing the phrases closer to being anagrams.

Ideally a wordlist would get reordered with consideration to:

- Letters needed
- Word commonness
- Thematic fit

Picking new words one by one you can eventually get to an anagram:
```
eternal september did come
reddit became le repost-men
```

# TODO:
- Interface
    - [ ] Auto-resize text to fit width
        - [X] On text change
        - [ ] On window size change
    - [ ] Advanced settings menu
        - [ ] Custom ignore list vs. `[^0-9a-z]`
        - [ ] Hide matching letters
        - [ ] History - track changes, revert, branch
- [ ] Suggestions
    - [ ] Has all characters within phrase
    - [ ] Perfect bridge, e.g. Need `a` + `e` suggest `anagram` + `manager` or `bad` + `bed`
- [ ] Wordlists
    - [ ] Hint at near-matches from arbitrary wordlist
    - [ ] Look for easy wordlists - something grabbable through `xmlHttpRequest`
        - [ ] Something tiny for testing
    - [ ] Look for functional wordlists - UrbanDictionary, reddit minus the gibberish
    - [ ] Checkboxes to choose your wordlist(s)

[1]: https://connorholyday.github.io/anagram-helper/
