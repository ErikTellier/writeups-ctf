# Level 0

**connection :**
`ssh -p 2220 bandit0@bandit.labs.overthewire.org`

mdp : `bandit0`

# Level 0 -> 1

**connection :**
`ssh -p 2220 bandit0@bandit.labs.overthewire.org`
mdp : `bandit0`

**solution :** 
```bash
cat readme
```

# Level 1 -> 2

**connection :**
`ssh -p 2220 bandit1@bandit.labs.overthewire.org`

**solution :** 
```bash
cat ./-
```

# Level 2 -> 3

**connection :**
`ssh -p 2220 bandit2@bandit.labs.overthewire.org`

**solution :** 
```bash
cat ./--spaces\ in\ this\ filename--
```

# Level 3 -> 4

**connection :**
`ssh -p 2220 bandit3@bandit.labs.overthewire.org`

**solution :** 
```bash
cd inhere/
ls -la
cat ...Hiding-From-You
```