---
title: accessReviewScope 资源类型
description: 表示需要在访问评审中查看的实体。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f14589faad21b586fb3dcc2c6f8b16be9da84f03
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698427"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

**accessReviewScope** 定义 [在 accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 中评审的实体。 它是一种抽象类型，由 [accessReviewQueryScope](accessreviewqueryscope.md)、 [principalResourceMembershipsScope](principalresourcemembershipsscope.md) 和 [accessReviewReviewerScope](accessreviewreviewerscope.md) 继承。 

有关 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上 **的作用域** 属性，请参阅 [accessReviewQueryScope](accessreviewqueryscope.md) 和 [principalResourceMembershipsScope](principalresourcemembershipsscope.md)。

有关 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上的 **审阅者** 属性，请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。

对于所有类型，强烈建议在 **范围内** 指定 OData 类型，但 [principalResourceMembershipsScope](principalresourcemembershipsscope.md) 和 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md) 需要此类型。

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
