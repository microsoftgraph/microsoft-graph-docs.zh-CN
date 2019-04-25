---
title: connectorGroup 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543390"
---
# <a name="connectorgroup-resource-type"></a>connectorGroup 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |读取 connectorGroup 对象的属性和关系。|
|[创建应用程序](../api/connectorgroup-post-applications.md) |[application](application.md)| 将应用程序与连接器组关联, 方法是发布到应用程序集合。|
|[列出应用程序](../api/connectorgroup-list-applications.md) |[应用程序](application.md)集合| 获取关联的应用程序对象集合。|
|[创建连接器](../api/connectorgroup-post-members.md) |[连接器](connector.md)| 通过发布到 members 集合, 将连接器添加到连接器组。|
|[List members](../api/connectorgroup-list-members.md) |[连接器](connector.md)集合| 获取连接器对象集合。|
|[更新](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |更新 connectorGroup 对象。 |
|[删除](../api/connectorgroup-delete.md) | 无 |删除 connectorGroup 对象。 必须删除所有连接器, 然后才能删除 conector 组。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|connectorGroupType|string| 将与组一起使用的连接器的类型。 可能的值是`applicationProxy`:。|
|id|字符串| connectorGroup 的对象 id|
|isDefault|Boolean| 指示 connectorGroup 是否为默认的连接器组。 只有一个连接器组可以是默认的 connectorGroup, 并由系统进行设置。|
|name|String| 与 connectorGroup 关联的名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|来说|[应用程序](application.md)集合| 只读。 可为 Null。|
|members|[连接器](connector.md)集合| 只读。可为空。|

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
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
