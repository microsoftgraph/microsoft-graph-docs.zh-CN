---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: bf082da6c628c5b4f4ef969ced3f4f50ebf2f65f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849156"
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
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | 受支持的资源实例 [：message](../resources/message.md) [、mailFolder](../resources/mailfolder.md) [、event](../resources/event.md) [、calendar](../resources/calendar.md) [、contact](../resources/contact.md) [、contactFolder](../resources/contactfolder.md) [、Outlook 任务](../resources/outlooktask.md)或 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)。 请注意，不支持 [post](../resources/post.md) 组。 | 在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。 |
|[获取](../api/multivaluelegacyextendedproperty-get.md) |受支持的资源 ([邮件](../resources/message.md)[、mailFolder](../resources/mailfolder.md) [、event](../resources/event.md) [、calendar](../resources/calendar.md) [、contact 、contactFolder](../resources/contactfolder.md) [、Outlook 任务](../resources/outlooktask.md)[、Outlook 任务](../resources/outlooktaskfolder.md)文件夹或[使用](../resources/post.md) [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)对象扩展) 的组帖子。 [contact](../resources/contact.md) |使用 `$expand` 获取具有扩展属性的资源实例。|

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
