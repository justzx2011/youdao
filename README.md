# YouDao

        It is a YouDao client for linux.

#Dependencies:
        python-xlib python-webkit xclip
#Installation
        #apt-get install python-xlib python-webkit xclip
        
        $git clone git@github.com:justzx2011/youdao.git
         
        $cd youdao
        
        #python youdao.py
        
TODO
--------------

        1 解决权限问题
        2 解决特殊字符串的输入问题
        3 增强与其它程序的兼容性
        4 重新规划目录、打包
        5 重新格式化网页界面 ----- 使用beautiful soup 
        6 创建配置页面 
DONE
-----
        1 功能模块划分完成   -------   成功的将界面和程序高度分离
        2 主程序结构设计完成   ------  一般情况下结构不会变更
        3 完成了程序退出机制  ------  全局统一退出标志，为差错控制模块预留了接口
RULES
----
        1 界面上永远不许有按钮
        2 主程序中既是测试程序，不许有功能模块
        3 所有功能模块保持最大化的独立，尤其是界面和程序不许纠缠
Construction
----
        
                                      ------
                                  |     主程序       |
                                  |    def main()    |
                                     ----------------
                      -------------       |       ------------
                  |                       |                      |
                  |                       |                      |
             ---------------         ------------         -------------
           |     取词        |    |     查字     |    |        显示        |
           |  def gettext（）|    |  def lookup()|    |     def webshow() |
             ---------------        -------------         --------------
        
        
        
        
        
        
        
        
        
        
        