---
title: accessReviewInactiveUsersQueryScope 资源类型
description: 一种 AccessReviewQueryScope 类型，它只允许在访问评审范围内选择非活动用户。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18790d11628f7e57a349a357e46ba75377e57cc4
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697573"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>accessReviewInactiveUsersQueryScope 资源类型

命名空间：microsoft.graph

一种 [AccessReviewQueryScope](../resources/accessreviewqueryscope.md) 类型，它只允许在访问评审范围内选择非活动用户。 非活动持续时间是根据用户针对 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 的 **settings** 属性中定义的访问评审实例的开始日期计算的。

继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inactiveDuration|持续时间|定义非活动持续时间。 与访问评审实例的开始日期相比，非活动基于用户的最后一个登录日期。 如果未指定此属性，则会为其分配默认值 `PT0S`。|
|查询|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|
|queryRoot|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|
|queryType|字符串|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|

还必须指定具有该值`#microsoft.graph.accessReviewInactiveUsersQueryScope`**的 @odata.type** 属性。 有关使用 **accessReviewInactiveUsersQueryScope** 的作用 **域** 的配置选项的详细信息，请参阅 [使用 Microsoft 图形 API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。

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
