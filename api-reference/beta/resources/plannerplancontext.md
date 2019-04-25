---
title: plannerPlanContext 资源类型
description: '**plannerPlanContext**资源表示 plannerPlan 在计划程序外的用户体验的关系。 Planner 中的计划可以在其他体验 (如 Microsoft 团队) 中进行, 以在该体验的上下文中跟踪工作。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522158"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="20af2-104">plannerPlanContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="20af2-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20af2-105">**plannerPlanContext**资源表示[plannerPlan](plannerplan.md)在计划程序外的用户体验的关系。</span><span class="sxs-lookup"><span data-stu-id="20af2-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="20af2-106">Planner 中的计划可以在其他体验 (如 Microsoft 团队) 中进行, 以在该体验的上下文中跟踪工作。</span><span class="sxs-lookup"><span data-stu-id="20af2-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="20af2-107">可以基于**ownerAppId**属性来标识**plannerPlanContext**条目 reresents 的体验:</span><span class="sxs-lookup"><span data-stu-id="20af2-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="20af2-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: 上下文条目属于 Microsoft 团队。</span><span class="sxs-lookup"><span data-stu-id="20af2-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="20af2-109">为 00000003-0000-0ff1-ce00-000000000000: 上下文条目属于 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="20af2-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="20af2-110">属性</span><span class="sxs-lookup"><span data-stu-id="20af2-110">Properties</span></span>
| <span data-ttu-id="20af2-111">属性</span><span class="sxs-lookup"><span data-stu-id="20af2-111">Property</span></span>     | <span data-ttu-id="20af2-112">类型</span><span class="sxs-lookup"><span data-stu-id="20af2-112">Type</span></span>   |<span data-ttu-id="20af2-113">说明</span><span class="sxs-lookup"><span data-stu-id="20af2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20af2-114">associationType</span><span class="sxs-lookup"><span data-stu-id="20af2-114">associationType</span></span>|<span data-ttu-id="20af2-115">String</span><span class="sxs-lookup"><span data-stu-id="20af2-115">String</span></span>|<span data-ttu-id="20af2-116">可为空。</span><span class="sxs-lookup"><span data-stu-id="20af2-116">Nullable.</span></span> <span data-ttu-id="20af2-117">[plannerPlan](plannerplan.md)与应用之间的应用程序定义类型的关联。</span><span class="sxs-lookup"><span data-stu-id="20af2-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="20af2-118">应用程序可以使用此信息跟踪与同一[plannerPlan](plannerplan.md)的不同类型的关系。</span><span class="sxs-lookup"><span data-stu-id="20af2-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="20af2-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20af2-119">createdDateTime</span></span>|<span data-ttu-id="20af2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20af2-120">DateTimeOffset</span></span>|<span data-ttu-id="20af2-121">只读。</span><span class="sxs-lookup"><span data-stu-id="20af2-121">Read-only.</span></span> <span data-ttu-id="20af2-122">**plannerPlanContext**的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="20af2-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="20af2-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="20af2-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="20af2-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="20af2-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="20af2-125">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="20af2-125">displayNameSegments</span></span>|<span data-ttu-id="20af2-126">String collection</span><span class="sxs-lookup"><span data-stu-id="20af2-126">String collection</span></span>|<span data-ttu-id="20af2-127">外部体验名称的各个部分。</span><span class="sxs-lookup"><span data-stu-id="20af2-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="20af2-128">段表示允许其他应用显示关系的层次结构。</span><span class="sxs-lookup"><span data-stu-id="20af2-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="20af2-129">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="20af2-129">ownerAppId</span></span>|<span data-ttu-id="20af2-130">String</span><span class="sxs-lookup"><span data-stu-id="20af2-130">String</span></span>|<span data-ttu-id="20af2-131">只读。</span><span class="sxs-lookup"><span data-stu-id="20af2-131">Read-only.</span></span> <span data-ttu-id="20af2-132">创建**plannerPlanContext**的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="20af2-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20af2-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20af2-133">JSON representation</span></span>

<span data-ttu-id="20af2-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20af2-134">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
