Odoo模組開發實戰
# 目錄
 1.models介紹
 2.常用的模型屬性
 
## 第一章 models介紹

|  名稱    | 功能 |  
| --------| -------- | 
| Model| Model是儲存資料記錄的最主要手段，它是持久化地對資料記錄(record)進行儲存，直至對其進行刪除 | 
|BaseModel|MetaModel的子類，是AbstractModel、TransientModel和Model的父類|
| TransientModel| 稱之為"瞬時模型"，與Model的差別是每日會清除該瞬時模型的資料| 
| MetaModel | 主要作用是註冊每个模塊中的模型 | 
| AbstractModel | 抽象類中定義一些通用的欄位和方法，在子類中進行繼承或者重寫 |  
 
## 第二章 屬性

|  名稱    | 內容 |  
| --------| -------- | 
| _name| 模型的名稱| 
| _description| 模型的描述信息| 
| _inherit| 繼承的模型列表| 
| _table| 指定數據庫中生成的表名| 
|__sql_constraints| 指定SQL約束[(name,約束,信息)]|
|_rec_name| 標籤名稱|
|_order| 排序依據，莫認為id字段|
|_parent_name|父级字段 Many2one字段用作父字段|
|_parent_store|是否存储父级路徑|
