---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512057"
---
# <a name="endpoint-resource-type"></a>终结点资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List endpoints](../api/group-list-endpoints.md) |[Endpoint](endpoint.md) 集合| 获取 endpoint 对象集合。 |
|[Get endpoint](../api/endpoint-get.md) | [终结点](endpoint.md) |读取 endpoint 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| Capability     | String  | 介绍与此资源相关联的功能。 （如邮件、 对话等） 不可为空。 只读。 |
| id             | String  | 终结点; 的唯一标识符键。 不可为 null。 只读。|
| ProviderID     | String  | 基础服务发布的应用程序 id。 不可为 null。 只读。|
| ProviderName   | String  | 发布基础服务的名称。 只读。|
| providerResourceId|String| Office 365 组，这是设置为资源 （例如 Yammer.FeedURL 等。） 的已知名称。 不可为 null。 只读。|
| uri            | String  | 已发布的资源的 URL。 不可为 null。 只读。|

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
