---
title: accessReviewScope 资源类型
description: '在 Azure AD 访问评审功能中，表示将在访问 `accessReviewScope` 评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84b427cdd05aa35fdacb6b80d6ac96c901eef318
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030916"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="607d2-103">accessReviewScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="607d2-103">accessReviewScope resource type</span></span>

<span data-ttu-id="607d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="607d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="607d2-105">**accessReviewScope** 定义哪些实体将在 [accessReviewScheduleDefinition 中查看](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="607d2-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="607d2-106">它是由 accessReviewQueryScope、principalResourceMembershipsScope 和[accessReviewReviewerScope](accessreviewreviewerscope.md)继承的抽象类型。 [](accessreviewqueryscope.md) [](principalresourcemembershipsscope.md)</span><span class="sxs-lookup"><span data-stu-id="607d2-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="607d2-107">有关[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 scope 属性，请参阅[accessReviewQueryScope](accessreviewqueryscope.md)和[principalResourceMembershipsScope](principalresourcemembershipsscope.md)。 </span><span class="sxs-lookup"><span data-stu-id="607d2-107">For **scope** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="607d2-108">有关 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 **reviewers** 属性，请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="607d2-108">For **reviewers** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span>

<span data-ttu-id="607d2-109">强烈建议所有类型指定作用域中的 OData 类型，但对于[principalResourceMembershipsScope](principalresourcemembershipsscope.md)和[accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)是必需的。 </span><span class="sxs-lookup"><span data-stu-id="607d2-109">Specifying the OData type in the **scope** is highly recommended for all types but required for [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="607d2-110">属性</span><span class="sxs-lookup"><span data-stu-id="607d2-110">Properties</span></span>
<span data-ttu-id="607d2-111">无。</span><span class="sxs-lookup"><span data-stu-id="607d2-111">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="607d2-112">关系</span><span class="sxs-lookup"><span data-stu-id="607d2-112">Relationships</span></span>
<span data-ttu-id="607d2-113">无。</span><span class="sxs-lookup"><span data-stu-id="607d2-113">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="607d2-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="607d2-114">JSON representation</span></span>
<span data-ttu-id="607d2-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="607d2-115">The following is a JSON representation of the resource.</span></span>
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
