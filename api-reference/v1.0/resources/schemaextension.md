---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
ms.localizationpriority: high
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: 5f0198e7b51a29afe9074efe2d6b2384c4367f6e
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556344"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>schemaExtension 资源类型（架构扩展）

命名空间：microsoft.graph

可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。 自定义数据在扩展资源上作为复杂类型显示。 以下资源类型支持架构扩展：

+ [user](/graph/api/resources/user)
+ [group](/graph/api/resources/group)
+ [administrativeUnit](/graph/api/resources/administrativeunit)
+ [application](/graph/api/resources/application)
+ [联系人](/graph/api/resources/contact)
+ [设备](/graph/api/resources/device)
+ [事件](/graph/api/resources/event) （适用于用户和组日历）
+ [邮件](/graph/api/resources/message)
+ [组织](/graph/api/resources/organization)
+ [帖子](/graph/api/resources/post)
+ [todoTask](/graph/api/resources/todotask)
+ [todoTaskList](/graph/api/resources/todotasklist)

使用此资源和关联的方法来管理 [架构扩展定义](/graph/api/resources/schemaextension)。 要管理扩展资源实例上的架构扩展数据，请使用你用于管理资源实例的同一 REST 请求。 请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。

有关Microsoft Graph扩展性的详细信息，包括架构扩展的限制， [请参阅使用扩展向资源添加自定义属性](/graph/extensibility-overview)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建](../api/schemaextension-post-schemaextensions.md) | [schemaExtension](schemaextension.md) |创建架构扩展定义。|
|[List](../api/schemaextension-list.md) | [schemaExtension](schemaextension.md) |列出可用的 schemaExtension 定义及其属性。|
|[Get](../api/schemaextension-get.md) | [schemaExtension](schemaextension.md) |读取特定的 schemaExtension 定义的属性。|
|[Update](../api/schemaextension-update.md) | [schemaExtension](schemaextension.md) |更新 schemaExtension 定义。 |
|[Delete](../api/schemaextension-delete.md) | 无 |删除 schemaExtension 定义。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|架构扩展的说明。支持`$filter`（`eq`）。|
|id|String|架构扩展定义的唯一标识符。 <br>你可以使用下面两种方法之一分配值： <ul><li>连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </li><li>提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</li></ul>此属性创建后无法更改。支持 `$filter`（`eq`）。**注意：** 我们 **建议 ID 以** A-Z 之间的字母开头，因为查询功能可能限制为以整数开头的 ID。 |
|所有者|String|属于架构扩展的所有者的应用程序的 `appId`。 可在创建时提供此属性以设置所有者。  如果未提供，则会将调用应用程序的 `appId` 设置为所有者。 在任一情况下，已登录用户均必须是应用程序的所有者。 因此，如果使用 Graph 浏览器新建一个架构扩展定义，则 **必须** 提供 owner 属性（以此为例）。 设置后，此属性为只读，且无法更改。 支持 `$filter`（`eq`）。| 
|properties|[extensionSchemaProperty](extensionschemaproperty.md) 集合|构成架构扩展定义的属性名称和类型的集合。|
|status|String|架构扩展的生命周期状态。 可能的状态为 `InDevelopment`、`Available` 和 `Deprecated`。 创建后将自动设置为 `InDevelopment`。 有关可能的状态转换和行为的详细信息，请参阅 [架构扩展生命周期](#schema-extensions-lifecycle)。 支持 `$filter`（`eq`）。|
|targetTypes|String collection|架构扩展适用的支持扩展的 Microsoft Graph 类型集。 从 **administrativeUnit**、 **联系人**、 **设备**、 **事件**、 **组**、 **消息**、 **组织**、 **帖子**、 **todoTask**、 **todoTaskList** 或 **用户** 中进行选择。|

### <a name="schema-extensions-lifecycle"></a>架构扩展生命周期

当应用创建架构扩展定义时，系统会将该应用标记为该架构扩展的所有者。

所有者应用可以在 **状态** 属性上使用 PATCH 操作将扩展转换为生命周期中的不同状态。基于当前状态，所有者应用可以更新或删除扩展。架构扩展的任何更新始终只能累加且不能间断。

|状态 |生命周期状态行为 |
|:-------------|:------------|
| InDevelopment | <ul><li>创建后的初始状态。所有者应用仍然在开发架构扩展。 </li><li>在此状态下，注册所有者应用的同一目录中的任何应用都可以使用此架构定义（如果应用对该资源具有权限）扩展资源实例。 </li><li>对于多租户的所有者应用，只有位于主目录不同目录中的所有者应用实例才能使用此架构定义（如果应用具有该资源的权限）扩展资源实例，或读取扩展数据。 </li><li>只有所有者应用，才能使用增量更改更新扩展定义。 </li><li>只有所有者应用可以删除扩展定义。 </li><li>所有者应用可以将扩展状态从 **开发中** 更改为 **可用**。</li></ul> |
| 可用 | <ul><li>架构扩展可供任意租户中的所有应用使用。 </li><li>在所有者应用将扩展设置为 **“可用**”后，任何应用都可以简单地将自定义数据添加到扩展中指定的那些资源类型的实例（如果应用对该资源具有权限）。 新建实例或更新现有实例时，应用可以分配自定义数据。 </li><li>只有所有者应用，才能使用增量更改更新扩展定义。 任何应用都无法删除这种状态下的扩展定义。 </li><li>所有者应用可以将架构扩展状态从“可用”更改为“已弃用”。</li></ul> |
| 不推荐使用 | <ul><li>架构扩展定义不再可供读取或修改。 </li><li>任何应用都无法查看、更新、添加新属性或删除扩展。 </li><li>但是应用仍可读取、更新或删除现有扩展 _属性值_。 </li></ul> |

> **注意：** 其他开发人员从其他租户创建的架构扩展定义（标记为 `Available`）对所有开发人员可见（通过列出所有架构扩展）。 这不同于仅返回租户特定数据的其他 API。 另一方面，基于架构扩展定义创建的扩展数据是特定于租户的，并且只能由被显式授予权限的应用访问。 

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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

## <a name="see-also"></a>另请参阅

+ [使用扩展向资源添加自定义属性](/graph/extensibility-overview)
+ [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

