---
title: accessReviewScope 资源类型
description: 表示需要在访问评审中审阅的实体。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9194d0b07c2b24d37f811c2348ed7b4b1a8498e2f592b6a10d97dc212d180be9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121443"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

**accessReviewScope** 定义哪些实体将在 [accessReviewScheduleDefinition 中查看](accessreviewscheduledefinition.md)。 它是由 accessReviewQueryScope、principalResourceMembershipsScope 和[accessReviewReviewerScope](accessreviewreviewerscope.md)继承的抽象类型。 [](accessreviewqueryscope.md) [](principalresourcemembershipsscope.md) 

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
