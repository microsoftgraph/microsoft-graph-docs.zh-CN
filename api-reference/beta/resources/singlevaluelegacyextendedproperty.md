---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: 51a42661ea3a19ea8e82ba78115bfa5290d99d15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857412"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>singleValueLegacyExtendedProperty 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含单个值的扩展属性。 

有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | 支持的资源实例：[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)中，或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)，但不是组[发布](../resources/post.md)。 | 在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。 |
|[获取](../api/singlevaluelegacyextendedproperty-get.md) |一项或者 （[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)或组[发布](../resources/post.md)），支持的资源实例的集合或展开[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)对象为一个此类的实例。 |使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ID|string|属性标识符。只读。|
|value|string|属性值。|

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
