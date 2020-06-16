# ST

## Installation

First clone the repo

```
git clone https://github.com/cmp102/st.git
cd st
```

Install for all users (this action should be done as root)

```
make clean install
```

Install for your actual user (~/.local/bin should be added to the PATH env var)

```
make clean install PREFIX=~/.local
```

## Keep tracking orignal suckless master branch

Setup:

```
git remote add suckless git://git.suckless.org/st
git pull suckless master:suckless
git branch --set-upstream-to=suckless/master suckless
```

Update branch:
```
git checkout suckless
git pull
```

