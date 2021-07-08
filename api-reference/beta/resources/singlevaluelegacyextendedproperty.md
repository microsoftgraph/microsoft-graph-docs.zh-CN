---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 578b2792a815dd0c7cd5dad4fc77d9c96319045a
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334582"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>singleValueLegacyExtendedProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

包含单个值的扩展属性。

有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | [](../resources/post.md)受支持的资源实例：message、mailFolder、event、calendar、contact、contactFolder、Outlook [](../resources/event.md) [](../resources/mailfolder.md) [task](../resources/outlooktask.md)或 Outlook [task folder](../resources/outlooktaskfolder.md)，但不是组 post 。 [](../resources/message.md) [](../resources/calendar.md) [](../resources/contact.md) [](../resources/contactfolder.md) | 在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。 |
|[获取](../api/singlevaluelegacyextendedproperty-get.md) |支持的资源实例 ([](../resources/message.md)message、mailFolder、event、calendar、contact、contactFolder、Outlook [](../resources/contactfolder.md) [](../resources/contact.md) [](../resources/mailfolder.md) [](../resources/event.md) [task、Outlook](../resources/outlooktask.md) [task folder](../resources/outlooktaskfolder.md)或 group [post](../resources/post.md)) 或一个此类实例（使用[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)对象扩展）的一个或一个集合。 [](../resources/calendar.md) |使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|属性标识符。只读。|
|value|string|属性值。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


