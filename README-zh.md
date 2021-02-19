# vue-admin-template

> 这是一个极简的 vue admin 管理后台。它只包含了 Element UI & axios & iconfont & permission control & lint，这些搭建后台必要的东西。

[线上地址](http://panjiachen.github.io/vue-admin-template)

[国内访问](https://panjiachen.gitee.io/vue-admin-template)

目前版本为 `v4.0+` 基于 `vue-cli` 进行构建，若你想使用旧版本，可以切换分支到[tag/3.11.0](https://github.com/PanJiaChen/vue-admin-template/tree/tag/3.11.0)，它不依赖 `vue-cli`。

## Extra

如果你想要根据用户角色来动态生成侧边栏和 router，你可以使用该分支[permission-control](https://github.com/PanJiaChen/vue-admin-template/tree/permission-control)

## 相关项目

- [vue-element-admin](https://github.com/PanJiaChen/vue-element-admin)

- [electron-vue-admin](https://github.com/PanJiaChen/electron-vue-admin)

- [vue-typescript-admin-template](https://github.com/Armour/vue-typescript-admin-template)

- [awesome-project](https://github.com/PanJiaChen/vue-element-admin/issues/2312)

写了一个系列的教程配套文章，如何从零构建后一个完整的后台项目:

- [手摸手，带你用 vue 撸后台 系列一(基础篇)](https://juejin.im/post/59097cd7a22b9d0065fb61d2)
- [手摸手，带你用 vue 撸后台 系列二(登录权限篇)](https://juejin.im/post/591aa14f570c35006961acac)
- [手摸手，带你用 vue 撸后台 系列三 (实战篇)](https://juejin.im/post/593121aa0ce4630057f70d35)
- [手摸手，带你用 vue 撸后台 系列四(vueAdmin 一个极简的后台基础模板,专门针对本项目的文章,算作是一篇文档)](https://juejin.im/post/595b4d776fb9a06bbe7dba56)
- [手摸手，带你封装一个 vue component](https://segmentfault.com/a/1190000009090836)

## Build Setup

```bash
# 克隆项目
git clone https://github.com/PanJiaChen/vue-admin-template.git

# 进入项目目录
cd vue-admin-template

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装以来，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 [http://localhost:9528](http://localhost:9528)

## 发布

```bash
# 构建测试环境
npm run build:stage

# 构建生产环境
npm run build:prod
```

## 其它

```bash
# 预览发布环境效果
npm run preview

# 预览发布环境效果 + 静态资源分析
npm run preview -- --report

# 代码格式检查
npm run lint

# 代码格式检查并自动修复
npm run lint -- --fix
```

更多信息请参考 [使用文档](https://panjiachen.github.io/vue-element-admin-site/zh/)

## 购买贴纸

你也可以通过 购买[官方授权的贴纸](https://smallsticker.com/product/vue-element-admin) 的方式来支持 vue-element-admin - 每售出一张贴纸，我们将获得 2 元的捐赠。

## Demo

![demo](https://github.com/PanJiaChen/PanJiaChen.github.io/blob/master/images/demo.gif)

## Browsers support

Modern browsers and Internet Explorer 10+.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions

## License

[MIT](https://github.com/PanJiaChen/vue-admin-template/blob/master/LICENSE) license.

## 澳門官網後臺
```bash
角色列表：
--權限名
--salse
--市場部人員
--按揭APP管理員
--兼職
--Admin
--VIPUser
--字典管理員
```
```bash
角色權限：
salse : 
  權限菜单 : 活動報名	Registration/GetList
市場部人員 :
    已有權限	     路徑
    澳門區-住宅	     RecommendProperty/List?type=MP
    工商舖-工商	     RecommendProperty/List?type=BS
    新增筍盤推介	 RecommendProperty/Add
    修改筍盤推介	 RecommendProperty/Edit
    刪除筍盤推介	 API/RecommendProperty/Delete
    新增澳門區-住宅	 RecommendProperty/Add?type=MP
    新增氹仔區-住宅	 RecommendProperty/Add?type=TP
    查看審核失敗樓盤-详细	SearchBuilding/FailOne
    審核失敗樓盤	SearchBuilding/FailList
    操作審核樓盤	SearchBuilding/CheckBuildingOne
    新增樓盤聯繫人	SearchBuilding/AddContacts
    查看聯繫人	    SearchBuilding/ListContacts
    查看樓盤圖片	SearchBuilding/BuildingImages
    會員列表	    Users/List
    修改會員	    Users/UpdateUsers
    修改樓盤	    SearchBuilding/UpdateBuilding
    已發佈房源	    SearchBuilding/List
    会员物业信息	VIPPropertyInfo/Index
    删除加入中原	
    会员基本信息	VIPUserManage/Index
    删除關於中原	
    新增加入中原	Article/Add?type=JO
    会员信息导入	Home/Index
    修改氹仔區-住宅	RecommendProperty/Edit?type=TP
    修改工商鋪-工商	RecommendProperty/Edit?type=BS
    删除澳門區-住宅	API/RecommendProperty/Delete?type=mp
    删除氹仔區-住宅	API/RecommendProperty/Delete?type=tp
    澳門區	Article/GetList?type=FMC
    氹仔區	Article/GetList?type=FTP
    東方明珠區	Article/GetList?type=FOP
    工商鋪	Article/GetList?type=FBS
    香港	Article/GetList?type=FHK
    大陸	Article/GetList?type=FML
    橫琴區	Article/GetList?type=FHQ
    修改焦點新盤—澳門區	Article/Edit?type=FMC
    刪除焦點新盤—澳門區	API/Article/Delete?type=FMC
    新增焦點新盤—氹仔區	Article/Add?type=FTP
    修改焦點新盤—氹仔區	Article/Edit?type=FTP
    刪除焦點新盤—氹仔區	API/Article/Delete?type=FTP
    新增焦點新盤—東方明珠區	Article/Add?type=FOP
    修改焦點新盤—東方明珠區	Article/Edit?type=FOP
    刪除焦點新盤—東方明珠區	API/Article/Delete?type=FOP
    新增焦點新盤—工商鋪	Article/Add?type=FBS
    修改焦點新盤—工商鋪	Article/Edit?type=FBS
    刪除焦點新盤—工商鋪	API/Article/Delete?type=FBS
    新增焦點新盤—香港	Article/Add?type=FHK
    修改分行網絡	BranchNetwork/Edit
    删除分行網絡	API/BranchNetwork/Delete
    修改關於中原	Article/Edit?type=AB
    添加樓盤	SearchBuilding/Add
    新增分行網絡	BranchNetwork/Add
    修改中原動態	Article/Editt?type=CN
    關於中原	Article/GetList?type=AB
    删除政府部門網址	WebSite/DeleteSite
    新增常用政府部門網址	WebSite/Add
    修改常用政府部門網址	WebSite/Edit
    删除樓市成交數據	Api/TransactionData/Delete
    新增樓市成交數據	TransactionData/Add
    樓市成交數據	TransactionData/List
    修改景氣指數	BoomIndex/Edit
    景氣指數	BoomIndex/List
    工商鋪文章	Article/GetList?type=GSP
    獨家研究	Article/GetList?type=EX
    修改獨家研究	Article/Edit?type=EX
    新增工商鋪文章	Article/Add?type=GSP
    刪除工商鋪文章	
    刪除獨家研究	
    批量導入数据	TransactionData/ExcelImport
    常用政府部門網址	WebSite/List
    中原動態	Article/GetList?type=CN
    分行網絡	BranchNetwork/List
    删除中原動態	
    加入中原	Article/GetList?type=JO
    修改工商鋪文章	Article/Edit?type=GSP
    删除景氣指數	API/BoomIndex/Delete
    刪除焦點新盤—橫琴區	API/Article/Delete?type=FHQ
    新增焦點新盤—橫琴區	Article/Add?type=FHQ
    新增焦點新盤—大陸	Article/Add?type=FML
    修改焦點新盤—大陸	Article/Edit?type=FML
    刪除焦點新盤—大陸	API/Article/Delete?type=FML
    新增景氣指數	BoomIndex/Add
    新增獨家研究	Article/Add?type=EX
    修改樓市成交數據	TransactionData/Edit
    新增關於中原	Article/Add?type=AB
    修改焦點新盤—橫琴區	Article/Edit?type=FHQ
    刪除焦點新盤—香港	API/Article/Delete?type=FHK
    新增焦點新盤—澳門區	Article/Add?type=FMC
    删除工商鋪-工商	API/RecommendProperty/Delete?type=bs
    批量導入数据	RecommendProperty/ExcelImport
    修改焦點新盤—香港	Article/Edit?type=FHK
    修改澳門區-住宅	RecommendProperty/Edit?type=MP
    新增中原動態	Article/Add?type=CN
    新增工商鋪-工商	RecommendProperty/Add?type=BS
    修改加入中原	Article/Edit?type=JO
    待審核樓盤	SearchBuilding/CheckBuilding
    氹仔區-住宅	RecommendProperty/List?type=TP&id=1
    刪除樓盤	api/Building/DeleteBuilding
    樓盤字典	Estate/EstateList
    员工管理	Staff/List
    添加封面圖	HomePagerManager/AddCoverImage
    查看封面圖	HomePagerManager/CoverImages
    官网首页显示	Article/ArTopList
    待確認房源	PreBuilding/List
    学院文章	Article/GetList?type=CA
    新增学院文章	Article/Add?type=CA
    新增学院文章	Article/Add?type=CA
    新增活动介绍	Article/Add?type=HD
    修改学院文章	Article/Editt?type=CA
    修改活动介绍	Article/Editt?type=HD
    视频揾楼	SearchByVideo/Index
    聚焦二手	EstatesBook/Index
    新增楼盘	Estate/EstateList
    編輯樓盤	Estate/EstateList
    刪除樓盤	Estate/EstateList
    楼市分析	AppArticle/List?type=347
    按揭须知	AppArticle/List?type=350
    市况速递	AppArticle/List?type=353
    按揭新闻	AppArticle/List?type=356
    按揭流程	AppArticle/List?type=357
    按揭简介	AppArticle/List?type=358
    廣告管理	AppArticle/List?type=359
    联系我们	AppArticle/ContactEdit?Operat=ContactUs
    联系我们	AppArticle/ContactEdit?Operat=ContactUs
    轉介流程	AppArticle/List?type=364
    员工管理-新增	Staff/Add
    樓盤天書	EstatesBook/BookIndex
    活动介绍删除	Activities/Delete
    橫琴分析	Article/GetList?type=HQ
    修改橫琴分析	Article/Edit?type=HQ
    新增橫琴分析	Article/Add?type=HQ
    SEO管理	PageSeo/List
    人員角色	Permissions/AddPermissions
    活动介绍	Article/GetList?type=HD
    活动介绍	Activities/GetList
    平均呎价图	BoomIndex/AvgPic
    活動報名	Registration/GetList
    預約睇樓	Reserve/Index
    橫琴分析2	Article/GetList?type=HQ
    網上放盤	Online/Index
    會員角色管理	VIPRoleManage/Index
    系統字典	Dictionary/Index
    流水號生成規則	CodeRule/List
    添加流水號	CodeRule/Add
    修改流水號	CodeRule/Edit
    添加會員	Users/AddUsers
    刪除會員	Api/Users/DeleteUsers
    角色列表	Permissions/ListRole
    角色權限	Permissions/AddRoleFor
    添加角色	Permissions/AddRole
    修改角色	Permissions/UpdateRole
    数据库备份	DataBase/GetDataBaseBackUp
    操作日志	LogRecord/GetList
    查看日志	actionlog/action
    免責聲明	Other/Index?type=Other_Disclaimer
    使用條款	Other/Index?type=Other_Terms
    配寘項	File/FileList
    PDF配寘	File/PDFUpload
    Url配寘	File/PathConfig
    會員角色管理	VIPRoleManage/Index
    系統字典	Dictionary/Index
    流水號生成規則	CodeRule/List
    添加流水號	CodeRule/Add
    修改流水號	CodeRule/Edit
    添加會員	Users/AddUsers
    刪除會員	Api/Users/DeleteUsers
    角色列表	Permissions/ListRole
    角色權限	Permissions/AddRoleFor
    添加角色	Permissions/AddRole
    修改角色	Permissions/UpdateRole
    数据库备份	DataBase/GetDataBaseBackUp
    操作日志	LogRecord/GetList
    查看日志	actionlog/action
    免責聲明	Other/Index?type=Other_Disclaimer
    使用條款	Other/Index?type=Other_Terms
    配寘項	File/FileList
    PDF配寘	File/PDFUpload
    Url配寘	File/PathConfig
按揭APP管理員:
    已有權限	路徑
    按揭简介	AppArticle/List?type=358
    按揭流程	AppArticle/List?type=357
    按揭新闻	AppArticle/List?type=356
    市况速递	AppArticle/List?type=353
    按揭须知	AppArticle/List?type=350
    楼市分析	AppArticle/List?type=347
兼職:
    已有權限	路徑
    澳門區-住宅	RecommendProperty/List?type=MP
    氹仔區-住宅	RecommendProperty/List?type=TP&id=1
    工商舖-工商	RecommendProperty/List?type=BS
    新增筍盤推介	RecommendProperty/Add
    修改筍盤推介	RecommendProperty/Edit
    刪除筍盤推介	API/RecommendProperty/Delete
    批量導入数据	RecommendProperty/ExcelImport
    聚焦二手	EstatesBook/Index
    網上放盤	Online/Index
VIPUser:
字典管理員:
  已有權限	路徑
  系統字典	Dictionary/Index
Admin:
  權限菜单 : 澳門區-住宅     路徑 : RecommendProperty/List?type=MP
  權限菜单 : 氹仔區-住宅     路徑 : RecommendProperty/List?type=TP&id=1
  權限菜单 : 工商舖-工商     路徑 : RecommendProperty/List?type=BS
  權限菜单 : 新增筍盤推介    路徑 : RecommendProperty/Add
  權限菜单 : 修改筍盤推介    路徑 : RecommendProperty/Edit
  權限菜单 : 刪除筍盤推介    路徑 : API/RecommendProperty/Delete
  權限菜单 : 新增澳門區-住宅 路徑 : RecommendProperty/Add?type=MP
  權限菜单 : 新增氹仔區-住宅 路徑 : RecommendProperty/Add?type=TP
  權限菜单 : 新增工商鋪-工商 路徑 : RecommendProperty/Add?type=BS
  權限菜单 : 修改澳門區-住宅 路徑 : RecommendProperty/Edit?type=MP
  權限菜单 : 修改氹仔區-住宅 路徑 : RecommendProperty/Edit?type=TP
  權限菜单 : 修改工商鋪-工商 路徑 : RecommendProperty/Edit?type=BS
  權限菜单 : 批量導入数据    路徑 : RecommendProperty/ExcelImport
  權限菜单 : 删除澳門區-住宅 路徑 : API/RecommendProperty/Delete?type=mp
  權限菜单 : 删除氹仔區-住宅  路徑 : API/RecommendProperty/Delete?type=tp
  權限菜单 : 删除工商鋪-工商 路徑 : API/RecommendProperty/Delete?type=bs
  權限菜单 : 澳門區  路徑 : Article/GetList?type=FMC
  權限菜单 : 氹仔區  路徑 : Article/GetList?type=FTP
  權限菜单 : 東方明珠區 路徑 : Article/GetList?type=FOP
  權限菜单 : 工商鋪 路徑 : Article/GetList?type=FBS
  權限菜单 : 香港 路徑 : Article/GetList?type=FHK
  權限菜单 : 大陸 路徑 : Article/GetList?type=FML
  權限菜单 : 橫琴區 路徑 : Article/GetList?type=FHQ
  權限菜单 : 新增焦點新盤—澳門區 路徑 : Article/Add?type=FMC
  權限菜单 : 修改焦點新盤—澳門區 路徑 : Article/Edit?type=FMC
  權限菜单 : 刪除焦點新盤—澳門區 路徑 : API/Article/Delete?type=FMC
  權限菜单 : 新增焦點新盤—氹仔區 路徑 : Article/Add?type=FTP
  權限菜单 : 修改焦點新盤—氹仔區 路徑 : Article/Edit?type=FTP
  權限菜单 : 刪除焦點新盤—氹仔區  路徑 : API/Article/Delete?type=FTP
  權限菜单 : 新增焦點新盤—東方明珠區 路徑 : Article/Add?type=FOP
  權限菜单 : 修改焦點新盤—東方明珠區 路徑 : Article/Edit?type=FOP
  權限菜单 : 刪除焦點新盤—東方明珠區 路徑 : API/Article/Delete?type=FOP
  權限菜单 : 新增焦點新盤—工商鋪 路徑 : Article/Add?type=FBS
  權限菜单 : 修改焦點新盤—工商鋪 路徑 : Article/Edit?type=FBS
  權限菜单 : 刪除焦點新盤—工商鋪 路徑 : API/Article/Delete?type=FBS
  權限菜单 : 新增焦點新盤—香港 路徑 : Article/Add?type=FHK
  權限菜单 : 修改焦點新盤—香港 路徑 : Article/Edit?type=FHK
  權限菜单 : 刪除焦點新盤—香港 路徑 : API/Article/Delete?type=FHK
  權限菜单 : 新增焦點新盤—大陸 路徑 : Article/Add?type=FML
  權限菜单 : 修改焦點新盤—大陸 路徑 : Article/Edit?type=FML
  權限菜单 : 刪除焦點新盤—大陸 路徑 : API/Article/Delete?type=FML
  權限菜单 : 新增焦點新盤—橫琴區 路徑 : Article/Add?type=FHQ
  權限菜单 : 修改焦點新盤—橫琴區 路徑 : Article/Edit?type=FHQ
  權限菜单 : 刪除焦點新盤—橫琴區 路徑 : API/Article/Delete?type=FHQ
  權限菜单 : 官网首页显示 路徑 : Article/ArTopList
  權限菜单 : 景氣指數 路徑 : BoomIndex/List
  權限菜单 : 新增景氣指數 路徑 : BoomIndex/Add
  權限菜单 : 修改景氣指數 路徑 : BoomIndex/Edit
  權限菜单 : 删除景氣指數 路徑 : API/BoomIndex/Delete
  權限菜单 : 獨家研究 路徑 : Article/GetList?type=EX
  權限菜单 : 工商鋪文章 路徑 : Article/GetList?type=GSP
  權限菜单 : 新增獨家研究 路徑 : Article/Add?type=EX
  權限菜单 : 修改獨家研究 路徑 : Article/Edit?type=EX
  權限菜单 : 刪除獨家研究 路徑 : 
  權限菜单 : 新增工商鋪文章 路徑 : Article/Add?type=GSP
  權限菜单 : 修改工商鋪文章 路徑 : Article/Edit?type=GSP
  權限菜单 : 刪除工商鋪文章 
  權限菜单 : 新增工商鋪文章 路徑 : Article/Add?type=GSP
  權限菜单 : 修改工商鋪文章 路徑 : Article/Edit?type=GSP
  權限菜单 : 刪除工商鋪文章
  權限菜单 : 樓市成交數據 路徑 : TransactionData/List
  權限菜单 : 批量導入数据 路徑 : TransactionData/ExcelImport
  權限菜单 : 新增樓市成交數據  路徑 : TransactionData/Add
  權限菜单 : 修改樓市成交數據  路徑 : TransactionData/Edit
  權限菜单 : 删除樓市成交數據  路徑 : Api/TransactionData/Delete
  權限菜单 : 常用政府部門網址  路徑 : WebSite/List
  權限菜单 : 新增常用政府部門網址 路徑 : WebSite/Add
  權限菜单 : 修改常用政府部門網址 路徑 : WebSite/Edit
  權限菜单 : 删除政府部門網址 路徑 : WebSite/DeleteSite
  權限菜单 : 中原動態 路徑 :  Article/GetList?type=CN
  權限菜单 : 分行網絡 路徑 : BranchNetwork/List
  權限菜单 : 關於中原 路徑 : Article/GetList?type=AB
  權限菜单 : 加入中原 路徑 : Article/GetList?type=JO
  權限菜单 : 新增中原動態 路徑 : Article/Add?type=CN
  權限菜单 : 修改中原動態 路徑 : Article/Editt?type=CN
  權限菜单 : 删除中原動態
  權限菜单 : 新增分行網絡 路徑 : BranchNetwork/Add
  權限菜单 : 修改分行網絡 路徑 : BranchNetwork/Edit
  權限菜单 : 删除分行網絡 路徑 : API/BranchNetwork/Delete
  權限菜单 : 新增關於中原 路徑 : Article/Add?type=AB
  權限菜单 : 修改關於中原 路徑 : Article/Edit?type=AB
  權限菜单 : 删除關於中原
  權限菜单 : 新增加入中原 路徑 : Article/Add?type=JO
  權限菜单 : 修改加入中原 路徑 : Article/Edit?type=JO
  權限菜单 : 删除加入中原 
  權限菜单 : 会员基本信息 路徑 : VIPUserManage/Index
  權限菜单 : 会员信息导入 路徑 : Home/Index
  權限菜单 : 会员物业信息 路徑 : VIPPropertyInfo/Index
  權限菜单 : 會員角色管理 路徑 : VIPRoleManage/Index
  權限菜单 : 已發佈房源  路徑 : SearchBuilding/List
  權限菜单 : 待審核樓盤 路徑 : SearchBuilding/CheckBuilding
  權限菜单 : 添加樓盤 路徑 : SearchBuilding/Add
  權限菜单 : 修改樓盤 路徑 : SearchBuilding/UpdateBuilding
  權限菜单 : 查看樓盤圖片 路徑 : SearchBuilding/BuildingImages
  權限菜单 : 查看聯繫人 路徑 : SearchBuilding/ListContacts
  權限菜单 : 新增樓盤聯繫人 路徑 : SearchBuilding/AddContacts
  權限菜单 : 操作審核樓盤 路徑 : SearchBuilding/CheckBuildingOne
  權限菜单 : 審核失敗樓盤 路徑 : SearchBuilding/FailList
  權限菜单 : 查看審核失敗樓盤-详细 路徑 : SearchBuilding/FailOne
  權限菜单 : 刪除樓盤 路徑 : api/Building/DeleteBuilding
  權限菜单 : 待確認房源 路徑 : PreBuilding/List
  權限菜单 : 樓盤字典 路徑 : Estate/EstateList
  權限菜单 : 新增楼盘 路徑 : Estate/EstateList
  權限菜单 : 編輯樓盤 路徑 : Estate/EstateList
  權限菜单 : 刪除樓盤 路徑 : Estate/EstateList
  權限菜单 : 系統字典 路徑 : Dictionary/Index
  權限菜单 : 流水號生成規則 路徑 : CodeRule/List
  權限菜单 :  添加流水號  路徑 : CodeRule/Add
  權限菜单 : 修改流水號 路徑 : CodeRule/Edit
  權限菜单 : 會員列表 路徑 : Users/List
  權限菜单 : 添加會員 路徑 : Users/AddUsers
  權限菜单 : 修改會員 路徑 : Users/UpdateUsers
  權限菜单 : 刪除會員 路徑 : Api/Users/DeleteUsers
  權限菜单 : 人員角色 路徑 : Permissions/AddPermissions
  權限菜单 : 角色列表 路徑 : Permissions/ListRole
  權限菜单 : 角色權限 路徑 : Permissions/AddRoleFor
  權限菜单 : 添加角色 路徑 : Permissions/AddRole
  權限菜单 :  修改角色  路徑 : Permissions/UpdateRole
  權限菜单 : 数据库备份 路徑 : DataBase/GetDataBaseBackUp
  權限菜单 : 操作日志 路徑 : LogRecord/GetList
  權限菜单 : 查看日志 路徑 : actionlog/action
  權限菜单 : 员工管理 路徑 : Staff/List
  權限菜单 : 添加封面圖 路徑 : HomePagerManager/AddCoverImage
  權限菜单 : 查看封面圖 路徑 :  HomePagerManager/CoverImages
  權限菜单 : 学院文章 路徑 : Article/GetList?type=CA
  權限菜单 : 活动介绍 路徑 : Activities/GetList
  權限菜单 : 新增学院文章 路徑 : Article/Add?type=CA
  權限菜单 : 新增活动介绍 路徑 : Article/Add?type=HD
  權限菜单 : 修改学院文章 路徑 : Article/Editt?type=CA
  權限菜单 : 修改活动介绍 路徑 : Article/Editt?type=HD
  權限菜单 : SEO管理 路徑 : PageSeo/List
  權限菜单 : 视频揾楼  路徑 : SearchByVideo/Index
  權限菜单 : 聚焦二手 路徑 : EstatesBook/Index
  權限菜单 : 楼市分析 路徑 : AppArticle/List?type=347
  權限菜单 : 按揭须知 路徑 : AppArticle/List?type=350
  權限菜单 : 市况速递 路徑 : AppArticle/List?type=353
  權限菜单 : 按揭新闻  路徑 : AppArticle/List?type=356
  權限菜单 : 按揭流程 路徑 : AppArticle/List?type=357
  權限菜单 : 按揭简介 路徑 : AppArticle/List?type=358
  權限菜单 : 廣告管理 路徑 : AppArticle/List?type=359
  權限菜单 : 联系我们 路徑 : AppArticle/ContactEdit?Operat=ContactUs
  權限菜单 : 轉介流程 路徑 : AppArticle/List?type=364
  權限菜单 : 员工管理-新增 路徑 : Staff/Add
  權限菜单 : 免責聲明  路徑 : Other/Index?type=Other_Disclaimer
  權限菜单 : 使用條款 路徑 : Other/Index?type=Other_Terms
  權限菜单 : 樓盤天書 路徑 : EstatesBook/BookIndex
  權限菜单 : 活动介绍 路徑 : Article/GetList?type=HD
  權限菜单 : 活动介绍删除 路徑 : Activities/Delete
  權限菜单 : 橫琴分析 路徑 : Article/GetList?type=HQ
  權限菜单 : 修改橫琴分析 路徑 : Article/Edit?type=HQ
  權限菜单 : 新增橫琴分析 路徑 : Article/Add?type=HQ
  權限菜单 : 平均呎价图 路徑 : BoomIndex/AvgPic
  權限菜单 : 橫琴分析2 路徑 : Article/GetList?type=HQ
  權限菜单 : 活動報名 路徑 : Registration/GetList
  權限菜单 : 配寘項 路徑 : File/FileList
  權限菜单 : PDF配寘 路徑 : File/PDFUpload
  權限菜单 : Url配寘 路徑 : File/PathConfig
  權限菜单 : 預約睇樓 路徑 : Reserve/Index
  權限菜单 : 網上放盤 路徑 : Online/Index
  權限菜单 : 财政局成交导入 路徑 : TransDataFinance/FinanzamtImport
  權限菜单 : 财政局成交数据 路徑 : TransDataFinance/FinanzamtList
  權限菜单 : 銀行公告 路徑 : AppArticle/List?type=398
``` 
```bash
頁面路由
首頁 路由地址: /
筍盤推介 
--澳門區-住宅
--氹仔區-住宅
--工商舖-工商
--批量導入数据
焦點新盤
--澳門區
--氹仔區
--東方明珠區
--工商鋪
--香港
--大陸
--橫琴區
--官网首页显示
--預約睇樓
數據分析
--景氣指數
--平均呎价图
市場分析
--
```



Copyright (c) 2017-present PanJiaChen
