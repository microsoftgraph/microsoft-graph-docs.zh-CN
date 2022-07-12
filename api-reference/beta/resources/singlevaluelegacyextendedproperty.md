---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
author: abheek-das
ms.openlocfilehash: 9f87c03e6a2d61fef478eed5554fc3a2d1e2de00
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736690"
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
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | 支持的资源实例： [邮件](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [事件](../resources/event.md)、 [日历](../resources/calendar.md)、 [联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)或 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)，但不是组 [帖子](../resources/post.md)。 | 在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。 |
|[获取](../api/singlevaluelegacyextendedproperty-get.md) |一个或一个受支持的资源实例集合 ([邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系](../resources/contact.md)[人、contactFolder](../resources/contactfolder.md)、[Outlook 任务](../resources/outlooktask.md)、[Outlook 任务文件夹](../resources/outlooktaskfolder.md)或组[后](../resources/post.md)) ，或者一个使用[单一ValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 对象展开的此类实例。 |使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。|

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


