---
title: plannerPlanContextDetailsCollection 资源类型
description: " 值是 plannerPlanContextDetails 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 017734f3d5f5fb1a0ed56f390a7c945e43b707a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981474"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="6a488-103">plannerPlanContextDetailsCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a488-103">plannerPlanContextDetailsCollection resource type</span></span>

> <span data-ttu-id="6a488-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a488-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a488-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a488-105">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="6a488-106">**PlannerPlanContextDetailsCollection**资源表示的外部上下文计划链接到的集合。</span><span class="sxs-lookup"><span data-stu-id="6a488-106">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="6a488-107">此资源是开放的类型， [plannerPlanDetails](plannerplandetails.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="6a488-107">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="6a488-108">中的属性值对的属性名称是上下文; 特定于应用程序的标识符值是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a488-108">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="6a488-109">属性</span><span class="sxs-lookup"><span data-stu-id="6a488-109">Properties</span></span>
<span data-ttu-id="6a488-110">打开类型的属性可定义由客户端。</span><span class="sxs-lookup"><span data-stu-id="6a488-110">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="6a488-111">在这种情况下，客户应使用的独特的标识符值，该值代表外部上下文与属性名称。</span><span class="sxs-lookup"><span data-stu-id="6a488-111">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="6a488-112">属性值必须是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a488-112">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="6a488-113">基于 OData，在打开的类型的属性名称不能包含下列字符： `.`， `:`， `@`， `%`。</span><span class="sxs-lookup"><span data-stu-id="6a488-113">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="6a488-114">需要 URL 编码格式编码这些字符。</span><span class="sxs-lookup"><span data-stu-id="6a488-114">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="6a488-115">在收藏夹列表中删除项目，需要的值从集合中删除[plannerPlanContextCollection](plannerplancontextcollection.md)相反，其自动将此对象中删除的项。</span><span class="sxs-lookup"><span data-stu-id="6a488-115">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
