# 要經彙集
## Dependencies
- uplatex
- Microsoft fonts `simsun.ttc`, `simhei.ttf`, `simkai.ttf`

## Build
Build `upzhserif-v.tfm`:
```
jfmutil zpl2tfm -u --lenient upzhserif-v.zpl
```
Making sure that the fonts used in this document is reachable
```
ln -s /path/to/simsun.ttc simsun.ttc
ln -s /path/to/simkai.ttf simkai.ttf
ln -s /path/to/simhei.ttf simhei.ttf 
```
Build using `uplatex`
```
uplatex yjhj && uplatex yjhj && dvipdfmx yjhj
```
