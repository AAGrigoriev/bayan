## Bayan
Duplicate file search utility

### Options:
```
  -i [ --include    ] Include paths for scaning (required)
  -e [ --exclude    ] Exclude paths from scaning (optional, by default is not set)
  -l [ --level      ] Scan nesting level (optional, by default is 0 - without nested)
  -s [ --min-size   ] Minimum file size in bytes for scaning (optional, by default is 1)
  -m [ --masks      ] Masks for file names allowed for comparison (optional, by default is not set)
  -b [ --block-size ] Block size in bytes for reading file (optional, by default is 1024)
  -a [ --algorithm  ] Hash algorithm: crc16 or crc32 (optional, by default is crc32)
  -h [ --help       ] Show help
```

### Examples: 
**long options:**

`bayan --include /home --exclude /~/temp --level=3 --min-size=256 --masks *.cpp *.txt --block-size=1024 --algorithm=crc32`

**short options:**

`bayan -i /home -e /~/temp -l 3 -s 256 -m*.cpp *.txt -b 1024 -a crc32`
