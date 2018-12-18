---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: tfitzmac
ms.openlocfilehash: c19a7914790d7659a7b60000a81655d81a5dce52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351434"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="826b6-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="826b6-103">auditEvent resource type</span></span>

> <span data-ttu-id="826b6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="826b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="826b6-105">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="826b6-105">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="826b6-106">方法</span><span class="sxs-lookup"><span data-stu-id="826b6-106">Methods</span></span>
|<span data-ttu-id="826b6-107">方法</span><span class="sxs-lookup"><span data-stu-id="826b6-107">Method</span></span>|<span data-ttu-id="826b6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="826b6-108">Return Type</span></span>|<span data-ttu-id="826b6-109">说明</span><span class="sxs-lookup"><span data-stu-id="826b6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="826b6-110">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="826b6-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="826b6-111">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="826b6-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="826b6-112">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="826b6-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="826b6-113">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="826b6-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="826b6-115">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="826b6-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="826b6-116">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="826b6-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="826b6-118">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="826b6-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="826b6-119">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="826b6-120">无</span><span class="sxs-lookup"><span data-stu-id="826b6-120">None</span></span>|<span data-ttu-id="826b6-121">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="826b6-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="826b6-122">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="826b6-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="826b6-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="826b6-124">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="826b6-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="826b6-125">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="826b6-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="826b6-126">String collection</span><span class="sxs-lookup"><span data-stu-id="826b6-126">String collection</span></span>|<span data-ttu-id="826b6-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="826b6-127">Not yet documented</span></span>|
|[<span data-ttu-id="826b6-128">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="826b6-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="826b6-129">String collection</span><span class="sxs-lookup"><span data-stu-id="826b6-129">String collection</span></span>|<span data-ttu-id="826b6-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="826b6-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="826b6-131">属性</span><span class="sxs-lookup"><span data-stu-id="826b6-131">Properties</span></span>
|<span data-ttu-id="826b6-132">属性</span><span class="sxs-lookup"><span data-stu-id="826b6-132">Property</span></span>|<span data-ttu-id="826b6-133">类型</span><span class="sxs-lookup"><span data-stu-id="826b6-133">Type</span></span>|<span data-ttu-id="826b6-134">说明</span><span class="sxs-lookup"><span data-stu-id="826b6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="826b6-135">id</span><span class="sxs-lookup"><span data-stu-id="826b6-135">id</span></span>|<span data-ttu-id="826b6-136">String</span><span class="sxs-lookup"><span data-stu-id="826b6-136">String</span></span>|<span data-ttu-id="826b6-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="826b6-137">Key of the entity.</span></span>|
|<span data-ttu-id="826b6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="826b6-138">displayName</span></span>|<span data-ttu-id="826b6-139">String</span><span class="sxs-lookup"><span data-stu-id="826b6-139">String</span></span>|<span data-ttu-id="826b6-140">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="826b6-140">Event display name.</span></span>|
|<span data-ttu-id="826b6-141">componentName</span><span class="sxs-lookup"><span data-stu-id="826b6-141">componentName</span></span>|<span data-ttu-id="826b6-142">String</span><span class="sxs-lookup"><span data-stu-id="826b6-142">String</span></span>|<span data-ttu-id="826b6-143">组件名称。</span><span class="sxs-lookup"><span data-stu-id="826b6-143">Component name.</span></span>|
|<span data-ttu-id="826b6-144">actor</span><span class="sxs-lookup"><span data-stu-id="826b6-144">actor</span></span>|[<span data-ttu-id="826b6-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="826b6-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="826b6-146">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="826b6-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="826b6-147">activity</span><span class="sxs-lookup"><span data-stu-id="826b6-147">activity</span></span>|<span data-ttu-id="826b6-148">String</span><span class="sxs-lookup"><span data-stu-id="826b6-148">String</span></span>|<span data-ttu-id="826b6-149">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="826b6-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="826b6-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="826b6-150">activityDateTime</span></span>|<span data-ttu-id="826b6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="826b6-151">DateTimeOffset</span></span>|<span data-ttu-id="826b6-152">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="826b6-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="826b6-153">activityType</span><span class="sxs-lookup"><span data-stu-id="826b6-153">activityType</span></span>|<span data-ttu-id="826b6-154">String</span><span class="sxs-lookup"><span data-stu-id="826b6-154">String</span></span>|<span data-ttu-id="826b6-155">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="826b6-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="826b6-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="826b6-156">activityOperationType</span></span>|<span data-ttu-id="826b6-157">String</span><span class="sxs-lookup"><span data-stu-id="826b6-157">String</span></span>|<span data-ttu-id="826b6-158">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="826b6-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="826b6-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="826b6-159">activityResult</span></span>|<span data-ttu-id="826b6-160">String</span><span class="sxs-lookup"><span data-stu-id="826b6-160">String</span></span>|<span data-ttu-id="826b6-161">活动结果。</span><span class="sxs-lookup"><span data-stu-id="826b6-161">The result of the activity.</span></span>|
|<span data-ttu-id="826b6-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="826b6-162">correlationId</span></span>|<span data-ttu-id="826b6-163">Guid</span><span class="sxs-lookup"><span data-stu-id="826b6-163">Guid</span></span>|<span data-ttu-id="826b6-164">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="826b6-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="826b6-165">resources</span><span class="sxs-lookup"><span data-stu-id="826b6-165">resources</span></span>|<span data-ttu-id="826b6-166">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="826b6-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="826b6-167">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="826b6-167">Resources being modified.</span></span>|
|<span data-ttu-id="826b6-168">category</span><span class="sxs-lookup"><span data-stu-id="826b6-168">category</span></span>|<span data-ttu-id="826b6-169">String</span><span class="sxs-lookup"><span data-stu-id="826b6-169">String</span></span>|<span data-ttu-id="826b6-170">审核类别。</span><span class="sxs-lookup"><span data-stu-id="826b6-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="826b6-171">关系</span><span class="sxs-lookup"><span data-stu-id="826b6-171">Relationships</span></span>
<span data-ttu-id="826b6-172">无</span><span class="sxs-lookup"><span data-stu-id="826b6-172">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="826b6-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="826b6-173">JSON Representation</span></span>
<span data-ttu-id="826b6-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="826b6-174">Here is a JSON representation of the resource.</span></span>
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



