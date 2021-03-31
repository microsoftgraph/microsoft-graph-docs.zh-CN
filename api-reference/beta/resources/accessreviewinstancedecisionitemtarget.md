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
# <a name="accessreviewinstancedecisionitemtarget-resource-type"></a><span data-ttu-id="3130b-103">accessReviewInstanceDecisionItemTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="3130b-103">accessReviewInstanceDecisionItemTarget resource type</span></span>

<span data-ttu-id="3130b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3130b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="3130b-105">表示不同类型的审阅目标的基类，每个基类都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="3130b-105">Represents a base class for different types of review targets, each one with its own specific properties.</span></span> <span data-ttu-id="3130b-106">支持的目标类型包括 [：accessReviewInstanceDecisionItemUserTarget](accessreviewinstancedecisionitemusertarget.md) 和 [accessReviewInstanceDecisionItemServicePrincipalTarget](accessreviewinstancedecisionitemserviceprincipaltarget.md)。</span><span class="sxs-lookup"><span data-stu-id="3130b-106">The supported target types are: [accessReviewInstanceDecisionItemUserTarget](accessreviewinstancedecisionitemusertarget.md) and [accessReviewInstanceDecisionItemServicePrincipalTarget](accessreviewinstancedecisionitemserviceprincipaltarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3130b-107">属性</span><span class="sxs-lookup"><span data-stu-id="3130b-107">Properties</span></span>
<span data-ttu-id="3130b-108">无。</span><span class="sxs-lookup"><span data-stu-id="3130b-108">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3130b-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3130b-109">JSON representation</span></span>
<span data-ttu-id="3130b-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3130b-110">The following is a JSON representation of the resource.</span></span>
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
