---
title: directoryAudit 资源类型
description: 介绍 Microsoft Graph API (REST) 的 directoryAudit (实体) ，这有助于审核 () beta () 的目录。
author: SarahBar
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f7d7031033a791bb6cf02e2bad527d4decf2b3ea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962614"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="ed3f6-103">directoryAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed3f6-103">directoryAudit resource type</span></span>

<span data-ttu-id="ed3f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed3f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed3f6-105">表示目录审核项目及其集合。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="ed3f6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ed3f6-106">Methods</span></span>

| <span data-ttu-id="ed3f6-107">方法</span><span class="sxs-lookup"><span data-stu-id="ed3f6-107">Method</span></span>           | <span data-ttu-id="ed3f6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed3f6-108">Return Type</span></span>    |<span data-ttu-id="ed3f6-109">说明</span><span class="sxs-lookup"><span data-stu-id="ed3f6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed3f6-110">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="ed3f6-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="ed3f6-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="ed3f6-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="ed3f6-112">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="ed3f6-113">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="ed3f6-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="ed3f6-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="ed3f6-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="ed3f6-115">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-115">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ed3f6-116">属性</span><span class="sxs-lookup"><span data-stu-id="ed3f6-116">Properties</span></span>
| <span data-ttu-id="ed3f6-117">属性</span><span class="sxs-lookup"><span data-stu-id="ed3f6-117">Property</span></span>            | <span data-ttu-id="ed3f6-118">类型</span><span class="sxs-lookup"><span data-stu-id="ed3f6-118">Type</span></span>                                                | <span data-ttu-id="ed3f6-119">说明</span><span class="sxs-lookup"><span data-stu-id="ed3f6-119">Description</span></span>                                                                                                                                                                                                                                                            |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ed3f6-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="ed3f6-120">activityDateTime</span></span>    | <span data-ttu-id="ed3f6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed3f6-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="ed3f6-122">指示执行活动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="ed3f6-123">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="ed3f6-124">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>                                                                              |
| <span data-ttu-id="ed3f6-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed3f6-125">activityDisplayName</span></span> | <span data-ttu-id="ed3f6-126">String</span><span class="sxs-lookup"><span data-stu-id="ed3f6-126">String</span></span>                                              | <span data-ttu-id="ed3f6-127">指示活动名称或操作名称（例如，</span><span class="sxs-lookup"><span data-stu-id="ed3f6-127">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="ed3f6-128">“创建用户”、“向组中添加成员”）。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-128">"Create User", "Add member to group").</span></span> <span data-ttu-id="ed3f6-129">有关记录的活动列表，请参阅 [Azure Ad 活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-129">For a list of activities logged, refer to [Azure Ad activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="ed3f6-130">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="ed3f6-130">additionalDetails</span></span>   | <span data-ttu-id="ed3f6-131">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed3f6-131">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="ed3f6-132">指示活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-132">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="ed3f6-133">category</span><span class="sxs-lookup"><span data-stu-id="ed3f6-133">category</span></span>            | <span data-ttu-id="ed3f6-134">String</span><span class="sxs-lookup"><span data-stu-id="ed3f6-134">String</span></span>                                              | <span data-ttu-id="ed3f6-135">指示活动所针对的资源类别。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-135">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="ed3f6-136">（例如：用户管理、组管理等。）</span><span class="sxs-lookup"><span data-stu-id="ed3f6-136">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                              |
| <span data-ttu-id="ed3f6-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="ed3f6-137">correlationId</span></span>       | <span data-ttu-id="ed3f6-138">GUID</span><span class="sxs-lookup"><span data-stu-id="ed3f6-138">GUID</span></span>                                                | <span data-ttu-id="ed3f6-139">指示有助于关联跨各种服务的活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-139">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="ed3f6-140">可用于跨服务跟踪日志。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-140">Can be used to trace logs across services.</span></span>                                                                                                                                    |
| <span data-ttu-id="ed3f6-141">id</span><span class="sxs-lookup"><span data-stu-id="ed3f6-141">id</span></span>                  | <span data-ttu-id="ed3f6-142">String</span><span class="sxs-lookup"><span data-stu-id="ed3f6-142">String</span></span>                                              | <span data-ttu-id="ed3f6-143">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-143">Indicates the unique ID for the activity.</span></span>                                                                                                                                                                                                            |
| <span data-ttu-id="ed3f6-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="ed3f6-144">initiatedBy</span></span>         | [<span data-ttu-id="ed3f6-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="ed3f6-145">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="ed3f6-146">指示有关启动活动的用户或应用的信息。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-146">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                    |
| <span data-ttu-id="ed3f6-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="ed3f6-147">loggedByService</span></span>     | <span data-ttu-id="ed3f6-148">String</span><span class="sxs-lookup"><span data-stu-id="ed3f6-148">String</span></span>                                              | <span data-ttu-id="ed3f6-149">指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                          |
| <span data-ttu-id="ed3f6-150">result</span><span class="sxs-lookup"><span data-stu-id="ed3f6-150">result</span></span>              | <span data-ttu-id="ed3f6-151">operationResult</span><span class="sxs-lookup"><span data-stu-id="ed3f6-151">operationResult</span></span>                                              | <span data-ttu-id="ed3f6-152">指示活动的结果。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-152">Indicates the result of the activity.</span></span> <span data-ttu-id="ed3f6-153">可取值为：`success`、`failure`、`timeout`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-153">Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                       |
| <span data-ttu-id="ed3f6-154">resultReason</span><span class="sxs-lookup"><span data-stu-id="ed3f6-154">resultReason</span></span>        | <span data-ttu-id="ed3f6-155">String</span><span class="sxs-lookup"><span data-stu-id="ed3f6-155">String</span></span>                                              | <span data-ttu-id="ed3f6-156">指示结果为 或 **时失败** `failure` 的原因 `timeout` 。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-156">Indicates the reason for failure if the **result** is `failure` or `timeout`.</span></span>                                                                                                                                                                                              |
| <span data-ttu-id="ed3f6-157">targetResources</span><span class="sxs-lookup"><span data-stu-id="ed3f6-157">targetResources</span></span>     | <span data-ttu-id="ed3f6-158">[targetResource](targetresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed3f6-158">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="ed3f6-159">指示由于活动而更改的资源的信息。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-159">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="ed3f6-160">目标资源类型可以是 `User` `Device` `Directory` `App` 、、、、、 `Role` 或 `Group` `Policy` `Other` 。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-160">Target Resource Type can be `User`, `Device`, `Directory`, `App`, `Role`, `Group`, `Policy` or `Other`.</span></span>                                                                                                       |

## <a name="relationships"></a><span data-ttu-id="ed3f6-161">关系</span><span class="sxs-lookup"><span data-stu-id="ed3f6-161">Relationships</span></span>
<span data-ttu-id="ed3f6-162">无</span><span class="sxs-lookup"><span data-stu-id="ed3f6-162">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed3f6-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed3f6-163">JSON representation</span></span>

<span data-ttu-id="ed3f6-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed3f6-164">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


