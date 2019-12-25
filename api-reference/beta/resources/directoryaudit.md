---
title: directoryAudit 资源类型
description: 介绍了 Microsoft Graph API （REST）的 directoryAudit 资源（实体），它可帮助审核目录（租户）活动（测试版）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fbd3789ca6a33a16f214d5d961986ef4e1b6c016
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870328"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="58e60-103">directoryAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="58e60-103">directoryAudit resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e60-104">表示目录审核项及其集合。</span><span class="sxs-lookup"><span data-stu-id="58e60-104">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="58e60-105">方法</span><span class="sxs-lookup"><span data-stu-id="58e60-105">Methods</span></span>

| <span data-ttu-id="58e60-106">方法</span><span class="sxs-lookup"><span data-stu-id="58e60-106">Method</span></span>           | <span data-ttu-id="58e60-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="58e60-107">Return Type</span></span>    |<span data-ttu-id="58e60-108">说明</span><span class="sxs-lookup"><span data-stu-id="58e60-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58e60-109">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="58e60-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="58e60-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="58e60-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="58e60-111">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="58e60-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="58e60-112">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="58e60-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="58e60-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="58e60-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="58e60-114">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="58e60-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="58e60-115">属性</span><span class="sxs-lookup"><span data-stu-id="58e60-115">Properties</span></span>
| <span data-ttu-id="58e60-116">属性</span><span class="sxs-lookup"><span data-stu-id="58e60-116">Property</span></span>     | <span data-ttu-id="58e60-117">类型</span><span class="sxs-lookup"><span data-stu-id="58e60-117">Type</span></span>   |<span data-ttu-id="58e60-118">说明</span><span class="sxs-lookup"><span data-stu-id="58e60-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58e60-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="58e60-119">activityDateTime</span></span>|<span data-ttu-id="58e60-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58e60-120">DateTimeOffset</span></span>|<span data-ttu-id="58e60-121">指示执行活动的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="58e60-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="58e60-122">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="58e60-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="58e60-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58e60-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58e60-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="58e60-124">activityDisplayName</span></span>|<span data-ttu-id="58e60-125">String</span><span class="sxs-lookup"><span data-stu-id="58e60-125">String</span></span>|<span data-ttu-id="58e60-126">指示活动名称或操作名称（例如，</span><span class="sxs-lookup"><span data-stu-id="58e60-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="58e60-127">“创建用户”、“向组中添加成员”）。</span><span class="sxs-lookup"><span data-stu-id="58e60-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="58e60-128">有关记录的活动列表，请参阅 [Azure AD 活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。</span><span class="sxs-lookup"><span data-stu-id="58e60-128">For a list of activities logged,refer to [Azure Ad activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="58e60-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="58e60-129">additionalDetails</span></span>|<span data-ttu-id="58e60-130">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58e60-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="58e60-131">指示活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="58e60-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="58e60-132">category</span><span class="sxs-lookup"><span data-stu-id="58e60-132">category</span></span>|<span data-ttu-id="58e60-133">String</span><span class="sxs-lookup"><span data-stu-id="58e60-133">String</span></span>|<span data-ttu-id="58e60-134">指示活动所针对的资源类别。</span><span class="sxs-lookup"><span data-stu-id="58e60-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="58e60-135">（例如：用户管理、组管理等。）</span><span class="sxs-lookup"><span data-stu-id="58e60-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="58e60-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="58e60-136">correlationId</span></span>|<span data-ttu-id="58e60-137">GUID</span><span class="sxs-lookup"><span data-stu-id="58e60-137">GUID</span></span>|<span data-ttu-id="58e60-138">指示有助于关联跨各种服务的活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="58e60-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="58e60-139">可用于跨服务跟踪日志。</span><span class="sxs-lookup"><span data-stu-id="58e60-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="58e60-140">id</span><span class="sxs-lookup"><span data-stu-id="58e60-140">id</span></span>|<span data-ttu-id="58e60-141">String</span><span class="sxs-lookup"><span data-stu-id="58e60-141">String</span></span>| <span data-ttu-id="58e60-142">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="58e60-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="58e60-143">这是 GUID。</span><span class="sxs-lookup"><span data-stu-id="58e60-143">This is a GUID.</span></span>|
|<span data-ttu-id="58e60-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="58e60-144">initiatedBy</span></span>|[<span data-ttu-id="58e60-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="58e60-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="58e60-146">指示有关启动活动的用户或应用的信息。</span><span class="sxs-lookup"><span data-stu-id="58e60-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="58e60-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="58e60-147">loggedByService</span></span>|<span data-ttu-id="58e60-148">String</span><span class="sxs-lookup"><span data-stu-id="58e60-148">String</span></span>|<span data-ttu-id="58e60-149">指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。</span><span class="sxs-lookup"><span data-stu-id="58e60-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="58e60-150">result</span><span class="sxs-lookup"><span data-stu-id="58e60-150">result</span></span>|<span data-ttu-id="58e60-151">string</span><span class="sxs-lookup"><span data-stu-id="58e60-151">string</span></span>| <span data-ttu-id="58e60-152">指示活动的结果。可取值为：`success`、`failure`、`timeout`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="58e60-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="58e60-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="58e60-153">resultReason</span></span>|<span data-ttu-id="58e60-154">String</span><span class="sxs-lookup"><span data-stu-id="58e60-154">String</span></span>|<span data-ttu-id="58e60-155">如果结果为“失败”或“超时”，指示失败的原因。</span><span class="sxs-lookup"><span data-stu-id="58e60-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="58e60-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="58e60-156">targetResources</span></span>|<span data-ttu-id="58e60-157">[targetResource](targetresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58e60-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="58e60-158">指示由于活动而更改的资源的信息。</span><span class="sxs-lookup"><span data-stu-id="58e60-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="58e60-159">目标资源类型可以是用户、设备、目录、应用、角色、组、策略或其他。</span><span class="sxs-lookup"><span data-stu-id="58e60-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="58e60-160">关系</span><span class="sxs-lookup"><span data-stu-id="58e60-160">Relationships</span></span>
<span data-ttu-id="58e60-161">无</span><span class="sxs-lookup"><span data-stu-id="58e60-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="58e60-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58e60-162">JSON representation</span></span>

<span data-ttu-id="58e60-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58e60-163">Here is a JSON representation of the resource.</span></span>

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
