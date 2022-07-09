---
title: accessReviewInstanceDecisionItemTarget 资源类型
description: '将评审的目标表示为用户目标或服务主体目标。 '
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 104d8c6c2611721b5c822cb75aef95a5b6145848
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698133"
---
# <a name="accessreviewinstancedecisionitemtarget-resource-type"></a>accessReviewInstanceDecisionItemTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示不同类型的审阅目标的基类，每个目标都有其自己的特定属性。 支持的目标类型为： [accessReviewInstanceDecisionItemUserTarget](accessreviewinstancedecisionitemusertarget.md) 和 [accessReviewInstanceDecisionItemServicePrincipalTarget](accessreviewinstancedecisionitemserviceprincipaltarget.md)。

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
