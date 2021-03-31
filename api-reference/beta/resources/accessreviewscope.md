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
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="11d89-103">accessReviewScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="11d89-103">accessReviewScope resource type</span></span>

<span data-ttu-id="11d89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11d89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="11d89-105">**accessReviewScope** 定义哪些实体将在 [accessReviewScheduleDefinition 中查看](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="11d89-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="11d89-106">它是由 accessReviewQueryScope、principalResourceMembershipsScope 和[accessReviewReviewerScope](accessreviewreviewerscope.md)继承的抽象类型。 [](accessreviewqueryscope.md) [](principalresourcemembershipsscope.md)</span><span class="sxs-lookup"><span data-stu-id="11d89-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="11d89-107">有关 `scope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 的属性，请参阅 [accessReviewQueryScope](accessreviewqueryscope.md) 和 [principalResourceMembershipsScope](principalresourcemembershipsscope.md)。</span><span class="sxs-lookup"><span data-stu-id="11d89-107">For `scope` property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="11d89-108">有关 `reviewers` [accessReviewScheduleDefinition 的属性，](accessreviewscheduledefinition.md) 请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="11d89-108">For `reviewers` property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11d89-109">属性</span><span class="sxs-lookup"><span data-stu-id="11d89-109">Properties</span></span>
<span data-ttu-id="11d89-110">无。</span><span class="sxs-lookup"><span data-stu-id="11d89-110">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="11d89-111">关系</span><span class="sxs-lookup"><span data-stu-id="11d89-111">Relationships</span></span>
<span data-ttu-id="11d89-112">无。</span><span class="sxs-lookup"><span data-stu-id="11d89-112">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11d89-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11d89-113">JSON representation</span></span>
<span data-ttu-id="11d89-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11d89-114">The following is a JSON representation of the resource.</span></span>
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
