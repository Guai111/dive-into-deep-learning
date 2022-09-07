### time.time() -> return seconds passed from LINUX epoch
`sec = time.time()`

`print(f'seconds passed by from epoch are: {sec}s')
`

### time.ctime(<seconds>) -> return local time
`curtime = time.ctime(sec)
  
print(f'Now is {curtime}')
`
  
### time.struct_time -> object
`time.struct_time(tm_year=2018, tm_mon=12, tm_mday=27, 
                    tm_hour=6, tm_min=35, tm_sec=17, 
                    tm_wday=3, tm_yday=361, tm_isdst=0)
`
  
### time.localtime()
`ltime = time.localtime()
  
print(f'Year is {ltime.tm_year}, month is {ltime.tm_mon}, date is {ltime.tm_mday}')
`
  
### time.gmtime(<seconds>) -> returns struct_time
`stime = time.gmtime(166666660)
  
print(f'Year is {stime.tm_year}, month is {stime.tm_mon}, date is {stime.tm_mday}')
`
  
### time.sleep(<seconds>) -> sleep for <second> time
`print('We are at here!')
  
time.sleep(4)
  
print("After 4 sec!")
`
### Summarize 
Now you know:
1. **time.time()** how to get seconds passed from epoch with **time.time()**
2. **time.ctime(<seconds>)** how to get specific with fixed format date with **time.ctime(<seconds>)**
3. **time.time_structure** how to use **time.time_structure** to obtain attributes like tm_year/tm_mon and so on
4. **time.localtime()** how to get local current time in time structure with it
5. **time.gmtime(<seconds>)** how to get time structure of specific time
