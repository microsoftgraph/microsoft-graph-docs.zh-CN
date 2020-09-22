---
title: 终结点资源类型
description: 终结点表示与实体相关联的资源的 Url。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 0bd50176690a9131ef1035d4b21b641d5a2c9b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018569"
---
# <a name="endpoint-resource-type"></a>终结点资源类型

命名空间：microsoft.graph

终结点表示与实体相关联的资源的 Url。  例如，在创建新的 Microsoft 365 组时，还会创建其他资源作为 Microsoft 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Microsoft 365 组资源的详细信息（包括其关联的资源 Url）现在可以使用组资源类型中的 *终结点* 导航进行读取。 这样，应用程序可以了解这些资源，甚至可以在自己的体验中嵌入资源 URL 体验。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List endpoints](../api/group-list-endpoints.md) |[Endpoint](endpoint.md) 集合| 获取 endpoint 对象集合。 |
|[Get endpoint](../api/endpoint-get.md) | [终结点](endpoint.md) |读取 endpoint 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| 性能     | String  | 介绍与此资源相关联的功能。  (，例如邮件、对话等 ) 不可为 null。 只读。 |
| id             | String  | 终结点的唯一标识符;主键. 不可为空。 只读。|
| providerId     | String  | 发布基础服务的应用程序 id。 不可为空。 只读。|
| providerName   | String  | 发布基础服务的名称。 只读。|
| providerResourceId|String| 对于 Microsoft 365 组，它设置为资源的已知名称 (例如，FeedURL 等 ) 。 不可为空。 只读。|
| url            | String  | 已发布资源的 URL。 不可为空。 只读。|

## <a name="relationships"></a>关系

无。


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
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
     "Error: microsoft.graph.servicePrincipal/endpoints:\r\n      Referenced type microsoft.graph.endPoint is not defined in the doc  set! Potential suggestion: microsoft.graph.callRecords.endpoint"
    ]
}
-->

