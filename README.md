# Rubcop Rules

Just a place to keep shared rubocop rules for Stootie

## What is it for?

The rubocop.yml file in this repository should hold the standard rules for
Stootie's ruby projects, those we want every project to follow, and the
exceptions thereof.

Everyone in the team is welcome to contribute, but try to keep it generic
(your project's local .rubocop.yml is there to keep project-specific rules
and exceptions) and reallistic (having too high a standard is worse than no
standard at all ^^).

## Getting started

Just add this to your project's ```.rubocop.yml``` and you're rolling:
```ruby
# .rubocop.yml
inherit_from:
  - 'https://raw.githubusercontent.com/stootie/rubocop-rules/master/rubocop.yml'
```

As the shared config is cached, you might also want to add to your .gitignore:

```
# .gitignore
.rubocop-*
```

If you add a rule to this repository and want to see it affect your current
project right away, remove the cache file:

```bash
rm .rubocop-*
```

Aaaaand that's pretty much all.
