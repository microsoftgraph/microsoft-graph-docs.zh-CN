---
title: accessReviewScope 资源类型
description: 表示需要在访问评审中审阅的实体。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99e13b08a08f81294588b1eceee09dca888b362f
ms.sourcegitcommit: 1e9a53e7b8e67349288f5cfbabe8355de83817b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2021
ms.locfileid: "58366615"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

**accessReviewScope** 定义在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中检查的实体。 它是由 accessReviewQueryScope、principalResourceMembershipsScope 和[accessReviewReviewerScope](accessreviewreviewerscope.md)继承的抽象类型。 [](accessreviewqueryscope.md) [](principalresourcemembershipsscope.md) 

有关[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 scope 属性，请参阅[accessReviewQueryScope](accessreviewqueryscope.md)和[principalResourceMembershipsScope](principalresourcemembershipsscope.md)。 

有关 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 **reviewers** 属性，请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。

强烈建议所有类型指定作用域中的 OData 类型，但对于[principalResourceMembershipsScope](principalresourcemembershipsscope.md)和[accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)是必需的。 

## <a name="properties"></a>属性
无。


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope"
}
```
