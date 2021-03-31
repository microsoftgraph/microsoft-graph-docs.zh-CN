---
title: accessReviewScope 资源类型
description: '在 Azure AD 访问评审功能中，表示将在访问 `accessReviewScope` 评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04955ba6980dd94995da1610afcc1e33046e4473
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469309"
---
# <a name="accessreviewscope-resource-type"></a>accessReviewScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**accessReviewScope** 定义哪些实体将在 [accessReviewScheduleDefinition 中查看](accessreviewscheduledefinition.md)。 它是由 accessReviewQueryScope、principalResourceMembershipsScope 和[accessReviewReviewerScope](accessreviewreviewerscope.md)继承的抽象类型。 [](accessreviewqueryscope.md) [](principalresourcemembershipsscope.md) 

有关 `scope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 的属性，请参阅 [accessReviewQueryScope](accessreviewqueryscope.md) 和 [principalResourceMembershipsScope](principalresourcemembershipsscope.md)。

有关 `reviewers` [accessReviewScheduleDefinition 的属性，](accessreviewscheduledefinition.md) 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)

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
