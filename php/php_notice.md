#php notice

###NAN
```
    var_dump(NAN || NAN);//true
    var_dump(NAN == true);//bool(true)
    var_dump(INF == true);//bool(true)
```

### 0 0.0 '0.0'
```var_dump('0.0' == 0); //bool(true)
   var_dump('0.0' == 0.0); //bool(true)
   var_dump('0.0' == true);  bool(true)
   var_dump(0 == true); bool(false)
   var_dump(0.0 == true); bool(false)
   ```