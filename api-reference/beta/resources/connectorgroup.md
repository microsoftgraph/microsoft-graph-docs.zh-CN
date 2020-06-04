---
title: connectorGroup 资源类型
description: 表示应用程序代理 connectorGroup。
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 446dae5e78878ba9648d532d2696b0bfde496601
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556168"
---
# <a name="connectorgroup-resource-type"></a>connectorGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

每个[AZURE AD 应用程序代理](https://aka.ms/whyappproxy)连接器始终是连接器组的一部分。 属于同一连接器组的所有连接器充当高可用性和负载平衡的独立单元。 如果不创建连接器组，则所有连接器都将成为默认组的一部分。 在使用应用程序代理配置应用程序时，还必须指定要向其分配应用程序的连接器组。

创建连接器组之后，可以使用 "[添加连接器](../api/connectorgroup-post-members.md)" 将连接器添加或移动到连接器组。 您还可以使用 "[添加应用程序](../api/connectorgroup-post-applications.md)" 将应用程序分配给连接器组。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 connectorGroup](../api/connectorgroup-list.md) |[connectorGroup](connectorgroup.md)集合 | 检索 connectorGroup 对象的列表。 |
|[获取 connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | 读取 connectorGroup 对象的属性和关系。 |
|[更新 connectorGroup](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| 更新 connectorGroup 对象。 |
|[删除 connectorGroup](../api/connectorgroup-delete.md) | 无 | 删除 connectorGroup 对象。 必须从 connectorGroup 中删除所有连接器，然后才能删除 connectorGroup。 |
|[List members](../api/connectorgroup-list-members.md) |[连接器](connector.md)集合| 获取连接器对象集合。 |
|[列出应用程序](../api/connectorgroup-list-applications.md) |[application](application.md) 集合| 获取与 connectorGroup 相关联的应用程序对象集合。 |
|[添加应用程序](../api/connectorgroup-post-applications.md) |[application](application.md)| 通过发布到应用程序集合，将应用程序与 connectorGroup 相关联。 |
|[添加连接器](../api/connectorgroup-post-members.md) |[连接器](connector.md)| 通过发布到 connectorGroup 集合，将连接器添加到 connectorGroup。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|connectorGroupType|string| 指示混合代理的类型。 此项预设置的系统。 只读。 |
|id|string| 此 connectorGroup 的唯一标识符。 只读。 |
|isDefault|boolean| 指示 connectorGroup 是否为默认的 connectorGroup。 只有一个连接器组可以是默认的 connectorGroup，这是由系统预设置的。 只读。 |
|name|string| 与 connectorGroup 关联的名称。 |
|范围|string| 向其分配 connectorGroup 的区域并将为其优化流量。 仅当未向 connectorGroup 分配**连接器或应用程序**时，才能设置此区域。 可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。 可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|来说|[application](application.md) 集合| 此为只读属性。 可为 Null。|
|members|[连接器](connector.md)集合| 只读。可为空。|

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
