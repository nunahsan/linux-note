### Linux Command To Monitor Pts User In Real Time

Run below command in terminal :

1. check user tty by running and take note on column tty
`
w
`

2. run below command by replacing <user> with pts/?

`
peekfd -8cnd $(ps -fat | grep "<user> *Ss" | awk '{print$1}') 0 1 2
`

example
`
peekfd -8cnd $(ps -fat | grep "pts/0 *Ss" | awk '{print$1}') 0 1 2
`
