---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 url。  例如, 在创建新的 Office 365 组时, 还会创建其他资源作为 Office 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Office 365 组资源的详细信息 (包括其关联的资源 url) 现在可以使用组资源类型中的*终结点*导航进行读取。 这样, 应用程序可以了解这些资源, 甚至可以在自己的体验中嵌入资源 URL 体验。 '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542939"
---
# <a name="endpoint-resource-type"></a>终结点资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

终结点表示与实体相关联的资源的 url。  例如, 在创建新的 Office 365 组时, 还会创建其他资源作为 Office 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Office 365 组资源的详细信息 (包括其关联的资源 url) 现在可以使用组资源类型中的*终结点*导航进行读取。 这样, 应用程序可以了解这些资源, 甚至可以在自己的体验中嵌入资源 URL 体验。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List endpoints](../api/group-list-endpoints.md) |[Endpoint](endpoint.md) 集合| 获取 endpoint 对象集合。 |
|[Get endpoint](../api/endpoint-get.md) | [终结点](endpoint.md) |读取 endpoint 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| 性能     | String  | 介绍与此资源相关联的功能。 (例如, 邮件、对话等) 不可为 null。 只读。 |
| id             | String  | 终结点的唯一标识符;主键. 不可为 null。 只读。|
| providerId     | String  | 发布基础服务的应用程序 id。 不可为 null。 只读。|
| providerName   | String  | 发布基础服务的名称。 只读。|
| providerResourceId|String| 对于 Office 365 组, 此设置为资源的已知名称 (例如, FeedURL 等)。 不可为 null。 只读。|
| url            | String  | 已发布资源的 URL。 不可为 null。 只读。|

## <a name="relationships"></a>关系

无。


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
