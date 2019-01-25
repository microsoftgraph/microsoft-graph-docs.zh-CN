---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 assignedPlan 集合。'
localization_priority: Normal
ms.openlocfilehash: 3e06894fa71f81993b94d174d6cde8a54126fd62
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525134"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="3a633-103">assignedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a633-103">assignedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a633-104">[用户](user.md) 实体和 [组织](organization.md) 实体的 **AssignedPlans** 属性都是一个 **assignedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="3a633-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="3a633-105">属性</span><span class="sxs-lookup"><span data-stu-id="3a633-105">Properties</span></span>
| <span data-ttu-id="3a633-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a633-106">Property</span></span>     | <span data-ttu-id="3a633-107">类型</span><span class="sxs-lookup"><span data-stu-id="3a633-107">Type</span></span>   |<span data-ttu-id="3a633-108">说明</span><span class="sxs-lookup"><span data-stu-id="3a633-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a633-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a633-109">assignedDateTime</span></span>|<span data-ttu-id="3a633-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a633-110">DateTimeOffset</span></span>|<span data-ttu-id="3a633-p101">分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3a633-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3a633-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="3a633-114">capabilityStatus</span></span>|<span data-ttu-id="3a633-115">String</span><span class="sxs-lookup"><span data-stu-id="3a633-115">String</span></span>|<span data-ttu-id="3a633-116">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="3a633-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="3a633-117">服务</span><span class="sxs-lookup"><span data-stu-id="3a633-117">service</span></span>|<span data-ttu-id="3a633-118">String</span><span class="sxs-lookup"><span data-stu-id="3a633-118">String</span></span>|<span data-ttu-id="3a633-119">服务名称；例如，“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="3a633-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="3a633-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="3a633-120">servicePlanId</span></span>|<span data-ttu-id="3a633-121">Guid</span><span class="sxs-lookup"><span data-stu-id="3a633-121">Guid</span></span>|<span data-ttu-id="3a633-122">用于标识服务计划的 GUID。</span><span class="sxs-lookup"><span data-stu-id="3a633-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a633-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a633-123">JSON representation</span></span>

<span data-ttu-id="3a633-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a633-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
