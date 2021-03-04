---
title: 标记资源类型
description: 表示电子数据展示标记，用于在审阅期间标记文档以分隔响应和非响应内容
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: dee53c5a7d8320822101addcf5764420456e703f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446655"
---
# <a name="tag-resource-type"></a>标记资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示电子数据展示标记，用于在审阅过程中标记文档，以分隔响应和非响应内容。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列表标记](../api/ediscovery-case-list-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|获取标记对象 **及其** 属性的列表。|
|[创建标记](../api/ediscovery-case-post-tags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|创建新的 **标记** 对象。|
|[获取标记](../api/ediscovery-tag-get.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|读取标记对象 **的属性** 和关系。|
|[更新标记](../api/ediscovery-tag-update.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|更新 **标记对象的属性** 。|
|[删除标记](../api/ediscovery-tag-delete.md)|无|删除 **标记** 对象。|
|[asHierarchy](../api/ediscovery-tag-ashierarchy.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|列出所有标记，包括其层次结构。|
|[列出 childTags](../api/ediscovery-tag-childtags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|获取与 **标记关联的** 子标记对象列表。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|childSelectability|[microsoft.graph.ediscovery.childSelectability](../resources/ediscovery-tag.md#childselectability-values)|指示单个或多个子标记是否可以与文档关联。 可取值为：`One`、`Many`。  此值控制 UX 是作为复选框还是单选按钮组显示标记。|
|createdBy|[identitySet](../resources/identityset.md)|创建标记的用户。|
|说明|String|标记的说明。|
|displayName|String|标记的显示名称。|
|id|String|标记的唯一标识符。|
|lastModifiedDateTime|DateTimeOffset|上次修改标记的日期和时间。|

### <a name="childselectability-values"></a>childSelectability 值

|成员|说明|
|:----|-----------|
|一个|只能选择一个子级。 这与显示具有单选按钮的标记的 UI 相对应。|
|许多|可以选择零个或多个子级。 这与显示带复选框的标记的 UI 相对应。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|childTags|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合|返回标记的子级标记。|
|父级|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|返回指定标记的父标记。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
