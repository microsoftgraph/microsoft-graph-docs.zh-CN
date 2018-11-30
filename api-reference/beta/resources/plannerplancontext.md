---
title: plannerPlanContext 资源类型
description: '**PlannerPlanContext**资源表示 plannerPlan 计划程序之外的用户体验的关系。 可以在其他体验，如 Microsoft 团队，来跟踪工作的用户体验的上下文中显示计划程序中的计划。'
ms.openlocfilehash: 84512c03081a3e1fd2b15456c64cecf3f9c39435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045631"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="9e197-104">plannerPlanContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e197-104">plannerPlanContext resource type</span></span>

> <span data-ttu-id="9e197-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9e197-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e197-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e197-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e197-107">**PlannerPlanContext**资源表示[plannerPlan](plannerplan.md)计划程序之外的用户体验的关系。</span><span class="sxs-lookup"><span data-stu-id="9e197-107">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="9e197-108">可以在其他体验，如 Microsoft 团队，来跟踪工作的用户体验的上下文中显示计划程序中的计划。</span><span class="sxs-lookup"><span data-stu-id="9e197-108">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="9e197-109">可以基于**ownerAppId**属性标识**plannerPlanContext**条目 reresents 的体验：</span><span class="sxs-lookup"><span data-stu-id="9e197-109">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="9e197-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346： 上下文项目所属的 Microsoft 团队。</span><span class="sxs-lookup"><span data-stu-id="9e197-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="9e197-111">00000003-0000-0ff1-ce00-000000000000： 上下文项目属于 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="9e197-111">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="9e197-112">属性</span><span class="sxs-lookup"><span data-stu-id="9e197-112">Properties</span></span>
| <span data-ttu-id="9e197-113">属性</span><span class="sxs-lookup"><span data-stu-id="9e197-113">Property</span></span>     | <span data-ttu-id="9e197-114">类型</span><span class="sxs-lookup"><span data-stu-id="9e197-114">Type</span></span>   |<span data-ttu-id="9e197-115">说明</span><span class="sxs-lookup"><span data-stu-id="9e197-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e197-116">associationType</span><span class="sxs-lookup"><span data-stu-id="9e197-116">associationType</span></span>|<span data-ttu-id="9e197-117">字符串</span><span class="sxs-lookup"><span data-stu-id="9e197-117">String</span></span>|<span data-ttu-id="9e197-118">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e197-118">Nullable.</span></span> <span data-ttu-id="9e197-119">[PlannerPlan](plannerplan.md)和应用程序之间的关联的应用程序定义的类型。</span><span class="sxs-lookup"><span data-stu-id="9e197-119">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="9e197-120">应用程序可以使用此信息来跟踪对同一[plannerPlan](plannerplan.md)不同类型的关系。</span><span class="sxs-lookup"><span data-stu-id="9e197-120">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="9e197-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e197-121">createdDateTime</span></span>|<span data-ttu-id="9e197-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e197-122">DateTimeOffset</span></span>|<span data-ttu-id="9e197-123">只读。</span><span class="sxs-lookup"><span data-stu-id="9e197-123">Read-only.</span></span> <span data-ttu-id="9e197-124">日期和时间创建**plannerPlanContext**时。</span><span class="sxs-lookup"><span data-stu-id="9e197-124">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="9e197-125">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9e197-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e197-126">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="9e197-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9e197-127">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="9e197-127">displayNameSegments</span></span>|<span data-ttu-id="9e197-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e197-128">String collection</span></span>|<span data-ttu-id="9e197-129">线段的外部体验的名称。</span><span class="sxs-lookup"><span data-stu-id="9e197-129">The segments of the name of the external experience.</span></span> <span data-ttu-id="9e197-130">段表示允许其他应用程序，以显示关系的层次结构。</span><span class="sxs-lookup"><span data-stu-id="9e197-130">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="9e197-131">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="9e197-131">ownerAppId</span></span>|<span data-ttu-id="9e197-132">String</span><span class="sxs-lookup"><span data-stu-id="9e197-132">String</span></span>|<span data-ttu-id="9e197-133">只读。</span><span class="sxs-lookup"><span data-stu-id="9e197-133">Read-only.</span></span> <span data-ttu-id="9e197-134">创建**plannerPlanContext**的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e197-134">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e197-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e197-135">JSON representation</span></span>

<span data-ttu-id="9e197-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e197-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
