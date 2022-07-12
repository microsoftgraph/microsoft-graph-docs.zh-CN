---
author: mohitpcad
title: 组资源类型
doc_type: resourcePageType
description: 表示术语存储中使用的组。
ms.localizationpriority: medium
ms.prod: taxonomy
ms.openlocfilehash: 3bd7f818cf9e38dcffcba9fac0c93b248d1d10d9
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732679"
---
# <a name="group-resource-type"></a>组资源类型

命名空间：microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


表示术语 [存储](../resources/termstore-store.md)中使用的组。 组是包含其下的集合的逻辑层次结构。 

继承自 [entity](../resources/entity.md)。


## <a name="methods"></a>Methods

| 方法                                                   | 返回类型       |    说明|
|:---------------------------------------------------------|:------------------|:---------------------|
| [创建组](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | 在术语 [存储]中创建组。|
| [Get group](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | 检索术语 [存储]中组的数据。|
| [删除组](../api/termstore-group-delete.md)                     | 无 |  删除术语 [存储]中的组。|

## <a name="properties"></a>属性

| 属性             | 类型               | 说明|
|:---------------------|:-------------------|:------------------------------------|
| createdDateTime      | DateTimeOffset     | 组创建的日期和时间。 只读。|
| 说明          | string             | 提供术语使用情况的详细信息的说明。|
| id                   | string             | 组的唯一标识符。 只读。|
| displayName          | string             | 组的名称。|
| scope                | string              | 返回组的类型。 可取值为：`global`、`system` 和 `siteCollection`。|
| parentSiteId         | string             | 此组的父站点的 ID。|

## <a name="relationships"></a>关系
| 关系       | 类型                        | 说明|
|:-------------------|:----------------------------|:--------------------------|
| 集           | [microsoft.graph.termStore.set][] 集合 | 术语 [存储]区中组下的所有集。|

## <a name="json-representation"></a>JSON 表示形式

下面是 **组** 资源的 JSON 表示形式。
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
  "parentSiteId" : "string"
}
```



[identitySet]: identitySet.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[商店]: ../resources/termstore-store.md
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
    "Resources/termStore.group&quot;: &quot;#"
  },
  "suppressions": []
}
-->


