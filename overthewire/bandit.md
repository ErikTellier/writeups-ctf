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

# Level 4 -> 5

**connection :**
`ssh -p 2220 bandit4@bandit.labs.overthewire.org`

**solution :** 
```bash
cd inhere/
file ./*
cat ./-file07
```

# Level 5 -> 6

**connection :**
`ssh -p 2220 bandit5@bandit.labs.overthewire.org`

**solution :** 
```bash
cd inhere/
find -readable -size 1033c -type f
cat ./maybehere07/.file2
```

# Level 6 -> 7

**connection :**
`ssh -p 2220 bandit6@bandit.labs.overthewire.org`

**solution :** 
```bash
cd ../..
find -size 33c -user bandit7 -group bandit6 2>/dev/null
cat ./var/lib/dpkg/info/bandit7.password
```

# Level 7 -> 8

**connection :**
`ssh -p 2220 bandit7@bandit.labs.overthewire.org`

**solution :** 
```bash
grep "millionth" data.txt
```

# Level 8 -> 9

**connection :**
`ssh -p 2220 bandit8@bandit.labs.overthewire.org`

**solution :** 
```bash
sort data.txt | uniq -u
```

# Level 9 -> 10

**connection :**
`ssh -p 2220 bandit9@bandit.labs.overthewire.org`

**solution :** 
```bash
strings -a data.txt | grep ====
```

# Level 10 -> 11

**connection :**
`ssh -p 2220 bandit10@bandit.labs.overthewire.org`

**solution :** 
```bash
base64 -d data.txt 
```

# Level 11 -> 12

**connection :**
`ssh -p 2220 bandit11@bandit.labs.overthewire.org`

**solution :** 
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

# Level 12 -> 13

**connection :**
`ssh -p 2220 bandit12@bandit.labs.overthewire.org`

**solution :** 
```bash
mktemp -d
cp data.txt /tmp/tmp.XXXXXX
cd /tmp/tmp.XXXXXX
xxd -r data.txt data
file data
mv data data.gz
gzip -d data.gz
file data
mv data data.bz
bzip2 -d data.bz
file data
mv data data.gz
gzip -d data.gz
file data
tar xf data
file data5.bin
tar xf data5.bin
file data6.bin
mv data6.bin data6.bz
bzip2 -d data6.bz
file data6
tar xf data6
file data8.bin
mv data8.bin data8.gz
gzip -d data8.gz
file data8
cat data8
```
