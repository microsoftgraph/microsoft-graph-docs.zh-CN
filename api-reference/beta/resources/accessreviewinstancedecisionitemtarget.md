---
title: accessReviewInstanceDecisionItemTarget 资源类型
description: '将评审的目标表示为用户目标或服务主体目标。 '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c395ffffaf19f03185dac15238eb535155353dca
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000840"
---
# <a name="accessreviewinstancedecisionitemtarget-resource-type"></a><span data-ttu-id="02922-103">accessReviewInstanceDecisionItemTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="02922-103">accessReviewInstanceDecisionItemTarget resource type</span></span>

<span data-ttu-id="02922-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02922-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02922-105">表示不同类型的审阅目标的基类，每种类型都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="02922-105">Represents a base class for different types of review targets, each one with its own specific properties.</span></span> <span data-ttu-id="02922-106">支持的目标类型为： [accessReviewInstanceDecisionItemUserTarget](accessreviewinstancedecisionitemusertarget.md) 和 [accessReviewInstanceDecisionItemServicePrincipalTarget](accessreviewinstancedecisionitemserviceprincipaltarget.md)。</span><span class="sxs-lookup"><span data-stu-id="02922-106">The supported target types are: [accessReviewInstanceDecisionItemUserTarget](accessreviewinstancedecisionitemusertarget.md) and [accessReviewInstanceDecisionItemServicePrincipalTarget](accessreviewinstancedecisionitemserviceprincipaltarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="02922-107">属性</span><span class="sxs-lookup"><span data-stu-id="02922-107">Properties</span></span>
<span data-ttu-id="02922-108">无。</span><span class="sxs-lookup"><span data-stu-id="02922-108">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="02922-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02922-109">JSON representation</span></span>
<span data-ttu-id="02922-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02922-110">The following is a JSON representation of the resource.</span></span>
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
