---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: non-product-specific
author: abheek-das
ms.openlocfilehash: 9a45cdff2bfdf1832400d6a563f2d7b1d64792de
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176614"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>multiValueLegacyExtendedProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

包含值集合的扩展属性。

有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | 支持的资源实例：[邮件](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、[contactFolder](../resources/contactfolder.md)、[Outlook任务](../resources/outlooktask.md)或[Outlook任务文件夹](../resources/outlooktaskfolder.md)。 请注意，不支持 [post](../resources/post.md) 组。 | 在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。 |
|[获取](../api/multivaluelegacyextendedproperty-get.md) |支持的资源实例 ([消息](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系](../resources/contact.md)[人、contactFolder](../resources/contactfolder.md)、[Outlook任务](../resources/outlooktask.md)、[Outlook任务文件夹](../resources/outlooktaskfolder.md)或组[后) ](../resources/post.md)使用 [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 对象展开。 |使用 `$expand` 获取具有扩展属性的资源实例。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|属性标识符。只读。|
|value|string collection|属性值的集合。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


