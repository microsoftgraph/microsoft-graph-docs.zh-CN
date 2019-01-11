---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 '
localization_priority: Normal
ms.openlocfilehash: 5a342bee0a1918eb142542693198173239d1b3c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871280"
---
# <a name="endpoint-resource-type"></a>终结点资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出终结点](../api/group-list-endpoints.md) |[终结点](endpoint.md)集合| 获取一个终结点对象集合。 |
|[获取终结点](../api/endpoint-get.md) | [终结点](endpoint.md) |读取属性和终结点对象的关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
| 功能     | 字符串  | 介绍与此资源相关联的功能。 （如邮件、 对话等） 不可为空。 此为只读属性。 |
| id             | 字符串  | 终结点; 的唯一标识符键。 不可为 null。 只读。|
| providerId     | 字符串  | 基础服务发布的应用程序 id。 不可为 null。 只读。|
| providerName   | 字符串  | 发布基础服务的名称。 此为只读属性。|
| providerResourceId|字符串| Office 365 组，这是设置为资源 （例如 Yammer.FeedURL 等。） 的已知名称。 不可为 null。 只读。|
| uri            | 字符串  | 已发布的资源的 URL。 不可为 null。 只读。|

## <a name="relationships"></a>Relationships

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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
