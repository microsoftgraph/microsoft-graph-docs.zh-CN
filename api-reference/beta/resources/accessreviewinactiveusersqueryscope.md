---
title: accessReviewInactiveUsersQueryScope 资源类型
description: 一种 accessReviewQueryScope 类型，只允许在访问评审范围内选择非活动用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 80d415125679ddbb44a08fe75f33b115e4ba1f04
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579744"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>accessReviewInactiveUsersQueryScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

一种 [accessReviewQueryScope](../resources/accessreviewqueryscope.md) 类型，只允许在访问评审范围内选择非活动用户。 不活动持续时间根据[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 settings 属性中定义的访问评审实例的开始日期，根据用户的上次登录日期计算。

继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inactiveDuration|期限|定义不活动持续时间。 与访问评审实例的开始日期相比，不活动基于用户的最后登录日期。 如果未指定此属性，则为其分配默认值 `PT0S` 。|
|查询|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|
|queryRoot|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|
|queryType|String|继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。|

还必须使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。 有关使用 **accessReviewInactiveUsersQueryScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 

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
