---
title: directoryAudit 资源类型
description: 表示目录审核项目及其集合。
author: SarahBar
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 102399d92b8287c7e82a5ae9323c0e827133a50a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131283"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="2a052-103">directoryAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a052-103">directoryAudit resource type</span></span>

<span data-ttu-id="2a052-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a052-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a052-105">表示目录审核项目及其集合。</span><span class="sxs-lookup"><span data-stu-id="2a052-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="2a052-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2a052-106">Methods</span></span>

| <span data-ttu-id="2a052-107">方法</span><span class="sxs-lookup"><span data-stu-id="2a052-107">Method</span></span>           | <span data-ttu-id="2a052-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a052-108">Return Type</span></span>    |<span data-ttu-id="2a052-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a052-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a052-110">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="2a052-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="2a052-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="2a052-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="2a052-112">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="2a052-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="2a052-113">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="2a052-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="2a052-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="2a052-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="2a052-115">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="2a052-115">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a052-116">属性</span><span class="sxs-lookup"><span data-stu-id="2a052-116">Properties</span></span>

| <span data-ttu-id="2a052-117">属性</span><span class="sxs-lookup"><span data-stu-id="2a052-117">Property</span></span>            | <span data-ttu-id="2a052-118">类型</span><span class="sxs-lookup"><span data-stu-id="2a052-118">Type</span></span>                                                | <span data-ttu-id="2a052-119">说明</span><span class="sxs-lookup"><span data-stu-id="2a052-119">Description</span></span>                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2a052-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="2a052-120">activityDateTime</span></span>    | <span data-ttu-id="2a052-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a052-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="2a052-122">指示执行活动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2a052-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="2a052-123">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2a052-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="2a052-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2a052-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>                                                                                          |
| <span data-ttu-id="2a052-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a052-125">activityDisplayName</span></span> | <span data-ttu-id="2a052-126">String</span><span class="sxs-lookup"><span data-stu-id="2a052-126">String</span></span>                                              | <span data-ttu-id="2a052-127">指示活动名称或操作名称 (示例："创建用户"和"向组添加成员") 。</span><span class="sxs-lookup"><span data-stu-id="2a052-127">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="2a052-128">有关完整列表，请参阅 [Azure AD 活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。</span><span class="sxs-lookup"><span data-stu-id="2a052-128">For full list, see [Azure AD activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="2a052-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="2a052-129">additionalDetails</span></span>   | <span data-ttu-id="2a052-130">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a052-130">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="2a052-131">指示活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="2a052-131">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                                      |
| <span data-ttu-id="2a052-132">category</span><span class="sxs-lookup"><span data-stu-id="2a052-132">category</span></span>            | <span data-ttu-id="2a052-133">String</span><span class="sxs-lookup"><span data-stu-id="2a052-133">String</span></span>                                              | <span data-ttu-id="2a052-134">指示活动所针对的资源类别。</span><span class="sxs-lookup"><span data-stu-id="2a052-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="2a052-135">（例如：用户管理、组管理等。）</span><span class="sxs-lookup"><span data-stu-id="2a052-135">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                                          |
| <span data-ttu-id="2a052-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="2a052-136">correlationId</span></span>       | <span data-ttu-id="2a052-137">GUID</span><span class="sxs-lookup"><span data-stu-id="2a052-137">GUID</span></span>                                                | <span data-ttu-id="2a052-138">指示有助于关联跨各种服务的活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2a052-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="2a052-139">可用于跨服务跟踪日志。</span><span class="sxs-lookup"><span data-stu-id="2a052-139">Can be used to trace logs across services.</span></span>                                                                                                                                                |
| <span data-ttu-id="2a052-140">id</span><span class="sxs-lookup"><span data-stu-id="2a052-140">id</span></span>                  | <span data-ttu-id="2a052-141">String</span><span class="sxs-lookup"><span data-stu-id="2a052-141">String</span></span>                                              | <span data-ttu-id="2a052-142">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2a052-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="2a052-143">这是 GUID。</span><span class="sxs-lookup"><span data-stu-id="2a052-143">This is a GUID.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="2a052-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="2a052-144">initiatedBy</span></span>         | [<span data-ttu-id="2a052-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="2a052-145">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="2a052-146">指示有关启动活动的用户或应用的信息。</span><span class="sxs-lookup"><span data-stu-id="2a052-146">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                                |
| <span data-ttu-id="2a052-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="2a052-147">loggedByService</span></span>     | <span data-ttu-id="2a052-148">String</span><span class="sxs-lookup"><span data-stu-id="2a052-148">String</span></span>                                              | <span data-ttu-id="2a052-149">指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。</span><span class="sxs-lookup"><span data-stu-id="2a052-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                                      |
| <span data-ttu-id="2a052-150">result</span><span class="sxs-lookup"><span data-stu-id="2a052-150">result</span></span>              | <span data-ttu-id="2a052-151">string</span><span class="sxs-lookup"><span data-stu-id="2a052-151">string</span></span>                                              | <span data-ttu-id="2a052-152">指示活动的结果。</span><span class="sxs-lookup"><span data-stu-id="2a052-152">Indicates the result of the activity.</span></span> <span data-ttu-id="2a052-153">可取值为：`success`、`failure`、`timeout`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2a052-153">Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                                   |
| <span data-ttu-id="2a052-154">resultReason</span><span class="sxs-lookup"><span data-stu-id="2a052-154">resultReason</span></span>        | <span data-ttu-id="2a052-155">String</span><span class="sxs-lookup"><span data-stu-id="2a052-155">String</span></span>                                              | <span data-ttu-id="2a052-156">描述"失败"或"超时"结果的原因。</span><span class="sxs-lookup"><span data-stu-id="2a052-156">Describes cause of "failure" or "timeout" results.</span></span>                                                                                                                                                                                                                                 |
| <span data-ttu-id="2a052-157">targetResources</span><span class="sxs-lookup"><span data-stu-id="2a052-157">targetResources</span></span>     | <span data-ttu-id="2a052-158">[targetResource](targetresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2a052-158">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="2a052-159">指示由于活动而更改的资源的信息。</span><span class="sxs-lookup"><span data-stu-id="2a052-159">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="2a052-160">目标资源类型可以是用户、设备、目录、应用、角色、组、策略或其他。</span><span class="sxs-lookup"><span data-stu-id="2a052-160">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>                                                                                                                   |

## <a name="relationships"></a><span data-ttu-id="2a052-161">关系</span><span class="sxs-lookup"><span data-stu-id="2a052-161">Relationships</span></span>

<span data-ttu-id="2a052-162">无</span><span class="sxs-lookup"><span data-stu-id="2a052-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a052-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a052-163">JSON representation</span></span>

<span data-ttu-id="2a052-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a052-164">Here is a JSON representation of the resource.</span></span>

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
