---
title: 筛选器资源类型
description: 确定应将哪些对象设置为应用程序。 例如，您可能希望仅预配位于美国的用户。 当存在范围筛选器时，将在同步过程中跳过不满足筛选器的对象。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9e7e4cfc629cb8586c1fd1cf2e32474b0bc6b6cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520196"
---
# <a name="filter-resource-type"></a><span data-ttu-id="f1714-105">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="f1714-105">filter resource type</span></span>

<span data-ttu-id="f1714-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f1714-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1714-107">确定应将哪些对象设置为应用程序。</span><span class="sxs-lookup"><span data-stu-id="f1714-107">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="f1714-108">例如，您可能希望仅预配位于美国的用户。</span><span class="sxs-lookup"><span data-stu-id="f1714-108">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="f1714-109">当存在范围筛选器时，将在同步过程中跳过不满足筛选器的对象。</span><span class="sxs-lookup"><span data-stu-id="f1714-109">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="f1714-110">筛选器是[对象映射](synchronization-objectmapping.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="f1714-110">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="f1714-111">它由多个筛选器组集组成，每个筛选器组包含一个或多个子句。</span><span class="sxs-lookup"><span data-stu-id="f1714-111">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="f1714-112">仅当组的所有子句都计算为`true` `true`时，才会在组的作用域中考虑对象（组的计算结果为）。</span><span class="sxs-lookup"><span data-stu-id="f1714-112">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="f1714-113">如果将集合中的任意组评估为， `true` `true`则在组集的范围内考虑对象（组集的计算结果为）。</span><span class="sxs-lookup"><span data-stu-id="f1714-113">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="f1714-114">有关详细信息，请参阅[基于属性的应用程序预配和作用域筛选器](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="f1714-114">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="f1714-115">属性</span><span class="sxs-lookup"><span data-stu-id="f1714-115">Properties</span></span>
| <span data-ttu-id="f1714-116">属性</span><span class="sxs-lookup"><span data-stu-id="f1714-116">Property</span></span>     | <span data-ttu-id="f1714-117">类型</span><span class="sxs-lookup"><span data-stu-id="f1714-117">Type</span></span>   |<span data-ttu-id="f1714-118">说明</span><span class="sxs-lookup"><span data-stu-id="f1714-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1714-119">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="f1714-119">categoryFilterGroups</span></span>|<span data-ttu-id="f1714-120">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1714-120">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="f1714-121">`*Experimental*`用于确定给定对象是否属于的筛选器组集，以及应作为此对象映射的一部分进行处理的筛选器组集。</span><span class="sxs-lookup"><span data-stu-id="f1714-121">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="f1714-122">*如果集合中的任何组的计算结果为， `true`* 则在范围内考虑对象。</span><span class="sxs-lookup"><span data-stu-id="f1714-122">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="f1714-123">groups</span><span class="sxs-lookup"><span data-stu-id="f1714-123">groups</span></span>|<span data-ttu-id="f1714-124">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1714-124">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="f1714-125">用于确定给定对象是否在设置范围内的筛选器组集。</span><span class="sxs-lookup"><span data-stu-id="f1714-125">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="f1714-126">**这是在大多数情况下应使用的筛选器**。</span><span class="sxs-lookup"><span data-stu-id="f1714-126">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="f1714-127">如果某个对象在给定时刻满足此筛选器的需要，然后对象或筛选器发生了更改，因此不能再满足筛选器的要求，则此类对象 \* 将被取消设置。</span><span class="sxs-lookup"><span data-stu-id="f1714-127">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="f1714-128">*如果集合中的任何组的计算结果为， `true`* 则在范围内考虑对象。</span><span class="sxs-lookup"><span data-stu-id="f1714-128">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="f1714-129">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="f1714-129">inputFilterGroups</span></span>|<span data-ttu-id="f1714-130">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1714-130">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="f1714-131">`*Experimental*`用于在从目录读取对象的早期阶段筛选出对象的筛选器组集。</span><span class="sxs-lookup"><span data-stu-id="f1714-131">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="f1714-132">如果对象不满足此筛选器，则不会对其进行进一步处理。</span><span class="sxs-lookup"><span data-stu-id="f1714-132">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="f1714-133">需要了解的重要一点是，如果某个对象在给定时刻满足此筛选器，然后对象或筛选器已更改，因此筛选器不再满足要求，则此类对象*将不会被取消预配*。</span><span class="sxs-lookup"><span data-stu-id="f1714-133">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="f1714-134">*如果集合中的任何组的计算结果为， `true`* 则在范围内考虑对象。</span><span class="sxs-lookup"><span data-stu-id="f1714-134">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1714-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1714-135">JSON representation</span></span>

<span data-ttu-id="f1714-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1714-136">Here is a JSON representation of the resource.</span></span>

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
