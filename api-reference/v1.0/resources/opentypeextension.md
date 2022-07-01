---
title: openTypeExtension 资源类型（开放扩展）
description: 借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。
ms.localizationpriority: high
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: d8d0e4ce76965205a1f1b3340d1e468f482b69b1
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556260"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension 资源类型（开放扩展）

命名空间：microsoft.graph

表示开放扩展（以前称为 Office 365 数据扩展），这是一种 [可扩展性选项](/graph/extensibility-overview)，提供一种简单的方法，可直接将非类型化属性添加到 Microsoft Graph 中的资源。

添加到资源的任何打开扩展都显示在 **扩展** 导航属性中。 每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。 一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖 _用户自己的域_。例如，`com.contoso.ContactInfo`。 **请勿** 在扩展名称中使用 Microsoft 域（`com.microsoft` 或 `com.onmicrosoft`）。

派生自 [扩展](extension.md) 抽象类型。

以下资源支持开放扩展。

+ [user](/graph/api/resources/user)
+ [group](/graph/api/resources/group)
<!--+ [administrativeUnit](/graph/api/resources/administrativeunit)-->
+ [联系人](/graph/api/resources/contact)
+ [设备](/graph/api/resources/device)
+ 用户日历和组日历的 [事件](/graph/api/resources/event)
+ [邮件](/graph/api/resources/message)
+ [组织](/graph/api/resources/organization)
+ [帖子](/graph/api/resources/post)
+ [todoTask](todotask.md) 
+ [todoTaskList](todotasklist.md)

> **注意：** \* 由于现有的服务限制，代理无法在共享邮箱日历中创建已追加开放扩展的事件。 尝试这样做将导致 `ErrorAccessDenied` 响应。

有关 Microsoft Graph 扩展性（包括开放扩展的限制）的详细信息，请参阅 [使用扩展向资源添加自定义属性](/graph/extensibility-overview) ，以及 [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)。

### <a name="outlook-specific-considerations"></a>Outlook 特定注意事项

Outlook 资源（事件、邮件或个人联系人）上存在每个开放扩展均存储在 [MAPI 命名属性](/office/client-developer/outlook/mapi/mapi-named-properties)中。 为 Outlook 创建开放扩展时，请考虑 MAPI 命名属性为用户邮箱中的有限资源。 当用户的命名属性配额用尽后，无法再为该用户创建任何其他命名属性。 这可能会导致依赖命名属性工作的客户端中出现异常行为。

在 Outlook 资源中创建开放扩展时，请遵循以下指导原则：

- 创建所需的最少数量的扩展。 大多数应用程序只需要一个扩展。 扩展未设定定义的属性或结构，因此，可以在一个扩展中存储多个值。
- 避免以可变方式命名扩展，如基于用户输入等。 每次使用用户邮箱中先前未使用过的新名称创建开放扩展时，将会创建新的 MAP 命名属性。 删除扩展不会删除命名属性。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>使用开放扩展（针对 Outlook 资源）或扩展属性

开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。但如果需要访问尚未通过 [Microsoft Graph API 元数据](/graph/traverse-the-graph#microsoft-graph-api-metadata) 公开的 Outlook MAPI 属性的自定义数据，则可以使用 [扩展属性及其 REST API](extended-properties-overview.md)。要确认元数据公开了哪些属性，请访问 https://graph.microsoft.com/v1.0/$metadata。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[创建](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](../resources/opentypeextension.md)（在现有资源实例中），或新的 [todoTask](todotask.md)、[todotasklist](todotasklist.md)[联系人](contact.md)、[事件](event.md)、[消息](message.md)、[帖子](post.md)、[todoTask](todotask.md)或包含 openTypeExtension 对象的 [todoTaskList](todotasklist.md)。 | 在现有的或新的资源实例中创建 openTypeExtension 对象。|
|[获取](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |读取 openTypeExtension 对象的属性和关系。|
|[更新](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |更新 openTypeExtension 对象。 |
|[删除](../api/opentypeextension-delete.md) | 无 |删除 openTypeExtension 对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|extensionName|String|开放类型数据扩展的唯一文本标识符。必需。|
|id|String| 连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。|


## <a name="relationships"></a>关系

无


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

## <a name="see-also"></a>另请参阅

+ [使用扩展向资源添加自定义属性](/graph/extensibility-overview)
+ [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
