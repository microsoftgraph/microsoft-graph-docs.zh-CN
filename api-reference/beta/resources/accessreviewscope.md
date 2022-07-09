---
title: accessReviewScope 资源类型
description: '在 Azure AD 访问评审功能中 `accessReviewScope` ，表示哪些实体将在访问评审中进行评审。  '
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa4d8dd9db5fa16736552acbed2c9e59592980af
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698105"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
