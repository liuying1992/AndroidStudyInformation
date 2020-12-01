# AndroidStudyInformation 学习资料

#### Android文件存储路径
|  区别   | 方法  | 说明 |
|  ----  | ----  |---- |
| 外部存储  | Environment.getExternalStorageDirectory() |  SD卡根目录 /mnt/sdcard|
| 应用扩展存储  | 	context.getExternalFilesDir(dir) |/mnt/sdcard/Android/data/< package name >/files/… 获取SD卡上的缓存目录，可以用来保存一些缓存文件如图片|
|应用私有存储|context.getFilesDir()|路径是:/data/data/< package name >/files/…可以用来保存不能公开给其他应用的一些敏感数据如用户个人信息|