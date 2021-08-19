---
title: accessReviewScope 资源类型
description: '在 Azure AD 访问评审功能中，表示将在访问 `accessReviewScope` 评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 21f21d3a3d7ca4d369493c6c5028185bdbdb0e20
ms.sourcegitcommit: 1e9a53e7b8e67349288f5cfbabe8355de83817b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2021
ms.locfileid: "58367287"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

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
