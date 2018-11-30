---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
ms.openlocfilehash: 96e8ad79dccd1b85ea848c6a975e4ee8d5217738
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007786"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="f9fe1-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9fe1-103">auditEvent resource type</span></span>

> <span data-ttu-id="f9fe1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9fe1-105">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-105">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="f9fe1-106">方法</span><span class="sxs-lookup"><span data-stu-id="f9fe1-106">Methods</span></span>
|<span data-ttu-id="f9fe1-107">方法</span><span class="sxs-lookup"><span data-stu-id="f9fe1-107">Method</span></span>|<span data-ttu-id="f9fe1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9fe1-108">Return Type</span></span>|<span data-ttu-id="f9fe1-109">说明</span><span class="sxs-lookup"><span data-stu-id="f9fe1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9fe1-110">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="f9fe1-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="f9fe1-111">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f9fe1-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="f9fe1-112">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="f9fe1-113">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="f9fe1-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="f9fe1-115">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="f9fe1-116">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="f9fe1-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="f9fe1-118">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="f9fe1-119">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="f9fe1-120">无</span><span class="sxs-lookup"><span data-stu-id="f9fe1-120">None</span></span>|<span data-ttu-id="f9fe1-121">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="f9fe1-122">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="f9fe1-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="f9fe1-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="f9fe1-124">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="f9fe1-125">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="f9fe1-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="f9fe1-126">String collection</span><span class="sxs-lookup"><span data-stu-id="f9fe1-126">String collection</span></span>|<span data-ttu-id="f9fe1-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9fe1-127">Not yet documented</span></span>|
|[<span data-ttu-id="f9fe1-128">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="f9fe1-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="f9fe1-129">String collection</span><span class="sxs-lookup"><span data-stu-id="f9fe1-129">String collection</span></span>|<span data-ttu-id="f9fe1-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9fe1-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f9fe1-131">属性</span><span class="sxs-lookup"><span data-stu-id="f9fe1-131">Properties</span></span>
|<span data-ttu-id="f9fe1-132">属性</span><span class="sxs-lookup"><span data-stu-id="f9fe1-132">Property</span></span>|<span data-ttu-id="f9fe1-133">类型</span><span class="sxs-lookup"><span data-stu-id="f9fe1-133">Type</span></span>|<span data-ttu-id="f9fe1-134">说明</span><span class="sxs-lookup"><span data-stu-id="f9fe1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9fe1-135">id</span><span class="sxs-lookup"><span data-stu-id="f9fe1-135">id</span></span>|<span data-ttu-id="f9fe1-136">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-136">String</span></span>|<span data-ttu-id="f9fe1-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-137">Key of the entity.</span></span>|
|<span data-ttu-id="f9fe1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f9fe1-138">displayName</span></span>|<span data-ttu-id="f9fe1-139">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-139">String</span></span>|<span data-ttu-id="f9fe1-140">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-140">Event display name.</span></span>|
|<span data-ttu-id="f9fe1-141">componentName</span><span class="sxs-lookup"><span data-stu-id="f9fe1-141">componentName</span></span>|<span data-ttu-id="f9fe1-142">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-142">String</span></span>|<span data-ttu-id="f9fe1-143">组件名称。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-143">Component name.</span></span>|
|<span data-ttu-id="f9fe1-144">actor</span><span class="sxs-lookup"><span data-stu-id="f9fe1-144">actor</span></span>|[<span data-ttu-id="f9fe1-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="f9fe1-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="f9fe1-146">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="f9fe1-147">activity</span><span class="sxs-lookup"><span data-stu-id="f9fe1-147">activity</span></span>|<span data-ttu-id="f9fe1-148">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-148">String</span></span>|<span data-ttu-id="f9fe1-149">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="f9fe1-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="f9fe1-150">activityDateTime</span></span>|<span data-ttu-id="f9fe1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9fe1-151">DateTimeOffset</span></span>|<span data-ttu-id="f9fe1-152">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="f9fe1-153">activityType</span><span class="sxs-lookup"><span data-stu-id="f9fe1-153">activityType</span></span>|<span data-ttu-id="f9fe1-154">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-154">String</span></span>|<span data-ttu-id="f9fe1-155">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="f9fe1-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="f9fe1-156">activityOperationType</span></span>|<span data-ttu-id="f9fe1-157">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-157">String</span></span>|<span data-ttu-id="f9fe1-158">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="f9fe1-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="f9fe1-159">activityResult</span></span>|<span data-ttu-id="f9fe1-160">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-160">String</span></span>|<span data-ttu-id="f9fe1-161">活动结果。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-161">The result of the activity.</span></span>|
|<span data-ttu-id="f9fe1-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="f9fe1-162">correlationId</span></span>|<span data-ttu-id="f9fe1-163">Guid</span><span class="sxs-lookup"><span data-stu-id="f9fe1-163">Guid</span></span>|<span data-ttu-id="f9fe1-164">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="f9fe1-165">resources</span><span class="sxs-lookup"><span data-stu-id="f9fe1-165">resources</span></span>|<span data-ttu-id="f9fe1-166">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f9fe1-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="f9fe1-167">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-167">Resources being modified.</span></span>|
|<span data-ttu-id="f9fe1-168">category</span><span class="sxs-lookup"><span data-stu-id="f9fe1-168">category</span></span>|<span data-ttu-id="f9fe1-169">String</span><span class="sxs-lookup"><span data-stu-id="f9fe1-169">String</span></span>|<span data-ttu-id="f9fe1-170">审核类别。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9fe1-171">关系</span><span class="sxs-lookup"><span data-stu-id="f9fe1-171">Relationships</span></span>
<span data-ttu-id="f9fe1-172">无</span><span class="sxs-lookup"><span data-stu-id="f9fe1-172">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9fe1-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9fe1-173">JSON Representation</span></span>
<span data-ttu-id="f9fe1-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9fe1-174">Here is a JSON representation of the resource.</span></span>
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



