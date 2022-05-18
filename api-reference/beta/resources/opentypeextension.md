---
title: openTypeExtension 资源类型（开放扩展）
description: 借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。
ms.localizationpriority: medium
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 476747b9341f0d7b2d5b551809319ccec5edc787
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461399"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension 资源类型（开放扩展）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。
开放扩展由 **openTypeExtension** 资源表示。 添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。  每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。 一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖 _用户自己的域_。例如，`com.contoso.ContactInfo`。 **请勿在** 扩展名中使用 Microsoft 域 (`com.microsoft` 或 `com.onmicrosoft`) 。

开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)

相应版本中的以下资源支持开放扩展 - 正式发布 (/v1.0) 或预览版 (/beta) 。

| 资源 | 版本 |
|---------------|-------|
| [管理单元](administrativeunit.md) | GA |
| [日历事件](event.md) \* | GA |
| 组[日历事件](event.md) | GA |
| 组对话线程[帖子](post.md) | GA |
| [设备](device.md) | GA |
| [组](group.md) | GA |
| [邮件](message.md) | GA |
| [组织](organization.md) | GA |
| [个人联系人](contact.md) | GA |
| [用户](user.md) | GA |
| [任务](basetask.md) | GA |
| [任务列表](basetasklist.md) | GA |

>\***注意：** 由于现有服务限制，委托无法在共享邮箱日历中创建打开的扩展追加事件。 尝试执行此操作将导致 `ErrorAccessDenied` 响应。

## <a name="outlook-specific-considerations"></a>Outlook 特定注意事项

Outlook 资源（事件、邮件或个人联系人）上存在每个开放扩展均存储在 [MAPI 命名属性](/office/client-developer/outlook/mapi/mapi-named-properties)中。 为 Outlook 创建开放扩展时，请考虑 MAPI 命名属性为用户邮箱中的有限资源。 当用户的命名属性配额用尽后，无法再为该用户创建任何其他命名属性。 这可能会导致依赖命名属性工作的客户端中出现异常行为。

在 Outlook 资源中创建开放扩展时，请遵循以下指导原则：

- 创建所需的最少数量的扩展。 大多数应用程序只需要一个扩展。 扩展未设定定义的属性或结构，因此，可以在一个扩展中存储多个值。
- 避免以可变方式命名扩展，如基于用户输入等。 每次使用用户邮箱中先前未使用过的新名称创建开放扩展时，将会创建新的 MAP 命名属性。 删除扩展不会删除命名属性。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>使用开放扩展（针对 Outlook 资源）或扩展属性

开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。 不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](/graph/traverse-the-graph#microsoft-graph-api-metadata)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。 若要确认元数据公开了哪些属性，请访问 https://graph.microsoft.com/v1.0/$metadata。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}
```

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|extensionName|String|开放类型数据扩展的唯一文本标识符。必需。|
|id|String| 连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。|

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[Create](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) (现有资源实例) 或包含 openTypeExtension 对象的新[联系](contact.md)人、[事件](event.md)、[消息](message.md)、[帖子](post.md)、[Task](basetask.md) 或 [TaskList](basetasklist.md)。 | 在现有的或新的资源实例中创建 openTypeExtension 对象。|
|[获取](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |读取 openTypeExtension 对象的属性和关系。|
|[更新](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |更新 openTypeExtension 对象。 |
|[删除](../api/opentypeextension-delete.md) | 无 |删除 openTypeExtension 对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
