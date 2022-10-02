
  # Regex_Tutorial
  
  ### Pinar Aktas
  https://github.com/PinarAktas/Regex_Tutorial

  [![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)


  ## Project Description
  Regular expressions, or regex for short, are a series of special characters that define a search pattern. Regular expressions can feel like their own language at times, but in fact they are universal and can be used within all programming languages. Let's break down the preceding “Matching a Username” regex in order to explore regex components in general.

  A regex is considered a literal, so the pattern must be wrapped in slash characters (/). If we examine the “Matching a Username” regex, you'll see that this is true:

    /^[a-z0-9_-]{3,16}$/

  Now let's take a look at the components of a regex about email address.

  Regular expressions, or regex for short, are a series of special characters that define a search pattern. 
  Example:

   ^([a-zA-Z0-9_\-\.]+)@([a-zA-Z0-9_\-\.]+)\.([a-zA-Z]{2,5})$

    ## Table of Content
  - [Anchors](#Anchors)
  - [Bracket Expressions](#BracketExpressions)
  - [Quantifiers](#Quantifiers)
  - [Grouping Constructs](#GroupingConstructs)
  - [The OR Operator](#TheOROperator)
  - [Character Escapes](#CharacterEscapes)
  - [Character Classes](#CharacterClasses)
  - [Flags](#Flags)




  ## Anchors
  
  The anchor in this example is the caret or (^). This is stating that where ever there is a pattern that begins with the proceeding charaters are that is what will be the match. These are special sequences which match an empty substring: ^ matches at the beginning of the target string, $ matches at the end of the target string and \b matches on a word boundary, i.e., the previous or subsequent character is not a word character.

  ## Bracket Expressions
  A bracket expression represents a character set via a list of characters enclosed by the square brackets: '[' and ']'. It normally matches the target string with any single character from the list.
  If the character list begins with '^', it matches any single character not from the rest of the list.

  If two characters in the list are separated by '–', this is shorthand for the (inclusive) range of characters between those two. It is illegal for two ranges to share an endpoint, e.g. a-c-e. Ranges are collating-sequence dependent and should be avoided for portability.
  Most special characters lose their special status and become literals within brackets. Additionally,
   – is literal at the end or beginning of a bracket expression
   ^ is literal if not at the beginning of a bracket expression
  The backslash character, \, retains its meaning in bracket expressions, permitting the usage of the special escape sequences: such as \n, \t, \w, \d, etc.

  ## Quantifiers
  Regular expressions use quantifiers to generate unbounded matching possibilities and other matching amount specifications. An atom can  optionally be followed by one of these quantifiers:
   -*   representing 0 or more occurrences of the atom,
   -+   representing 1 or more occurrence of the atom,
   -?   representing 0 or 1 occurrences of the atom,
   -the bound {n}   representing exactly n occurrences of the atom,
   -the bound {m,n}   representing between m and n occurrences of the atom.
  The quantifier can optionally be followed by "?" indicating that the match be minimal (non-greedy, reluctant) as opposed to the default maximal (greedy) match.

  ## Grouping Constructs
  Grouping constructs delineate the subexpressions of a regular expression and capture the substrings of an input string. As regular expressions grow more complicated, you may check multiple parts of a string to determine that different sections fulfill different requirements. To break these sections up, you'll need to use grouping constructs. Using parantheses is primary way of group a section

  ## The OR Operator
  Grouping and alternation are core features of every modern regular expression library. You can provide as many terms as desired, as long as they are separated with the pipe character: |. This character separates terms contained within each (...) group.

  Using the OR operator (|), the expression [abc] could be written as (a|b|c). 

  ## Character Escapes
  Let’s say we want to find literally a dot. Not “any character”, but just a dot. To use a special character as a regular one, prepend it with a backslash: \.. That’s also called “escaping a character”.

  It's important to note that all special characters, including the backslash (\), lose their special significance inside bracket expressions.

  ## Character Classes
  Matches any one of the enclosed characters. You can specify a range of characters by using a hyphen, but if the hyphen appears as the first or last character enclosed in the square brackets, it is taken as a literal hyphen to be included in the character class as a normal character. For example, [abcd-] and [-abcd] match the "b" in "brisket", the "c" in "chop", and the "-" (hyphen) in "non-profit".

  ## Flags
  These are filters that you can pass that will affect the way that it is searched. There are multiple options that you can use that will help you narrow your search to help you find the match that will be returned. For example "flag i" is one that will nullify the difference between A and a in the search.

  
  ## Questions

  If you have any questions about the repo, open an issue or contact Github:PinarAktas directly at : pinaraktas81@gmail.com.
  https://github.com/PinarAktas/Regex_Tutorial


  ## License
  Licensed under the [![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC) license


