# CLI Documentation
The prefix is always `arithmos`.

> **Content List**
- Commands
- Arguments
- Option
- Aliases

<br>

## Commands
- encrypt `[text]`
- decrypt `[cipher]`
- version

<br>
<br>

## Arguments
> encrypt `[text]`

`text` : the string to be encrypted into a cipher.

> decrypt `[cipher]`

`cipher` : the cipher to be decrypted into a string.

> version

Not have arguments.

<br>
<br>

## Option

> encrypt `[text]` `[option]` `[option args]`

**Option :**
- `--ignore`/`-i` | letters that will not be encrypted by the algorithm.
if you don't want to encrypt more than 1 letter or sentence, add `--ignore`/`-g` again as before.

**Example :**
```
arithmos encrypt example -i e

# output
2401131612 (xampl)

# more than 1 letters and sentence
arithmos encrypt example123 -i e -i 123

# output
2401131612 (xampl)
```

<br>
<br>

> decrypt `[text]` `[option]` `[option args]`

**Option :**
- `--ignore`/`-i` | number that will not be decrypted by the algorithm.
if you don't want to decrypt more than 1 number or sentence, add `--ignore`/`-g` again as before.

**Example :**
```
arithmos decrypt 05240113161205 -i 05

# output
xampl (2401131612)

# more than 1 number and sentence
arithmos decrypt 05240113161205868788 -i 05 -i 868788

# output
xampl (2401131612)
```

<br>
<br>

> version

Not have option.

<br>
<br>

## Aliases
Commands aliases.

**Alias :**
- encrypt = `enc`
- decrypt = `dec`
- version = `ver`