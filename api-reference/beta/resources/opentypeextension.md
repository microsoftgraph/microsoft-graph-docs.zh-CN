---
title: openTypeExtension 资源类型（开放扩展）
description: 开放扩展 (以前称为 Office 365 数据扩展) 提供了一种简单的方法, 可将非类型化属性直接添加到 Microsoft Graph 中的资源。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568886"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension 资源类型（开放扩展）

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

开放扩展 (以前称为 Office 365 数据扩展) 提供了一种简单的方法, 可将非类型化属性直接添加到 Microsoft Graph 中的资源。
开放扩展由 **openTypeExtension** 资源表示。 添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。  每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。 一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。 请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。

开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)

一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。

| 资源 | 版本 |
|---------------|-------|
| [管理单元](administrativeunit.md)  | 仅供预览 |
| [日历事件](event.md) | GA |
| 组[日历事件](event.md) | GA |
| 组对话线程[帖子](post.md) | GA |
| [设备](device.md) | GA |
| [组](group.md) | GA |
| [邮件](message.md) | GA |
| [组织](organization.md) | GA |
| [个人联系人](contact.md) | GA |
| [用户](user.md) | GA |

## <a name="outlook-specific-considerations"></a>特定于 Outlook 的注意事项

Outlook 资源 (事件、邮件或个人联系人) 上的每个打开的扩展均存储在[MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)中。 为 Outlook 创建开放扩展时, 请考虑 MAPI 命名属性是用户邮箱中的有限资源。 当用户的命名属性配额耗尽时, 不能为该用户创建更多的命名属性。 这可能会导致来自依赖命名属性的客户端的意外行为能够正常运行。

在 Outlook 资源上创建开放扩展时, 请应用以下准则:

- 创建所需的最少分机数。 大多数应用程序不应要求有一个以上的扩展名。 扩展没有任何已定义的属性或结构, 因此您可以将多个值存储在一个扩展中。
- 避免以可变方式命名扩展名 (例如, 基于用户输入等)。 每次使用尚未在用户邮箱中使用的新名称创建一个打开的扩展时, 都会创建一个新的 MAPI 命名属性。 删除扩展不会删除命名属性。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>使用开放扩展 (针对 Outlook 资源) 或扩展属性

开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。 不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。 您可以验证元数据公开[ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)的属性。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
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
|[Post](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md)(在现有资源实例中) 或包含 openTypeExtension 对象的新[联系人](../resources/contact.md)、[事件](../resources/event.md)或[邮件](../resources/message.md)。 | 在现有的或新的资源实例中创建 openTypeExtension 对象。|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
