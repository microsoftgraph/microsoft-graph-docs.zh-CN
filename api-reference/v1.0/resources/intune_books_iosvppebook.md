# <a name="iosvppebook-resource-type"></a>iosVppEBook 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 iOS Vpp eBook的属性的类。

继承自 [managedEBook](../resources/intune_books_managedebook.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List iosVppEBooks](../api/intune_books_iosvppebook_list.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md) 集合|列出 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象的属性和关系。|
|[Get iosVppEBook](../api/intune_books_iosvppebook_get.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|读取 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象的属性和关系。|
|[Create iosVppEBook](../api/intune_books_iosvppebook_create.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|创建新的 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象。|
|[Delete iosVppEBook](../api/intune_books_iosvppebook_delete.md)|无|删除 [iosVppEBook](../resources/intune_books_iosvppebook.md)。|
|[Update iosVppEBook](../api/intune_books_iosvppebook_update.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|更新 [iosVppEBook](../resources/intune_books_iosvppebook.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|实体的键。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|displayName|字符串|电子书的名称。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|说明|字符串|说明。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|发布服务器|字符串|发布者。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|publishedDateTime|DateTimeOffset|电子书的发布日期和时间。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|largeCover|[mimeContent](../resources/intune_shared_mimecontent.md)|书籍封面。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|createdDateTime|DateTimeOffset|电子书文件的创建日期和时间。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改电子书的日期和时间。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|informationUrl|字符串|详细信息 Url。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|privacyInformationUrl|字符串|隐私声明 Url。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|vppTokenId|Guid|Vpp 令牌 ID。|
|appleId|字符串|与 Vpp 令牌关联的 Apple ID。|
|vppOrganizationName|字符串|Vpp 令牌的组织名称。|
|genres|String 集合|流派。|
|language|字符串|语言。|
|seller|字符串|经销商。|
|totalLicenseCount|Int32|许可证总数。|
|usedLicenseCount|Int32|使用的许可证数。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 集合|此电子书的作业列表。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|移动应用安装摘要。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合|此电子书的安装状态列表。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|
|userStateSummary|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 集合|此电子书的安装状态列表。 继承自 [managedEBook](../resources/intune_books_managedebook.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedEBook",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```








