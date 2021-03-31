---
title: accessReviewInstanceDecisionItemTarget 资源类型
description: '表示作为用户目标或服务主体目标的审阅目标。 '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c49af4f136e860edbfbcc635b7fc44e67814117c
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469218"
---
# <a name="accessreviewinstancedecisionitemtarget-resource-type"></a>accessReviewInstanceDecisionItemTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示不同类型的审阅目标的基类，每个基类都有其自己的特定属性。 支持的目标类型包括 [：accessReviewInstanceDecisionItemUserTarget](accessreviewinstancedecisionitemusertarget.md) 和 [accessReviewInstanceDecisionItemServicePrincipalTarget](accessreviewinstancedecisionitemserviceprincipaltarget.md)。

## <a name="properties"></a>属性
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemTarget"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItemTarget resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
