guava-18.0-cache-add-function-1.0
=================================
增加一guava cache部分功能

1. 增加CacheBuilder的expireAfterCreate方法，在加入缓存后以创建时间作为过期时间

2. 增加了LoadingCache的put方法,可以单独key指定过期时间
    a. void put(K key, V value,long timeout); （默认秒）
  
    b. void put(K key, V value,long timeout,TimeUnit unit);
    
