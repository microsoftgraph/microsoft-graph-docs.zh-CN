---
author: vishriv
title: 组资源类型
doc_type: resourcePageType
description: 表示术语库中使用的组。
localization_priority: Normal
ms.prod: taxonomy
ms.openlocfilehash: a73cd750ffbfe8487b67acbf49c05432b3e46ec3
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514964"
---
# <a name="group-resource-type"></a>组资源类型

命名空间：microsoft.graph.termStore


表示在术语库中使用的 [组](../resources/termstore-store.md)。 组是逻辑层次结构，其中包含其下的集合。 

继承自 [实体](../resources/entity.md)。


## <a name="methods"></a>方法

| 方法                                                   | 返回类型       |    说明      |
|:---------------------------------------------------------|:------------------|:---------------------
| [创建组](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | 在术语库创建 [组]。 |
| [Get group](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | 检索术语库中的组 [数据]。 |
| [删除组](../api/termstore-group-delete.md)                     | 无 |  删除术语库中的 [组]。 |

## <a name="properties"></a>属性

| 属性             | 类型               | 说明                        |
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | 组创建日期和时间。 只读。 |
| 说明          | string             | 提供有关术语用法的详细信息的说明。 |
| id                   | string             | 组的唯一标识符。 只读。 |
| displayName          | string             | 组的名称。 |
| scope                | string              | 返回组的类型。 可能的值是"global"、"system"和"siteCollection"。 |
| parentSiteId         | string             | 此组的父网站的 ID。 |

## <a name="relationships"></a>关系
| 关系       | 类型                        | 说明              |
|:-------------------|:----------------------------|:--------------------------
| sets           | [microsoft.graph.termStore.set][] 集合 | 术语库 中的组下的所有 [集]。 |

## <a name="json-representation"></a>JSON 表示形式

下面是组资源的 JSON **表示** 形式。
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
[store]: ../resources/termstore-store.md
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


