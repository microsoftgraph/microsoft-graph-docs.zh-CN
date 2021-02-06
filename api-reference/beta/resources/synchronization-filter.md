---
title: 筛选器资源类型
description: 确定应该向应用程序预配哪些对象。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8c461dffab9af810d20f6b866134ecc5d4238eb1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133929"
---
# <a name="filter-resource-type"></a><span data-ttu-id="aa80c-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="aa80c-103">filter resource type</span></span>

<span data-ttu-id="aa80c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa80c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa80c-105">确定应该向应用程序预配哪些对象。</span><span class="sxs-lookup"><span data-stu-id="aa80c-105">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="aa80c-106">例如，你可能希望仅预配位于美国的用户。</span><span class="sxs-lookup"><span data-stu-id="aa80c-106">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="aa80c-107">存在作用域筛选器时，在同步过程中将跳过不满足该筛选器的对象。</span><span class="sxs-lookup"><span data-stu-id="aa80c-107">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="aa80c-108">筛选器是对象 [映射的一部分](synchronization-objectmapping.md)。</span><span class="sxs-lookup"><span data-stu-id="aa80c-108">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="aa80c-109">它由多组筛选器组组成，每个筛选器组包含一个或多个子句。</span><span class="sxs-lookup"><span data-stu-id="aa80c-109">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="aa80c-110">在组范围内考虑对象 (只有在组的所有子句都计算为) 计算组时，才计算为一 `true` 个对象 `true` 。</span><span class="sxs-lookup"><span data-stu-id="aa80c-110">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="aa80c-111">在组集范围内考虑对象， (组集求值) 组集的任何组求值为 `true` `true` 。</span><span class="sxs-lookup"><span data-stu-id="aa80c-111">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="aa80c-112">有关详细信息，请参阅使用范围筛选器的基于属性 [的应用程序设置](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="aa80c-112">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="aa80c-113">属性</span><span class="sxs-lookup"><span data-stu-id="aa80c-113">Properties</span></span>
| <span data-ttu-id="aa80c-114">属性</span><span class="sxs-lookup"><span data-stu-id="aa80c-114">Property</span></span>     | <span data-ttu-id="aa80c-115">类型</span><span class="sxs-lookup"><span data-stu-id="aa80c-115">Type</span></span>   |<span data-ttu-id="aa80c-116">说明</span><span class="sxs-lookup"><span data-stu-id="aa80c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa80c-117">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="aa80c-117">categoryFilterGroups</span></span>|<span data-ttu-id="aa80c-118">[filterGroup](synchronization-filtergroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa80c-118">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="aa80c-119">`*Experimental*` 用于决定给定对象是否属于且应作为此对象映射的一部分进行处理的筛选器组集。</span><span class="sxs-lookup"><span data-stu-id="aa80c-119">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="aa80c-120">如果将集合中的任一组求值为 ，则视为范围内 *的对象 `true`*。</span><span class="sxs-lookup"><span data-stu-id="aa80c-120">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="aa80c-121">groups</span><span class="sxs-lookup"><span data-stu-id="aa80c-121">groups</span></span>|<span data-ttu-id="aa80c-122">[filterGroup](synchronization-filtergroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa80c-122">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="aa80c-123">用于决定给定对象是否位于设置范围的筛选器组集。</span><span class="sxs-lookup"><span data-stu-id="aa80c-123">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="aa80c-124">**这是在大多数情况下应该使用的筛选器**。</span><span class="sxs-lookup"><span data-stu-id="aa80c-124">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="aa80c-125">如果用于满足此筛选器的对象在给定时刻，然后对象或筛选器已更改，以便不再满足筛选器，则此类对象 \*将被取消设置"。</span><span class="sxs-lookup"><span data-stu-id="aa80c-125">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="aa80c-126">如果将集合中的任一组求值为 ，则视为范围内 *的对象 `true`*。</span><span class="sxs-lookup"><span data-stu-id="aa80c-126">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="aa80c-127">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="aa80c-127">inputFilterGroups</span></span>|<span data-ttu-id="aa80c-128">[filterGroup](synchronization-filtergroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa80c-128">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="aa80c-129">`*Experimental*` 用于在从目录读取对象的早期阶段筛选出对象的筛选器组集。</span><span class="sxs-lookup"><span data-stu-id="aa80c-129">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="aa80c-130">如果对象不满足此筛选器，则将不会进一步处理该对象。</span><span class="sxs-lookup"><span data-stu-id="aa80c-130">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="aa80c-131">必须了解的是，如果用于满足此筛选器的对象在给定时刻，然后对象或筛选器已更改，以便不再满足筛选器，则此类对象将不会取消 *设置*。</span><span class="sxs-lookup"><span data-stu-id="aa80c-131">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="aa80c-132">如果将集合中的任一组求值为 ，则视为范围内 *的对象 `true`*。</span><span class="sxs-lookup"><span data-stu-id="aa80c-132">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa80c-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa80c-133">JSON representation</span></span>

<span data-ttu-id="aa80c-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa80c-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


