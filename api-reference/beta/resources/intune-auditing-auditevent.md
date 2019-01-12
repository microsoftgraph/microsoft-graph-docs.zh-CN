---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b659367c9274e8564116eea9351058be59b6dd68
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960763"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="d9e19-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9e19-103">auditEvent resource type</span></span>

> <span data-ttu-id="d9e19-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9e19-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9e19-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9e19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9e19-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9e19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9e19-107">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="d9e19-107">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="d9e19-108">方法</span><span class="sxs-lookup"><span data-stu-id="d9e19-108">Methods</span></span>
|<span data-ttu-id="d9e19-109">方法</span><span class="sxs-lookup"><span data-stu-id="d9e19-109">Method</span></span>|<span data-ttu-id="d9e19-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9e19-110">Return Type</span></span>|<span data-ttu-id="d9e19-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9e19-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9e19-112">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="d9e19-112">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="d9e19-113">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9e19-113">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="d9e19-114">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9e19-114">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="d9e19-115">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-115">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="d9e19-116">auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-116">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="d9e19-117">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9e19-117">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="d9e19-118">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-118">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="d9e19-119">auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-119">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="d9e19-120">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e19-120">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="d9e19-121">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-121">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="d9e19-122">无</span><span class="sxs-lookup"><span data-stu-id="d9e19-122">None</span></span>|<span data-ttu-id="d9e19-123">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="d9e19-123">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="d9e19-124">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-124">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="d9e19-125">auditEvent</span><span class="sxs-lookup"><span data-stu-id="d9e19-125">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="d9e19-126">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e19-126">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="d9e19-127">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="d9e19-127">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="d9e19-128">String collection</span><span class="sxs-lookup"><span data-stu-id="d9e19-128">String collection</span></span>|<span data-ttu-id="d9e19-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9e19-129">Not yet documented</span></span>|
|[<span data-ttu-id="d9e19-130">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="d9e19-130">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="d9e19-131">String collection</span><span class="sxs-lookup"><span data-stu-id="d9e19-131">String collection</span></span>|<span data-ttu-id="d9e19-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9e19-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d9e19-133">属性</span><span class="sxs-lookup"><span data-stu-id="d9e19-133">Properties</span></span>
|<span data-ttu-id="d9e19-134">属性</span><span class="sxs-lookup"><span data-stu-id="d9e19-134">Property</span></span>|<span data-ttu-id="d9e19-135">类型</span><span class="sxs-lookup"><span data-stu-id="d9e19-135">Type</span></span>|<span data-ttu-id="d9e19-136">说明</span><span class="sxs-lookup"><span data-stu-id="d9e19-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e19-137">id</span><span class="sxs-lookup"><span data-stu-id="d9e19-137">id</span></span>|<span data-ttu-id="d9e19-138">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-138">String</span></span>|<span data-ttu-id="d9e19-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9e19-139">Key of the entity.</span></span>|
|<span data-ttu-id="d9e19-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d9e19-140">displayName</span></span>|<span data-ttu-id="d9e19-141">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-141">String</span></span>|<span data-ttu-id="d9e19-142">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9e19-142">Event display name.</span></span>|
|<span data-ttu-id="d9e19-143">componentName</span><span class="sxs-lookup"><span data-stu-id="d9e19-143">componentName</span></span>|<span data-ttu-id="d9e19-144">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-144">String</span></span>|<span data-ttu-id="d9e19-145">组件名称。</span><span class="sxs-lookup"><span data-stu-id="d9e19-145">Component name.</span></span>|
|<span data-ttu-id="d9e19-146">actor</span><span class="sxs-lookup"><span data-stu-id="d9e19-146">actor</span></span>|[<span data-ttu-id="d9e19-147">auditActor</span><span class="sxs-lookup"><span data-stu-id="d9e19-147">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="d9e19-148">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="d9e19-148">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="d9e19-149">activity</span><span class="sxs-lookup"><span data-stu-id="d9e19-149">activity</span></span>|<span data-ttu-id="d9e19-150">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-150">String</span></span>|<span data-ttu-id="d9e19-151">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d9e19-151">Friendly name of the activity.</span></span>|
|<span data-ttu-id="d9e19-152">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e19-152">activityDateTime</span></span>|<span data-ttu-id="d9e19-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e19-153">DateTimeOffset</span></span>|<span data-ttu-id="d9e19-154">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="d9e19-154">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="d9e19-155">activityType</span><span class="sxs-lookup"><span data-stu-id="d9e19-155">activityType</span></span>|<span data-ttu-id="d9e19-156">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-156">String</span></span>|<span data-ttu-id="d9e19-157">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="d9e19-157">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="d9e19-158">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="d9e19-158">activityOperationType</span></span>|<span data-ttu-id="d9e19-159">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-159">String</span></span>|<span data-ttu-id="d9e19-160">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="d9e19-160">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="d9e19-161">activityResult</span><span class="sxs-lookup"><span data-stu-id="d9e19-161">activityResult</span></span>|<span data-ttu-id="d9e19-162">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-162">String</span></span>|<span data-ttu-id="d9e19-163">活动结果。</span><span class="sxs-lookup"><span data-stu-id="d9e19-163">The result of the activity.</span></span>|
|<span data-ttu-id="d9e19-164">correlationId</span><span class="sxs-lookup"><span data-stu-id="d9e19-164">correlationId</span></span>|<span data-ttu-id="d9e19-165">Guid</span><span class="sxs-lookup"><span data-stu-id="d9e19-165">Guid</span></span>|<span data-ttu-id="d9e19-166">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="d9e19-166">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="d9e19-167">resources</span><span class="sxs-lookup"><span data-stu-id="d9e19-167">resources</span></span>|<span data-ttu-id="d9e19-168">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9e19-168">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="d9e19-169">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="d9e19-169">Resources being modified.</span></span>|
|<span data-ttu-id="d9e19-170">category</span><span class="sxs-lookup"><span data-stu-id="d9e19-170">category</span></span>|<span data-ttu-id="d9e19-171">String</span><span class="sxs-lookup"><span data-stu-id="d9e19-171">String</span></span>|<span data-ttu-id="d9e19-172">审核类别。</span><span class="sxs-lookup"><span data-stu-id="d9e19-172">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9e19-173">关系</span><span class="sxs-lookup"><span data-stu-id="d9e19-173">Relationships</span></span>
<span data-ttu-id="d9e19-174">无</span><span class="sxs-lookup"><span data-stu-id="d9e19-174">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9e19-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9e19-175">JSON Representation</span></span>
<span data-ttu-id="d9e19-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9e19-176">Here is a JSON representation of the resource.</span></span>
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





