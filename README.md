# Getting started

Read the directions after you play.

# Fenced code block
Here's an example:

```
function test() {
  console.log("notice the blank line before this function?");
}
```

# Syntax highlighting example

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

# Tables

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

For aesthetic purposes, you can also add extra pipes on the ends:

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

Note that the dashes at the top don't need to match the length of the header text exactly:

| Name | Description          |
| ------------- | ----------- |
| Help      | Display the help window.|
| Close     | Closes a window     |

You can also include inline Markdown such as links, bold, italics, or strikethrough:

| Name | Description          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |

Finally, by including colons within the header row, you can define text to be left-aligned, right-aligned, or center-aligned:

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

# Task lists

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> are supported
- [x] list syntax is required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

# Task lists can be nested to better structure your tasks:

- [ ] a bigger project
  - [ ] first subtask #1234
  - [ ] follow up subtask #4321
  - [ ] final subtask cc @mention
- [ ] a separate task

# References

However, Chrome doesn't seem to render it at this time but it rendered the original...
Certain references are auto-linked:

* SHA: ddd3e57edee8bad621fab67bb845247635cce445
* User@SHA: otherness-space@ddd3e57edee8bad621fab67bb845247635cce445
* User/Repository@SHA: otherness-space/sheetsee.ddd3e57edee8bad621fab67bb845247635cce445
* #Num: #26
* GH-Num: GH-26
* User#Num: otherness-space#26
* User/Repository#Num: otherness-space/sheetsee.js#26

# h1
## h2
### h3
#### h4
##### h5
###### h6

# Blockquotes

In the words of Abraham Lincoln:

> Pardon my french

# Unordered lists

* 1
* 2
* 3

- item
- item
- item

# Ordered Lists

1. Item 1
2. Item 2
3. Item 3

# Nested lists

1. Item 1
  1. A corollary to the above item.
  2. Yet another point to consider.
2. Item 2
  * A corollary that does not need to be ordered.
    * This is indented four spaces, because it's two spaces further than the item above.
    * You might want to consider making a new list.
3. Item 3

# Code formatting

## Inline formatting

Single back ticks

Here's an idea: why don't we take `SuperiorProject` and turn it into `ReasonableProject`.

## Multiple lines

Triple back ticks

Check out this neat program I wrote:

```
x = 0
x = 2 + 2
what is x
```

# Links

[Visit Github](http:github.com)

* * *
- - -
***
*****
