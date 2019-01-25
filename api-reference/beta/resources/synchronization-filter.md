---
title: 筛选器资源类型
description: 确定哪些对象应该设置到应用程序。 例如，您可能希望向只位于美国的设置用户。 存在范围筛选器时，将同步过程中跳过不满足筛选器的对象。
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516677"
---
# <a name="filter-resource-type"></a><span data-ttu-id="fbc32-105">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="fbc32-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbc32-106">确定哪些对象应该设置到应用程序。</span><span class="sxs-lookup"><span data-stu-id="fbc32-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="fbc32-107">例如，您可能希望向只位于美国的设置用户。</span><span class="sxs-lookup"><span data-stu-id="fbc32-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="fbc32-108">存在范围筛选器时，将同步过程中跳过不满足筛选器的对象。</span><span class="sxs-lookup"><span data-stu-id="fbc32-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="fbc32-109">筛选器是[对象映射](synchronization-objectmapping.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="fbc32-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="fbc32-110">它包含的筛选器组几组和每个筛选器组包含一个或多个子句。</span><span class="sxs-lookup"><span data-stu-id="fbc32-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="fbc32-111">对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。</span><span class="sxs-lookup"><span data-stu-id="fbc32-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="fbc32-112">对象被视为组集范围内 (组集中计算为`true`) 如果任何集中组计算结果为`true`。</span><span class="sxs-lookup"><span data-stu-id="fbc32-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="fbc32-113">有关详细信息，请参阅[基于属性的应用程序与范围筛选器设置](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="fbc32-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="fbc32-114">属性</span><span class="sxs-lookup"><span data-stu-id="fbc32-114">Properties</span></span>
| <span data-ttu-id="fbc32-115">属性</span><span class="sxs-lookup"><span data-stu-id="fbc32-115">Property</span></span>     | <span data-ttu-id="fbc32-116">类型</span><span class="sxs-lookup"><span data-stu-id="fbc32-116">Type</span></span>   |<span data-ttu-id="fbc32-117">说明</span><span class="sxs-lookup"><span data-stu-id="fbc32-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbc32-118">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="fbc32-118">categoryFilterGroups</span></span>|<span data-ttu-id="fbc32-119">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbc32-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="fbc32-120">`*Experimental*`用于确定是否给定对象所属的组设置筛选器，并应作为此对象映射的一部分。</span><span class="sxs-lookup"><span data-stu-id="fbc32-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="fbc32-121">对象被视为范围内*如果集合中的组的任何计算结果为`true`*。</span><span class="sxs-lookup"><span data-stu-id="fbc32-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="fbc32-122">组</span><span class="sxs-lookup"><span data-stu-id="fbc32-122">groups</span></span>|<span data-ttu-id="fbc32-123">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbc32-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="fbc32-124">组设置用来确定给定对象是否在范围内用于设置筛选器。</span><span class="sxs-lookup"><span data-stu-id="fbc32-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="fbc32-125">**这是在大多数情况下应使用哪些筛选器**。</span><span class="sxs-lookup"><span data-stu-id="fbc32-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="fbc32-126">如果用来满足给定时刻，此筛选器对象然后对象或筛选器已更改，因此该筛选器是不满足任何更长时间，此类对象 \* 获取取消设置"。</span><span class="sxs-lookup"><span data-stu-id="fbc32-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="fbc32-127">对象被视为范围内*如果集合中的组的任何计算结果为`true`*。</span><span class="sxs-lookup"><span data-stu-id="fbc32-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="fbc32-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="fbc32-128">inputFilterGroups</span></span>|<span data-ttu-id="fbc32-129">[filterGroup](synchronization-filtergroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbc32-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="fbc32-130">`*Experimental*`用于在从目录中读取的早期阶段筛选掉对象的筛选器组设置。</span><span class="sxs-lookup"><span data-stu-id="fbc32-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="fbc32-131">如果对象不满足此筛选器，它将不进一步处理。</span><span class="sxs-lookup"><span data-stu-id="fbc32-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="fbc32-132">一定要了解，如果一个对象用于在给定的时刻，满足此筛选器，然后对象或筛选器已更改，以便该筛选器不再满足，例如对象*不获取取消设置*。</span><span class="sxs-lookup"><span data-stu-id="fbc32-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="fbc32-133">对象被视为范围内*如果集合中的组的任何计算结果为`true`*。</span><span class="sxs-lookup"><span data-stu-id="fbc32-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fbc32-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbc32-134">JSON representation</span></span>

<span data-ttu-id="fbc32-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbc32-135">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
