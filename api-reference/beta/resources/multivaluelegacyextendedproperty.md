---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 2b0bfa2d8d5da5c3cca9479195a6649e25c8d7e8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810521"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>multiValueLegacyExtendedProperty 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含值集合的扩展属性。

有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | 受支持的资源实例 [： message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [outlook task](../resources/outlooktask.md)或 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)。 请注意，不支持 [post](../resources/post.md) 组。 | 在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。 |
|[获取](../api/multivaluelegacyextendedproperty-get.md) |受支持的资源实例 [ (message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [outlook 任务](../resources/outlooktask.md)、 [outlook 任务文件夹](../resources/outlooktaskfolder.md)或组 [帖子](../resources/post.md)) 使用 [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 对象进行扩展。 |使用 `$expand` 获取具有扩展属性的资源实例。|

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
