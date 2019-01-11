---
title: connectorGroup 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 211efe5d8caae57457a6a5cc4fa95d145cd176f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823189"
---
# <a name="connectorgroup-resource-type"></a>connectorGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |读取属性和 connectorGroup 对象的关系。|
|[创建应用程序](../api/connectorgroup-post-applications.md) |[application](application.md)| 将应用程序关联连接器组与发布到应用程序集合。|
|[应用程序列表](../api/connectorgroup-list-applications.md) |[应用程序](application.md)集合| 获取关联的应用程序对象集合。|
|[创建连接器](../api/connectorgroup-post-members.md) |[连接器](connector.md)| 通过投递到 members 集合添加到组连接器的连接器。|
|[列出成员](../api/connectorgroup-list-members.md) |[连接器](connector.md)集合| 获取一个连接器对象集合。|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |更新 connectorGroup 对象。 |
|[删除](../api/connectorgroup-delete.md) | 无 |删除 connectorGroup 对象。 可以删除连接器组之前必须删除所有连接线。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|connectorGroupType|string| 将使用与组的连接器的类型。 可能的值为： `applicationProxy`。|
|id|字符串| ConnectorGroup 对象 id|
|isDefault|布尔| 指示 connectorGroup 是默认连接器组。 仅限单个连接器组可以是默认 connectorGroup 并且由系统设置。|
|name|字符串| 与 connectorGroup 关联的名称。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|应用程序|[应用程序](application.md)集合| 只读。可为 NULL。|
|members|[连接器](connector.md)集合| 只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
