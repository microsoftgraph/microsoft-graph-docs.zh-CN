---
title: directoryAudit 资源类型
description: 此资源表示的目录审核项，并且其集合
ms.openlocfilehash: 8656bd910cd5b84d7760f973b160d91efe08abe1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041262"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="80197-103">directoryAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="80197-103">directoryAudit resource type</span></span>
<span data-ttu-id="80197-104">此资源表示的目录审核项，并且其集合</span><span class="sxs-lookup"><span data-stu-id="80197-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="80197-105">方法</span><span class="sxs-lookup"><span data-stu-id="80197-105">Methods</span></span>

| <span data-ttu-id="80197-106">方法</span><span class="sxs-lookup"><span data-stu-id="80197-106">Method</span></span>           | <span data-ttu-id="80197-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="80197-107">Return Type</span></span>    |<span data-ttu-id="80197-108">说明</span><span class="sxs-lookup"><span data-stu-id="80197-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80197-109">列表 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="80197-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="80197-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="80197-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="80197-111">列表中的集合，及其属性的目录审核项。</span><span class="sxs-lookup"><span data-stu-id="80197-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="80197-112">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="80197-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="80197-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="80197-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="80197-114">获取特定目录审核项和其属性。</span><span class="sxs-lookup"><span data-stu-id="80197-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="80197-115">属性</span><span class="sxs-lookup"><span data-stu-id="80197-115">Properties</span></span>
| <span data-ttu-id="80197-116">属性</span><span class="sxs-lookup"><span data-stu-id="80197-116">Property</span></span>     | <span data-ttu-id="80197-117">类型</span><span class="sxs-lookup"><span data-stu-id="80197-117">Type</span></span>   |<span data-ttu-id="80197-118">说明</span><span class="sxs-lookup"><span data-stu-id="80197-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80197-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="80197-119">activityDateTime</span></span>|<span data-ttu-id="80197-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80197-120">DateTimeOffset</span></span>|<span data-ttu-id="80197-121">指示的日期和时间执行活动。</span><span class="sxs-lookup"><span data-stu-id="80197-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="80197-122">时间戳类型始终为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="80197-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="80197-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="80197-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="80197-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="80197-124">activityDisplayName</span></span>|<span data-ttu-id="80197-125">字符串</span><span class="sxs-lookup"><span data-stu-id="80197-125">String</span></span>|<span data-ttu-id="80197-126">指示活动名称或操作名称 （例如</span><span class="sxs-lookup"><span data-stu-id="80197-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="80197-127">"创建用户"，"向组添加成员")。</span><span class="sxs-lookup"><span data-stu-id="80197-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="80197-128">有关记录的活动的列表，请参阅[Azure Ad 活动列表](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。</span><span class="sxs-lookup"><span data-stu-id="80197-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="80197-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="80197-129">additionalDetails</span></span>|<span data-ttu-id="80197-130">[keyValue](keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="80197-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="80197-131">指示活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="80197-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="80197-132">category</span><span class="sxs-lookup"><span data-stu-id="80197-132">category</span></span>|<span data-ttu-id="80197-133">String</span><span class="sxs-lookup"><span data-stu-id="80197-133">String</span></span>|<span data-ttu-id="80197-134">指示活动所针对的资源类别。</span><span class="sxs-lookup"><span data-stu-id="80197-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="80197-135">(例如： 用户管理、 组管理等。。)</span><span class="sxs-lookup"><span data-stu-id="80197-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="80197-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="80197-136">correlationId</span></span>|<span data-ttu-id="80197-137">GUID</span><span class="sxs-lookup"><span data-stu-id="80197-137">GUID</span></span>|<span data-ttu-id="80197-138">指示帮助关联跨越各种服务的活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="80197-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="80197-139">可以使用跟踪日志服务。</span><span class="sxs-lookup"><span data-stu-id="80197-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="80197-140">id</span><span class="sxs-lookup"><span data-stu-id="80197-140">id</span></span>|<span data-ttu-id="80197-141">字符串</span><span class="sxs-lookup"><span data-stu-id="80197-141">String</span></span>| <span data-ttu-id="80197-142">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="80197-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="80197-143">这是一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="80197-143">This is a GUID.</span></span>|
|<span data-ttu-id="80197-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="80197-144">initiatedBy</span></span>|[<span data-ttu-id="80197-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="80197-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="80197-146">指示信息的用户或应用程序启动活动。</span><span class="sxs-lookup"><span data-stu-id="80197-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="80197-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="80197-147">loggedByService</span></span>|<span data-ttu-id="80197-148">字符串</span><span class="sxs-lookup"><span data-stu-id="80197-148">String</span></span>|<span data-ttu-id="80197-149">指示服务在其启动活动的信息 (例如： 自助服务密码管理、 核心目录、 B2C、 邀请用户、 Microsoft Identity Manager、 特权身份管理。</span><span class="sxs-lookup"><span data-stu-id="80197-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="80197-150">result</span><span class="sxs-lookup"><span data-stu-id="80197-150">result</span></span>|<span data-ttu-id="80197-151">string</span><span class="sxs-lookup"><span data-stu-id="80197-151">string</span></span>| <span data-ttu-id="80197-152">指示活动的结果。可能的值为： `success`， `failure`， `timeout`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="80197-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="80197-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="80197-153">resultReason</span></span>|<span data-ttu-id="80197-154">字符串</span><span class="sxs-lookup"><span data-stu-id="80197-154">String</span></span>|<span data-ttu-id="80197-155">如果结果为"Failure"或"超时"，指示失败的原因。</span><span class="sxs-lookup"><span data-stu-id="80197-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="80197-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="80197-156">targetResources</span></span>|<span data-ttu-id="80197-157">[targetResource](targetresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="80197-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="80197-158">指示由于活动更改资源的信息。</span><span class="sxs-lookup"><span data-stu-id="80197-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="80197-159">目标资源类型可以是用户、 设备、 目录、 应用程序、 角色、 组、 策略或其他。</span><span class="sxs-lookup"><span data-stu-id="80197-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="80197-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="80197-160">Relationships</span></span>
<span data-ttu-id="80197-161">无</span><span class="sxs-lookup"><span data-stu-id="80197-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="80197-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80197-162">JSON representation</span></span>

<span data-ttu-id="80197-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80197-163">Here is a JSON representation of the resource.</span></span>

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