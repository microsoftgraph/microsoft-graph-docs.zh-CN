# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension 资源类型（开放扩展）

打开扩展 （之前被称为 Office 365 数据扩展） 提供轻松直接将非类型化的属性添加到 Microsoft Graph 中的资源。

开放扩展由 **openTypeExtension** 资源表示。 添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。 每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。

一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。 请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。

开放扩展示例：[使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)

一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。

|资源 |版本 |
|:---------------|:-------|
| [管理单元](../../beta/resources/administrativeunit.md)  | 仅供预览 |
| [日历事件](event.md) | GA |
| 组[日历事件](event.md) | GA |
| 组对话线程[帖子](post.md) | GA |
| [设备](device.md) | GA |
| [组](group.md) | GA |
| [邮件](message.md) | GA |
| [组织](organization.md) | GA |
| [个人联系人](contact.md) | GA |
| [用户](user.md) | GA |

## <a name="outlook-specific-considerations"></a>特定于 outlook 的注意事项

每个打开的扩展名存在于 Outlook 的资源 （事件、 消息或个人联系人） 存储在[MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)。 为 Outlook 创建打开扩展时，请考虑 MAPI 命名属性是用户的邮箱的有限资源。 在用尽用户的命名的属性配额时，您无法创建该用户的任何多命名的属性。 这会导致出现异常行为依赖于对函数的命名属性的客户端。

打开扩展名创建在 Outlook 资源时，请应用以下准则：

- 创建所需的扩展的最小数目。 大多数应用程序应该要求不多个扩展名。 扩展具有未定义的设置的属性或结构，因此您可以将多个值存储在一个扩展。
- 避免 （例如，基于用户输入等。） 来扩展命名变量的方式。 打开扩展名创建新的名称之前, 的用户的邮箱中未用过的每次创建新的 MAPI 命名属性。 删除扩展不会删除的命名的属性。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>使用打开扩展名 （对于 Outlook 资源） 或扩展的属性

打开扩展是适用于大多数的方案涉及存储和访问自定义数据的建议的解决方案。 但是，您需要通过[Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)访问自定义 Outlook MAPI 属性未已公开的数据，您可以使用[扩展的属性和其 REST API](extended-properties-overview.md)。 您可以验证元数据在公开哪些属性[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>属性

|属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|extensionName|字符串|开放类型开放扩展的唯一文本标识符。必需。|
|id|String| 连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。|

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension_post_opentypeextension.md) | [openTypeExtension](opentypeextension.md)（在现有资源实例中），或包含 openTypeExtension 对象的新 [contact](../resources/contact.md)、[event](../resources/event.md) 或 [message](../resources/message.md)。 | 在现有的或新的资源实例中创建 openTypeExtension 对象。|
|[获取](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |读取 openTypeExtension 对象的属性和关系。|
|[更新](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md) |更新 openTypeExtension 对象。 |
|[删除](../api/opentypeextension_delete.md) | 无 |删除 openTypeExtension 对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
