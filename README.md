# timging_the_market_multifactors

# *Project Title*

权益市场因子择时模型

卷 TU100 的文件夹 PATH 列表
卷序列号为 0000-0000

# *Keywords and Descriptions*

- 权益市场、多因子、择时
- 流程为：原始数据提取并清理-->因子值计算-->信号值计算-->因子组合得出结果，可由三分.ipynb脚本实现

# Dictionary
E:.

│  CompositSignal_LoopModule_BackTesting.ipynb --信号组合.ipynb

│  CompositSignal_LoopModule_BackTesting.py --信号组合.py

│  configuration.py -- 配置文件

│  SQL_GetSignals.ipynb --信号更新并写入SQL

│  SQL_UpDate.ipynb --metadata、因子值更新并写入SQL  

├─db -- database

│      database.md

│      中国社会融资规模存量同比.xlsx
│      

├─src -- 业务模块

│  │  src_CompositSignal_LoopModule.py
│          

└─utils  -- 公用模块
        SQL_DataBase.ipynb

# *Instructions*        
- .py文件是为了后续拓展形成的模块包，日常使用仅使用.ipynb文件即可
- 顺序：
更新metadata并写入sql、更新因子值并写入sql-->更新信号值并写入sql-->进行因子组合
（SQL_UpDate.ipynb）-->（SQL_GetSignals.ipynb）-->（CompositSignal_LoopModule_BackTesting.ipynb ）
