---
title: accessReviewReviewerScope 资源类型
description: 表示将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68f353b81b6a14292828d82929a0eeac81d67bc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469155"
---
# <a name="accessreviewreviewerscope-resource-type"></a>accessReviewReviewerScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

accessReviewReviewerScope 定义谁将审阅 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。 这表示为 OData 查询，它允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (，即每个用户都由其经理) 审阅的情况。 若要创建自审阅 (用户查看自己的访问权限) ，请不要在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。

继承自 [accessReviewScope](../resources/accessreviewscope.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| 查询 | String | 用于指定审阅者的查询。 有关示例，请参阅表。 |
| queryType | String | 查询的类型。 示例包括 `MicrosoftGraph` `ARM` 和 。 |
| queryRoot | String | 在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。 此属性仅在指定了相对查询 (，即 ./manager) 是必需的。 |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>accessReviewReviewerScope 支持的查询

|方案| 查询 | queryType | queryRoot |
|--|--|--|--|
| 作为审阅者的组所有者 | /groups/{group id}/owners |MicrosoftGraph||
| 作为审阅者的特定用户 | /users/{user id} |MicrosoftGraph||
| 被审阅为审阅者的用户的经理 | ./manager | MicrosoftGraph |决策|
| 自我审阅 | 空列表 (没有审阅者)  | MicrosoftGraph  |


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
