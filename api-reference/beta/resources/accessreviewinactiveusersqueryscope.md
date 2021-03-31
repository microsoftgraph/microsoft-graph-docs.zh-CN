---
title: accessReviewInactiveUsersQueryScope 资源类型
description: 一种 accessReviewQueryScope 类型，只允许在访问评审范围内选择非活动用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 51fc61ce186b0346bc065ddc5dfea40158758223
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469748"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>accessReviewInactiveUsersQueryScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

一种 [accessReviewQueryScope](../resources/accessreviewqueryscope.md) 类型，只允许在访问评审范围内选择非活动用户。

继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inactiveDuration|持续时间|定义不活动持续时间的长度。 不活动基于用户的上次登录日期。|
|查询|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|
|queryRoot|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|
|queryType|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|

### <a name="supported-queries-for-accessreviewinactiveuserqueryscope-as-scope"></a>accessReviewInactiveUserQueryScope 作为范围的受支持的查询
[accessReviewScope](../resources/accessreviewscope.md)上支持的相同查询在 accessReviewInactiveUserQueryScope 上也受支持。 以下是查询。 它们作为 `scope` [accessReviewScheduleDefinition 中的 属性受到支持](accessreviewscheduledefinition.md)。

|方案| 查询 |
|--|--|
| 查看分配给组的所有非活动来宾用户 | /groups/{group ID}/transitiveMembers/microsoft.graph.user/？ \$count=true&$filter= (userType eq 'Guest')  |
| 查看分配给组的所有非活动用户 | /groups/{group ID}/transitiveMembers |
| 查看分配给所有组的所有非活动来宾用户 | ./members/microsoft.graph.user/？ \$count=true&$filter= (userType eq 'Guest')  |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
