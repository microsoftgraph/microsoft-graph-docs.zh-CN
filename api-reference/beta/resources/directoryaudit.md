---
title: directoryAudit 资源类型
description: 介绍了 directoryAudit 资源 (entity) of Microsoft Graph API (REST) ，这有助于审核目录 (租户)  (beta 版本) 中的活动。
author: SarahBar
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 82093afe35ec5c89158d72c2d3ce80d82770419b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217282"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="15d6b-103">directoryAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="15d6b-103">directoryAudit resource type</span></span>

<span data-ttu-id="15d6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15d6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15d6b-105">表示目录审核项及其集合。</span><span class="sxs-lookup"><span data-stu-id="15d6b-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="15d6b-106">方法</span><span class="sxs-lookup"><span data-stu-id="15d6b-106">Methods</span></span>

| <span data-ttu-id="15d6b-107">方法</span><span class="sxs-lookup"><span data-stu-id="15d6b-107">Method</span></span>           | <span data-ttu-id="15d6b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="15d6b-108">Return Type</span></span>    |<span data-ttu-id="15d6b-109">说明</span><span class="sxs-lookup"><span data-stu-id="15d6b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15d6b-110">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="15d6b-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="15d6b-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="15d6b-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="15d6b-112">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="15d6b-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="15d6b-113">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="15d6b-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="15d6b-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="15d6b-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="15d6b-115">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="15d6b-115">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="15d6b-116">属性</span><span class="sxs-lookup"><span data-stu-id="15d6b-116">Properties</span></span>
| <span data-ttu-id="15d6b-117">属性</span><span class="sxs-lookup"><span data-stu-id="15d6b-117">Property</span></span>            | <span data-ttu-id="15d6b-118">类型</span><span class="sxs-lookup"><span data-stu-id="15d6b-118">Type</span></span>                                                | <span data-ttu-id="15d6b-119">说明</span><span class="sxs-lookup"><span data-stu-id="15d6b-119">Description</span></span>                                                                                                                                                                                                                                                            |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="15d6b-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="15d6b-120">activityDateTime</span></span>    | <span data-ttu-id="15d6b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15d6b-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="15d6b-122">指示执行活动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="15d6b-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="15d6b-123">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="15d6b-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="15d6b-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="15d6b-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>                                                                              |
| <span data-ttu-id="15d6b-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="15d6b-125">activityDisplayName</span></span> | <span data-ttu-id="15d6b-126">String</span><span class="sxs-lookup"><span data-stu-id="15d6b-126">String</span></span>                                              | <span data-ttu-id="15d6b-127">指示活动名称或操作名称（例如，</span><span class="sxs-lookup"><span data-stu-id="15d6b-127">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="15d6b-128">“创建用户”、“向组中添加成员”）。</span><span class="sxs-lookup"><span data-stu-id="15d6b-128">"Create User", "Add member to group").</span></span> <span data-ttu-id="15d6b-129">有关已记录活动的列表，请参阅 [Azure Ad 活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。</span><span class="sxs-lookup"><span data-stu-id="15d6b-129">For a list of activities logged, refer to [Azure Ad activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="15d6b-130">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="15d6b-130">additionalDetails</span></span>   | <span data-ttu-id="15d6b-131">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15d6b-131">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="15d6b-132">指示活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="15d6b-132">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="15d6b-133">category</span><span class="sxs-lookup"><span data-stu-id="15d6b-133">category</span></span>            | <span data-ttu-id="15d6b-134">String</span><span class="sxs-lookup"><span data-stu-id="15d6b-134">String</span></span>                                              | <span data-ttu-id="15d6b-135">指示活动所针对的资源类别。</span><span class="sxs-lookup"><span data-stu-id="15d6b-135">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="15d6b-136">（例如：用户管理、组管理等。）</span><span class="sxs-lookup"><span data-stu-id="15d6b-136">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                              |
| <span data-ttu-id="15d6b-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="15d6b-137">correlationId</span></span>       | <span data-ttu-id="15d6b-138">GUID</span><span class="sxs-lookup"><span data-stu-id="15d6b-138">GUID</span></span>                                                | <span data-ttu-id="15d6b-139">指示有助于关联跨各种服务的活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="15d6b-139">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="15d6b-140">可用于跨服务跟踪日志。</span><span class="sxs-lookup"><span data-stu-id="15d6b-140">Can be used to trace logs across services.</span></span>                                                                                                                                    |
| <span data-ttu-id="15d6b-141">id</span><span class="sxs-lookup"><span data-stu-id="15d6b-141">id</span></span>                  | <span data-ttu-id="15d6b-142">String</span><span class="sxs-lookup"><span data-stu-id="15d6b-142">String</span></span>                                              | <span data-ttu-id="15d6b-143">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="15d6b-143">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="15d6b-144">这是 GUID。</span><span class="sxs-lookup"><span data-stu-id="15d6b-144">This is a GUID.</span></span>                                                                                                                                                                                                              |
| <span data-ttu-id="15d6b-145">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="15d6b-145">initiatedBy</span></span>         | [<span data-ttu-id="15d6b-146">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="15d6b-146">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="15d6b-147">指示有关启动活动的用户或应用的信息。</span><span class="sxs-lookup"><span data-stu-id="15d6b-147">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                    |
| <span data-ttu-id="15d6b-148">loggedByService</span><span class="sxs-lookup"><span data-stu-id="15d6b-148">loggedByService</span></span>     | <span data-ttu-id="15d6b-149">String</span><span class="sxs-lookup"><span data-stu-id="15d6b-149">String</span></span>                                              | <span data-ttu-id="15d6b-150">指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。</span><span class="sxs-lookup"><span data-stu-id="15d6b-150">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                          |
| <span data-ttu-id="15d6b-151">result</span><span class="sxs-lookup"><span data-stu-id="15d6b-151">result</span></span>              | <span data-ttu-id="15d6b-152">string</span><span class="sxs-lookup"><span data-stu-id="15d6b-152">string</span></span>                                              | <span data-ttu-id="15d6b-153">指示活动的结果。</span><span class="sxs-lookup"><span data-stu-id="15d6b-153">Indicates the result of the activity.</span></span> <span data-ttu-id="15d6b-154">可取值为：`success`、`failure`、`timeout`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="15d6b-154">Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                       |
| <span data-ttu-id="15d6b-155">resultReason</span><span class="sxs-lookup"><span data-stu-id="15d6b-155">resultReason</span></span>        | <span data-ttu-id="15d6b-156">String</span><span class="sxs-lookup"><span data-stu-id="15d6b-156">String</span></span>                                              | <span data-ttu-id="15d6b-157">如果结果为“失败”或“超时”，指示失败的原因。</span><span class="sxs-lookup"><span data-stu-id="15d6b-157">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>                                                                                                                                                                                              |
| <span data-ttu-id="15d6b-158">targetResources</span><span class="sxs-lookup"><span data-stu-id="15d6b-158">targetResources</span></span>     | <span data-ttu-id="15d6b-159">[targetResource](targetresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15d6b-159">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="15d6b-160">指示由于活动而更改的资源的信息。</span><span class="sxs-lookup"><span data-stu-id="15d6b-160">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="15d6b-161">目标资源类型可以是用户、设备、目录、应用、角色、组、策略或其他。</span><span class="sxs-lookup"><span data-stu-id="15d6b-161">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>                                                                                                       |

## <a name="relationships"></a><span data-ttu-id="15d6b-162">关系</span><span class="sxs-lookup"><span data-stu-id="15d6b-162">Relationships</span></span>
<span data-ttu-id="15d6b-163">无</span><span class="sxs-lookup"><span data-stu-id="15d6b-163">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="15d6b-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15d6b-164">JSON representation</span></span>

<span data-ttu-id="15d6b-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15d6b-165">Here is a JSON representation of the resource.</span></span>

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


