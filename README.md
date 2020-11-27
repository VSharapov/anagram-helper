# anagram-helper
Bridge the gap between two near-anagrams

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
- [x] Make an interface like [https://connorholyday.github.io/anagram-helper/][1]...
    - [x] ...but without React...
    - [x] ...with both phrases represented...
    - [x] ...and dark mode
- [ ] Suggestions
    - [ ] Has all characters within phrase
    - [ ] Perfect bridge, e.g. Need `a` + `e` suggest `anagram` + `manager` or `bad` + `bed`
- [ ] Wordlists
    - [ ] Hint at near-matches from arbitrary wordlist
    - [ ] Look for easy wordlists - something grabbable through `xmlHttpRequest`
        - [ ] Something tiny for testing
    - [ ] Look for functional wordlists - UrbanDictionary, reddit minus the gibberish
    - [ ] Checkboxes to choose your wordlist(s)
- [ ] History - track changes, revert, branch

[1]: https://connorholyday.github.io/anagram-helper/
