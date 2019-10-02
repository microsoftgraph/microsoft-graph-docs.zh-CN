---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5dfadf90d2498fa13f2367ca7467bbce5f810e3f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355986"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="e96fb-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e96fb-103">auditEvent resource type</span></span>

> <span data-ttu-id="e96fb-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e96fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e96fb-105">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="e96fb-105">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="e96fb-106">方法</span><span class="sxs-lookup"><span data-stu-id="e96fb-106">Methods</span></span>
|<span data-ttu-id="e96fb-107">方法</span><span class="sxs-lookup"><span data-stu-id="e96fb-107">Method</span></span>|<span data-ttu-id="e96fb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e96fb-108">Return Type</span></span>|<span data-ttu-id="e96fb-109">说明</span><span class="sxs-lookup"><span data-stu-id="e96fb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e96fb-110">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="e96fb-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="e96fb-111">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e96fb-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="e96fb-112">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e96fb-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="e96fb-113">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="e96fb-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="e96fb-115">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e96fb-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="e96fb-116">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="e96fb-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="e96fb-118">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e96fb-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="e96fb-119">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="e96fb-120">无</span><span class="sxs-lookup"><span data-stu-id="e96fb-120">None</span></span>|<span data-ttu-id="e96fb-121">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="e96fb-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="e96fb-122">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="e96fb-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="e96fb-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="e96fb-124">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e96fb-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="e96fb-125">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="e96fb-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="e96fb-126">String collection</span><span class="sxs-lookup"><span data-stu-id="e96fb-126">String collection</span></span>|<span data-ttu-id="e96fb-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e96fb-127">Not yet documented</span></span>|
|[<span data-ttu-id="e96fb-128">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="e96fb-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="e96fb-129">String collection</span><span class="sxs-lookup"><span data-stu-id="e96fb-129">String collection</span></span>|<span data-ttu-id="e96fb-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e96fb-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e96fb-131">属性</span><span class="sxs-lookup"><span data-stu-id="e96fb-131">Properties</span></span>
|<span data-ttu-id="e96fb-132">属性</span><span class="sxs-lookup"><span data-stu-id="e96fb-132">Property</span></span>|<span data-ttu-id="e96fb-133">类型</span><span class="sxs-lookup"><span data-stu-id="e96fb-133">Type</span></span>|<span data-ttu-id="e96fb-134">说明</span><span class="sxs-lookup"><span data-stu-id="e96fb-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e96fb-135">id</span><span class="sxs-lookup"><span data-stu-id="e96fb-135">id</span></span>|<span data-ttu-id="e96fb-136">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-136">String</span></span>|<span data-ttu-id="e96fb-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e96fb-137">Key of the entity.</span></span>|
|<span data-ttu-id="e96fb-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e96fb-138">displayName</span></span>|<span data-ttu-id="e96fb-139">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-139">String</span></span>|<span data-ttu-id="e96fb-140">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="e96fb-140">Event display name.</span></span>|
|<span data-ttu-id="e96fb-141">componentName</span><span class="sxs-lookup"><span data-stu-id="e96fb-141">componentName</span></span>|<span data-ttu-id="e96fb-142">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-142">String</span></span>|<span data-ttu-id="e96fb-143">组件名称。</span><span class="sxs-lookup"><span data-stu-id="e96fb-143">Component name.</span></span>|
|<span data-ttu-id="e96fb-144">actor</span><span class="sxs-lookup"><span data-stu-id="e96fb-144">actor</span></span>|[<span data-ttu-id="e96fb-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="e96fb-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="e96fb-146">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="e96fb-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="e96fb-147">activity</span><span class="sxs-lookup"><span data-stu-id="e96fb-147">activity</span></span>|<span data-ttu-id="e96fb-148">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-148">String</span></span>|<span data-ttu-id="e96fb-149">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="e96fb-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="e96fb-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="e96fb-150">activityDateTime</span></span>|<span data-ttu-id="e96fb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e96fb-151">DateTimeOffset</span></span>|<span data-ttu-id="e96fb-152">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="e96fb-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="e96fb-153">activityType</span><span class="sxs-lookup"><span data-stu-id="e96fb-153">activityType</span></span>|<span data-ttu-id="e96fb-154">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-154">String</span></span>|<span data-ttu-id="e96fb-155">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="e96fb-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="e96fb-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="e96fb-156">activityOperationType</span></span>|<span data-ttu-id="e96fb-157">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-157">String</span></span>|<span data-ttu-id="e96fb-158">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="e96fb-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="e96fb-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="e96fb-159">activityResult</span></span>|<span data-ttu-id="e96fb-160">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-160">String</span></span>|<span data-ttu-id="e96fb-161">活动结果。</span><span class="sxs-lookup"><span data-stu-id="e96fb-161">The result of the activity.</span></span>|
|<span data-ttu-id="e96fb-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="e96fb-162">correlationId</span></span>|<span data-ttu-id="e96fb-163">Guid</span><span class="sxs-lookup"><span data-stu-id="e96fb-163">Guid</span></span>|<span data-ttu-id="e96fb-164">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="e96fb-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="e96fb-165">resources</span><span class="sxs-lookup"><span data-stu-id="e96fb-165">resources</span></span>|<span data-ttu-id="e96fb-166">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e96fb-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="e96fb-167">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="e96fb-167">Resources being modified.</span></span>|
|<span data-ttu-id="e96fb-168">“类别”</span><span class="sxs-lookup"><span data-stu-id="e96fb-168">category</span></span>|<span data-ttu-id="e96fb-169">String</span><span class="sxs-lookup"><span data-stu-id="e96fb-169">String</span></span>|<span data-ttu-id="e96fb-170">审核类别。</span><span class="sxs-lookup"><span data-stu-id="e96fb-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e96fb-171">关系</span><span class="sxs-lookup"><span data-stu-id="e96fb-171">Relationships</span></span>
<span data-ttu-id="e96fb-172">无</span><span class="sxs-lookup"><span data-stu-id="e96fb-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e96fb-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e96fb-173">JSON Representation</span></span>
<span data-ttu-id="e96fb-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e96fb-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```




