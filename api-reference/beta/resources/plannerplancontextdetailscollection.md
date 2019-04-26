---
title: plannerPlanContextDetailsCollection 资源类型
description: " 值是 plannerPlanContextDetails 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 2e2f292de763674510f6da5a8aad90fe8e17ab7f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344394"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="fd108-103">plannerPlanContextDetailsCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd108-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="fd108-104">**plannerPlanContextDetailsCollection**资源表示规划所链接到的外部上下文的集合。</span><span class="sxs-lookup"><span data-stu-id="fd108-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="fd108-105">此资源是打开的类型, 并且是[plannerPlanDetails](plannerplandetails.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="fd108-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="fd108-106">属性值对中的属性名称是上下文特定于应用程序的标识符;值是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd108-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="fd108-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd108-107">Properties</span></span>
<span data-ttu-id="fd108-108">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="fd108-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="fd108-109">在这种情况下, 客户端应使用表示外部上下文的独特标识符作为属性名称。</span><span class="sxs-lookup"><span data-stu-id="fd108-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="fd108-110">属性值必须是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd108-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="fd108-111">根据 OData, 开放式类型中的属性名称不能包含以下字符: `.`、 `:`、 `@`、 `%`。</span><span class="sxs-lookup"><span data-stu-id="fd108-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="fd108-112">需要使用 URL 编码格式对这些字符进行编码。</span><span class="sxs-lookup"><span data-stu-id="fd108-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="fd108-113">若要删除收藏夹列表中的项, 需要从[plannerPlanContextCollection](plannerplancontextcollection.md)集合中删除此值, 这将自动删除此对象中的条目。</span><span class="sxs-lookup"><span data-stu-id="fd108-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd108-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd108-114">JSON representation</span></span>
<span data-ttu-id="fd108-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd108-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
