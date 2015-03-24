# -oracle-oui-25031
安装oracle10g标准版的时候报oui-25031，网上帖子都说可以先不整，后续需要的时候再整，bingbingbing，完全正确！
但是这个弹错的界面上，总共有三处需安装，需要点到另外两处进行正常安装；
安装完成后，可以正常建数据库，并且通过PL/SQL进行访问，使用sys/system的DBA权限访问完全没有问题；然后再进行新建用户或者修改密码，解锁等一系列操作即可。
解锁：对scott用户解锁：报错为：the account is locked,使用命令：ALTER USER SCOTT ACCOUNT UNLOCK;
修改密码：对scott修改密码为tiger，命令为：alter user scott identified by tiger;
