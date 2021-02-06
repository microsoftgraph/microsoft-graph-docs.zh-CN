---
title: accessReviewReviewerScope 资源类型
description: 代表将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c8a0644699daf7e204226d89bdd6cab6048888d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133488"
---
# <a name="accessreviewreviewerscope-resource-type"></a>accessReviewReviewerScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

accessReviewReviewerScope 定义谁将审阅 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。 这表示为 OData 查询，它允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (，即每个用户都由其经理) 审阅的情况。 若要创建自 (查看自己的访问权限的自) ，请不要在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。


## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | 字符串 | 用于指定审阅者的查询。 有关示例，请参阅表。 |
| queryType | 字符串 | 查询的类型。 示例包括 `MicrosoftGraph` `ARM` 和 。 |
| queryRoot | 字符串 | 在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定了相对查询 (./manager) 是必需的。 |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>AccessReviewReviewerScope 支持的查询

|应用场景| 查询 | queryType | queryRoot |
|--|--|--|--|
| 作为审阅者的组所有者 | /groups/{group id}/owners |MicrosoftGraph||
| 特定用户作为审阅者 | /users/{user id} |MicrosoftGraph||
| 被审阅为审阅者的用户的经理 | ./manager | MicrosoftGraph |决策|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
