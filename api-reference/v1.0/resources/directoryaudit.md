---
title: directoryAudit 资源类型
description: 表示目录审核项及其集合。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f49229ed1ce461a0e9dcc104087ec89726597267
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629290"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="2813c-103">directoryAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="2813c-103">directoryAudit resource type</span></span>

<span data-ttu-id="2813c-104">表示目录审核项及其集合。</span><span class="sxs-lookup"><span data-stu-id="2813c-104">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="2813c-105">方法</span><span class="sxs-lookup"><span data-stu-id="2813c-105">Methods</span></span>

| <span data-ttu-id="2813c-106">方法</span><span class="sxs-lookup"><span data-stu-id="2813c-106">Method</span></span>           | <span data-ttu-id="2813c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2813c-107">Return Type</span></span>    |<span data-ttu-id="2813c-108">说明</span><span class="sxs-lookup"><span data-stu-id="2813c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2813c-109">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="2813c-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="2813c-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="2813c-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="2813c-111">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="2813c-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="2813c-112">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="2813c-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="2813c-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="2813c-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="2813c-114">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="2813c-114">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="2813c-115">属性</span><span class="sxs-lookup"><span data-stu-id="2813c-115">Properties</span></span>

| <span data-ttu-id="2813c-116">属性</span><span class="sxs-lookup"><span data-stu-id="2813c-116">Property</span></span>     | <span data-ttu-id="2813c-117">类型</span><span class="sxs-lookup"><span data-stu-id="2813c-117">Type</span></span>   |<span data-ttu-id="2813c-118">说明</span><span class="sxs-lookup"><span data-stu-id="2813c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2813c-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="2813c-119">activityDateTime</span></span>|<span data-ttu-id="2813c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2813c-120">DateTimeOffset</span></span>|<span data-ttu-id="2813c-121">指示执行活动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2813c-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="2813c-122">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2813c-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="2813c-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2813c-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2813c-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="2813c-124">activityDisplayName</span></span>|<span data-ttu-id="2813c-125">String</span><span class="sxs-lookup"><span data-stu-id="2813c-125">String</span></span>|<span data-ttu-id="2813c-126">指示活动名称或操作名称 (示例: "创建用户" 和 "将成员添加到组")。</span><span class="sxs-lookup"><span data-stu-id="2813c-126">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="2813c-127">有关完整列表, 请参阅[AZURE AD 活动列表](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。</span><span class="sxs-lookup"><span data-stu-id="2813c-127">For full list, see [Azure AD activity list](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="2813c-128">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="2813c-128">additionalDetails</span></span>|<span data-ttu-id="2813c-129">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2813c-129">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="2813c-130">指示活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="2813c-130">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="2813c-131">category</span><span class="sxs-lookup"><span data-stu-id="2813c-131">category</span></span>|<span data-ttu-id="2813c-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2813c-132">String</span></span>|<span data-ttu-id="2813c-133">指示活动所针对的资源类别。</span><span class="sxs-lookup"><span data-stu-id="2813c-133">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="2813c-134">（例如：用户管理、组管理等。）</span><span class="sxs-lookup"><span data-stu-id="2813c-134">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="2813c-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="2813c-135">correlationId</span></span>|<span data-ttu-id="2813c-136">GUID</span><span class="sxs-lookup"><span data-stu-id="2813c-136">GUID</span></span>|<span data-ttu-id="2813c-137">指示有助于关联跨各种服务的活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2813c-137">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="2813c-138">可用于跨服务跟踪日志。</span><span class="sxs-lookup"><span data-stu-id="2813c-138">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="2813c-139">id</span><span class="sxs-lookup"><span data-stu-id="2813c-139">id</span></span>|<span data-ttu-id="2813c-140">String</span><span class="sxs-lookup"><span data-stu-id="2813c-140">String</span></span>| <span data-ttu-id="2813c-141">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2813c-141">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="2813c-142">这是 GUID。</span><span class="sxs-lookup"><span data-stu-id="2813c-142">This is a GUID.</span></span>|
|<span data-ttu-id="2813c-143">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="2813c-143">initiatedBy</span></span>|[<span data-ttu-id="2813c-144">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="2813c-144">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="2813c-145">指示有关启动活动的用户或应用的信息。</span><span class="sxs-lookup"><span data-stu-id="2813c-145">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="2813c-146">loggedByService</span><span class="sxs-lookup"><span data-stu-id="2813c-146">loggedByService</span></span>|<span data-ttu-id="2813c-147">String</span><span class="sxs-lookup"><span data-stu-id="2813c-147">String</span></span>|<span data-ttu-id="2813c-148">指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。</span><span class="sxs-lookup"><span data-stu-id="2813c-148">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="2813c-149">result</span><span class="sxs-lookup"><span data-stu-id="2813c-149">result</span></span>|<span data-ttu-id="2813c-150">string</span><span class="sxs-lookup"><span data-stu-id="2813c-150">string</span></span>| <span data-ttu-id="2813c-151">指示活动的结果。可取值为：`success`、`failure`、`timeout`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2813c-151">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="2813c-152">resultReason</span><span class="sxs-lookup"><span data-stu-id="2813c-152">resultReason</span></span>|<span data-ttu-id="2813c-153">String</span><span class="sxs-lookup"><span data-stu-id="2813c-153">String</span></span>|<span data-ttu-id="2813c-154">描述 "失败" 或 "超时" 结果的原因。</span><span class="sxs-lookup"><span data-stu-id="2813c-154">Describes cause of "failure" or "timeout" results.</span></span>|
|<span data-ttu-id="2813c-155">targetResources</span><span class="sxs-lookup"><span data-stu-id="2813c-155">targetResources</span></span>|<span data-ttu-id="2813c-156">[targetResource](targetresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2813c-156">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="2813c-157">指示由于活动而更改的资源的信息。</span><span class="sxs-lookup"><span data-stu-id="2813c-157">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="2813c-158">目标资源类型可以是用户、设备、目录、应用、角色、组、策略或其他。</span><span class="sxs-lookup"><span data-stu-id="2813c-158">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="2813c-159">关系</span><span class="sxs-lookup"><span data-stu-id="2813c-159">Relationships</span></span>

<span data-ttu-id="2813c-160">无</span><span class="sxs-lookup"><span data-stu-id="2813c-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2813c-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2813c-161">JSON representation</span></span>

<span data-ttu-id="2813c-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2813c-162">Here is a JSON representation of the resource.</span></span>

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
