# <a name="managedebook-resource-type"></a>managedEBook 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含托管电子书基属性的抽象类。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedEBooks](../api/intune_books_managedebook_list.md)|[managedEBook](../resources/intune_books_managedebook.md) 集合|列出 [managedEBook](../resources/intune_books_managedebook.md) 对象的属性和关系。|
|[获取 managedEBook](../api/intune_books_managedebook_get.md)|[managedEBook](../resources/intune_books_managedebook.md)|读取 [managedEBook](../resources/intune_books_managedebook.md) 对象的属性和关系。|
|[assign 操作](../api/intune_books_managedebook_assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|displayName|字符串|电子书的名称。|
|description|字符串|说明。|
|publisher|字符串|发布者。|
|publishedDateTime|DateTimeOffset|电子书的发布日期和时间。|
|largeCover|[mimeContent](../resources/intune_shared_mimecontent.md)|书籍封面。|
|createdDateTime|DateTimeOffset|电子书文件的创建日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改电子书的日期和时间。|
|informationUrl|字符串|详细信息 Url。|
|privacyInformationUrl|字符串|隐私声明 Url。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 集合|此电子书的分配列表。|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|移动应用安装摘要。|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合|此电子书的安装状态列表。|
|userStateSummary|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 集合|此电子书的安装状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedEBook"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



