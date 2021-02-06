---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 1733aa15f6989aaef1bb2c80d469f47d6ad86e2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136540"
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
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | 受支持的资源实例： [邮件](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [事件](../resources/event.md)、 [日历](../resources/calendar.md)、 [联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook](../resources/outlooktask.md)任务或 Outlook 任务 [文件夹](../resources/outlooktaskfolder.md)， 但不是组 [帖子](../resources/post.md)。 | 在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。 |
|[获取](../api/singlevaluelegacyextendedproperty-get.md) |一个或一个受支持的资源实例 ([message，](../resources/message.md) [mailFolder，](../resources/mailfolder.md) [event，](../resources/event.md) [calendar，](../resources/calendar.md) [contact，](../resources/contact.md) [contactFolder，](../resources/contactfolder.md) [Outlook task，](../resources/outlooktask.md) [Outlook task folder，](../resources/outlooktaskfolder.md)or group [post](../resources/post.md)) ， or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object. |使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。|

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


