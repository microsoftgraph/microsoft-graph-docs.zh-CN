---
title: assignedPlan 资源类型
description: '**用户** 实体和 组织 实体的 AssignedPlans 属性都是一个 **assignedPlan** 集合。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 5e408212855e4ca0bc5af4c03302c8b79e415566
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809826"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="78bcc-103">assignedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="78bcc-103">assignedPlan resource type</span></span>

<span data-ttu-id="78bcc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78bcc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78bcc-105">**用户** 实体和 [组织](user.md) 实体的 [AssignedPlans](organization.md) 属性都是一个 **assignedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="78bcc-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="78bcc-106">属性</span><span class="sxs-lookup"><span data-stu-id="78bcc-106">Properties</span></span>
| <span data-ttu-id="78bcc-107">属性</span><span class="sxs-lookup"><span data-stu-id="78bcc-107">Property</span></span>     | <span data-ttu-id="78bcc-108">类型</span><span class="sxs-lookup"><span data-stu-id="78bcc-108">Type</span></span>   |<span data-ttu-id="78bcc-109">说明</span><span class="sxs-lookup"><span data-stu-id="78bcc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78bcc-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="78bcc-110">assignedDateTime</span></span>|<span data-ttu-id="78bcc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78bcc-111">DateTimeOffset</span></span>|<span data-ttu-id="78bcc-p101">分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78bcc-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78bcc-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="78bcc-115">capabilityStatus</span></span>|<span data-ttu-id="78bcc-116">String</span><span class="sxs-lookup"><span data-stu-id="78bcc-116">String</span></span>|<span data-ttu-id="78bcc-117">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="78bcc-117">For example, “Enabled”.</span></span>|
|<span data-ttu-id="78bcc-118">服务</span><span class="sxs-lookup"><span data-stu-id="78bcc-118">service</span></span>|<span data-ttu-id="78bcc-119">String</span><span class="sxs-lookup"><span data-stu-id="78bcc-119">String</span></span>|<span data-ttu-id="78bcc-120">服务名称；例如，“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="78bcc-120">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="78bcc-121">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="78bcc-121">servicePlanId</span></span>|<span data-ttu-id="78bcc-122">Guid</span><span class="sxs-lookup"><span data-stu-id="78bcc-122">Guid</span></span>|<span data-ttu-id="78bcc-123">用于标识服务计划的 GUID。</span><span class="sxs-lookup"><span data-stu-id="78bcc-123">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78bcc-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78bcc-124">JSON representation</span></span>

<span data-ttu-id="78bcc-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78bcc-125">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
