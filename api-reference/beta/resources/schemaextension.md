---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a2f58ba623f521766b446b13241cf50aaabd78e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933594"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>schemaExtension 资源类型（架构扩展）

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 

以下资源类型支持架构扩展：

 - [administrativeUnit](administrativeunit.md)
 - [联系人](contact.md)
 - [设备](device.md)
 - 用户或 Office 365 组日历上的[事件](event.md)。
 - Office 365 组的[帖子](post.md)
 - [组](group.md)
 - [邮件](message.md) 
 - [组织](organization.md)
 - [用户](user.md)

请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create](../api/schemaextension-post-schemaextensions.md) | schemaExtension |创建架构扩展定义。|
|[List](../api/schemaextension-list.md) | schemaExtension |列出 avaialbe schemaExtension 定义和及其属性。|
|[Get](../api/schemaextension-get.md) | schemaExtension |读取特定的 schemaExtension 定义的属性。|
|[Update](../api/schemaextension-update.md) | schemaExtension   |更新 schemaExtension 定义。 |
|[Delete](../api/schemaextension-delete.md) | 无 |删除 schemaExtension 定义。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|架构扩展的说明。|
|id|String|架构扩展定义的唯一标识符。 <br>你可以使用下面两种方法之一分配值： <ul><li>连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </li><li>提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</li></ul>此属性一旦创建，便无法更改。 |
|owner|String|属于架构扩展的所有者的应用程序的 `appId`。 可在创建时提供此属性以设置所有者。  如果未提供，则会将调用应用程序的 `appId` 设置为所有者。 在任一情况下，已登录用户均必须是应用程序的所有者。 设置后，此属性为只读，且无法更改。|
|properties|[extensionSchemaProperty](extensionschemaproperty.md) 集合|构成架构扩展定义的属性名称和类型的集合。|
|status|字符串|架构扩展的生命周期状态。可能的值为 **InDevelopment**、**Available** 和 **Deprecated**。创建后将自动设置为 **InDevelopment**。[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。|
|targetTypes|String collection|架构扩展适用的支持扩展的 Microsoft Graph 类型集。 从**administrativeUnit**、**联系人**、**设备**、**事件**、**组**、**消息**、**组织**、**发布**或**用户**选择。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
