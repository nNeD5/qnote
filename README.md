# qnote - quick notes

Command line utility for daily and weekly note taking.

## Usage

qnote will create `${DIARY_DIR}/{week}/{year-month-day}.md` file structure to store nodes.

### Commands:

- `qnote today(t)`: open/create today note
- `qnote week(w)`: open/create current week note
- `qnote prev-day(pd)`: open/create yesterday note
- `qnote yesterday(y)`: alias to prev-day
- `qnote prev-week(pw)`: open/create previos week note
- `qnote next-day(nd)`: open/create tommorow note
- `qnote next-week(nw)`: open/create next week note
- `qnote list(l)`: list all notes. ignore hidden direcotry
- `qnote select(s)`: selet and open note. Ignore hidden direcotry. And actually search from `${DIARY_DIR}/../` ) (require [fzf][https://github.com/junegunn/fzf?tab=readme-ov-file#installation])

## Configuration

Use enviroment variable `NOTES_DIR` to set where notes will be stored.
Add next string to your .bashrc/.zshrc. Obviously any path can be provided.
```sh
$ export DIARY_DIR="${HOME}/Notes/diary"
```
By default `DIARY_DIR` set to `${HOME}/Notes/diary`

## TODO:

- [ ] Templates
- [ ] synchronization whith [HabitNow][https://play.google.com/store/apps/details?id=com.habitnow&hl=en_US]
