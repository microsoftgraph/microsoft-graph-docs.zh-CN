---
author: mohitpcad
title: 组资源类型
doc_type: resourcePageType
description: 代表术语库中使用的组。
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 91ad02722bcbddb1d21222381ced7cabc531f3fc
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539161"
---
# <a name="group-resource-type"></a>组资源类型

命名空间： termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


代表术语[库](../resources/termstore-store.md)中使用的组。 组是一个逻辑层次结构，其中包含在其下设置的集合。 

继承自[entity](../resources/entity.md)。


## <a name="methods"></a>方法

| 方法                                                   | 返回类型       |    说明
|:---------------------------------------------------------|:------------------|:---------------------
| [创建组](../api/termstore-group-post.md)                     | [termStore 的组] | 在术语[库]中创建一个组。
| [Get group](../api/termstore-store-get-group.md)                           | [termStore 的组] | 在术语[库]中检索组的数据。
| [删除组](../api/termstore-group-delete.md)                     | 无 |  删除术语[库]中的组。

## <a name="properties"></a>属性

| 属性             | 类型               | 说明
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | 创建组的日期和时间。 只读。
| 说明          | string             | 说明：提供有关术语用法的详细信息。
| id                   | 字符串             | 组的唯一标识符。 只读。
| displayName          | string             | 组的名称。
| scope                | string              | 返回组的类型。 可能的值为 "global"、"system" 和 "siteCollection"。

## <a name="relationships"></a>关系
| 关系       | 类型                        | 说明
|:-------------------|:----------------------------|:--------------------------
| 下例           | [Microsoft termStore][]集合 | 术语[库]中的组下的所有集。

## <a name="json-representation"></a>JSON 表示形式

以下是**组**资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string",  
}
```



[identitySet]: identitySet.md
[termStore 设置]: termstore-set.md
[termStore 的组]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group": "#"
  },
  "suppressions": []
}
-->
