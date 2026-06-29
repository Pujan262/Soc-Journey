# Day 9 — Linux File Permissions

## Permission Values
- Read (r) = 4
- Write (w) = 2
- Execute (x) = 1

## Combinations
- r+w+x = 7
- r-- = 4
- -w- = 2
- --x = 1

## Who the 3 digits represent
- u = user (owner)
- g = group
- o = others

## Commands
- ls -la — view file permissions
- chmod — change permissions (change mode)

## Example
chmod 744 example.txt
- Owner (u) = 7 = read+write+execute
- Group (g) = 4 = read only
- Others (o) = 4 = read only
