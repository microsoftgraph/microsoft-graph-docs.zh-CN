---
title: connectorGroup 资源类型
description: 表示应用程序代理连接器组。
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: df3a80c6dfd4004daccfe33045c8775c2e2e6e48
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958806"
---
# <a name="connectorgroup-resource-type"></a>connectorGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

每个 [Azure AD 应用程序代理](https://aka.ms/whyappproxy) 连接器始终是连接器组的一部分。 属于同一连接器组的所有连接器都充当高可用性和负载平衡的单独单元。 如果未创建连接器组，则所有连接器都将是默认组的一部分。 使用应用程序代理配置应用程序时，还必须指定要为其分配应用程序的连接器组。

创建连接器组后，可以使用添加连接器将连接器添加或移动到 [连接器组](../api/connectorgroup-post-members.md)。 您还可以使用 ["添加应用程序](../api/connectorgroup-post-applications.md) "将应用程序分配给连接器组。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 connectorGroup](../api/connectorgroup-list.md) |[connectorGroup](connectorgroup.md) 集合 | 检索 connectorGroup 对象的列表。 |
|[Create connectorGroup](../api/connectorgroup-post.md) |[connectorGroup](connectorgroup.md) 集合 | 创建 connectorGroup 对象。 |
|[Get connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | 读取 connectorGroup 对象的属性和关系。 |
|[Update connectorGroup](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| 更新 connectorGroup 对象。 |
|[Delete connectorGroup](../api/connectorgroup-delete.md) | 无 | 删除 connectorGroup 对象。 必须先从 connectorGroup 中删除所有连接器，然后才能删除 connectorGroup。 |
|[List members](../api/connectorgroup-list-members.md) |[连接器](connector.md) 集合| 获取连接器对象集合。 |
|[列出应用程序](../api/connectorgroup-list-applications.md) |[application](application.md) 集合| 获取与 connectorGroup 关联的应用程序对象集合。 |
|[添加应用程序](../api/connectorgroup-post-applications.md) |[application](application.md)| 通过发布到应用程序集合将应用程序与 connectorGroup 关联。 |
|[Add connector](../api/connectorgroup-post-members.md) |[connector](connector.md)| 通过发布到 connectorGroup 集合将连接器添加到 connectorGroup。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|connectorGroupType|connectorGroupType| 指示混合代理的类型。 此预设置由系统设置。 可能的值是 `applicationProxy` ：。 只读。 |
|id|string| 此 connectorGroup 的唯一标识符。 只读。 |
|isDefault|boolean| 指示 connectorGroup 是否默认为 connectorGroup。 只有一个连接器组可以是默认的 connectorGroup，这由系统预先设置。 只读。 |
|name|string| 与 connectorGroup 关联的名称。 |
|region|connectorGroupRegion| connectorGroup 分配到的区域，并将优化其流量。 只有未向 connectorGroup **分配连接器** 或应用程序时，才能设置此区域。 可能的值包括：北美 `nam` () 、 (for Europe  `eur` `aus`) 、 (for Australia `asia`) 、 (for Asia `ind`) 、 (for India) `unknownFutureValue` 和 。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|应用程序|[application](application.md) 集合| 只读。 可为 Null。|
|members|[连接器](connector.md) 集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



