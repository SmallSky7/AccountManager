# 测试账户管理器

提供一个工具，便于测试工程师更方便的管理自己的账户，实现账户脚本一键生成并导出，账户资金、证券余额一键增加

##前置准备

conf/database.xml
配置数据库相关表的执行策略
'''
<?xml version="1.0" encoding="UTF-8"?>
<database>username:password@127.0.0.1:8088/orcl</database>

<table tablename="User">
    <coloum coloumname="Username">
        <strategy></strategy>
    </coloum>
    <coloum coloumname="UserId">
        <strategy></strategy>
    </coloum>
    <coloum coloumname="position_str">
        <strategy>UserId</strategy>
    </coloum>
</table>
'''

conf/table.properties
配置相关操作对应的表
'''
accountcreate=User
fundAdd=fund
stockAdd=Stock
'''
