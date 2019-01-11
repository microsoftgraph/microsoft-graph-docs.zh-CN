---
title: 筛选资源类型
description: 确定哪些对象应该设置到应用程序。 例如，您可能希望向只位于美国的设置用户。 存在范围筛选器时，将同步过程中跳过不满足筛选器的对象。
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894409"
---
# <a name="filter-resource-type"></a><span data-ttu-id="c9833-105">筛选资源类型</span><span class="sxs-lookup"><span data-stu-id="c9833-105">filter resource type</span></span>

> <span data-ttu-id="c9833-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9833-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9833-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9833-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9833-108">确定哪些对象应该设置到应用程序。</span><span class="sxs-lookup"><span data-stu-id="c9833-108">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="c9833-109">例如，您可能希望向只位于美国的设置用户。</span><span class="sxs-lookup"><span data-stu-id="c9833-109">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="c9833-110">存在范围筛选器时，将同步过程中跳过不满足筛选器的对象。</span><span class="sxs-lookup"><span data-stu-id="c9833-110">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="c9833-111">筛选器是[对象映射](synchronization-objectmapping.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="c9833-111">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="c9833-112">它包含的筛选器组几组和每个筛选器组包含一个或多个子句。</span><span class="sxs-lookup"><span data-stu-id="c9833-112">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="c9833-113">对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。</span><span class="sxs-lookup"><span data-stu-id="c9833-113">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="c9833-114">对象被视为组集范围内 (组集中计算为`true`) 如果任何集中组计算结果为`true`。</span><span class="sxs-lookup"><span data-stu-id="c9833-114">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="c9833-115">有关详细信息，请参阅[基于属性的应用程序与范围筛选器设置](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="c9833-115">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="c9833-116">属性</span><span class="sxs-lookup"><span data-stu-id="c9833-116">Properties</span></span>
| <span data-ttu-id="c9833-117">属性</span><span class="sxs-lookup"><span data-stu-id="c9833-117">Property</span></span>     | <span data-ttu-id="c9833-118">类型</span><span class="sxs-lookup"><span data-stu-id="c9833-118">Type</span></span>   |<span data-ttu-id="c9833-119">Description</span><span class="sxs-lookup"><span data-stu-id="c9833-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9833-120">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="c9833-120">categoryFilterGroups</span></span>|<span data-ttu-id="c9833-121">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9833-121">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="c9833-122">`*Experimental*`用于确定是否给定对象所属的组设置筛选器，并应作为此对象映射的一部分。</span><span class="sxs-lookup"><span data-stu-id="c9833-122">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="c9833-123">对象被视为范围内*如果集合中的组的任何计算结果为`true`*。</span><span class="sxs-lookup"><span data-stu-id="c9833-123">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="c9833-124">组</span><span class="sxs-lookup"><span data-stu-id="c9833-124">groups</span></span>|<span data-ttu-id="c9833-125">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9833-125">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="c9833-126">组设置用来确定给定对象是否在范围内用于设置筛选器。</span><span class="sxs-lookup"><span data-stu-id="c9833-126">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="c9833-127">**这是在大多数情况下应使用哪些筛选器**。</span><span class="sxs-lookup"><span data-stu-id="c9833-127">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="c9833-128">如果用来满足给定时刻，此筛选器对象然后对象或筛选器已更改，因此该筛选器是不满足任何更长时间，此类对象 \* 获取取消设置"。</span><span class="sxs-lookup"><span data-stu-id="c9833-128">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="c9833-129">对象被视为范围内*如果集合中的组的任何计算结果为`true`*。</span><span class="sxs-lookup"><span data-stu-id="c9833-129">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="c9833-130">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="c9833-130">inputFilterGroups</span></span>|<span data-ttu-id="c9833-131">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9833-131">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="c9833-132">`*Experimental*`用于在从目录中读取的早期阶段筛选掉对象的筛选器组设置。</span><span class="sxs-lookup"><span data-stu-id="c9833-132">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="c9833-133">如果对象不满足此筛选器，它将不进一步处理。</span><span class="sxs-lookup"><span data-stu-id="c9833-133">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="c9833-134">一定要了解，如果一个对象用于在给定的时刻，满足此筛选器，然后对象或筛选器已更改，以便该筛选器不再满足，例如对象*不获取取消设置*。</span><span class="sxs-lookup"><span data-stu-id="c9833-134">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="c9833-135">对象被视为范围内*如果集合中的组的任何计算结果为`true`*。</span><span class="sxs-lookup"><span data-stu-id="c9833-135">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9833-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9833-136">JSON representation</span></span>

<span data-ttu-id="c9833-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9833-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
