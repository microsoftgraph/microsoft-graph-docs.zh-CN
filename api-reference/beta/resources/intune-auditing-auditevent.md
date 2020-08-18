---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1945795798033e876aa4e26631c667e198d8d5e0
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792980"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="5a185-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a185-103">auditEvent resource type</span></span>

<span data-ttu-id="5a185-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a185-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a185-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a185-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a185-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a185-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a185-107">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="5a185-107">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="5a185-108">方法</span><span class="sxs-lookup"><span data-stu-id="5a185-108">Methods</span></span>
|<span data-ttu-id="5a185-109">方法</span><span class="sxs-lookup"><span data-stu-id="5a185-109">Method</span></span>|<span data-ttu-id="5a185-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a185-110">Return Type</span></span>|<span data-ttu-id="5a185-111">说明</span><span class="sxs-lookup"><span data-stu-id="5a185-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a185-112">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="5a185-112">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="5a185-113">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a185-113">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="5a185-114">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a185-114">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="5a185-115">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-115">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="5a185-116">auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-116">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="5a185-117">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a185-117">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="5a185-118">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-118">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="5a185-119">auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-119">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="5a185-120">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a185-120">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="5a185-121">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-121">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="5a185-122">无</span><span class="sxs-lookup"><span data-stu-id="5a185-122">None</span></span>|<span data-ttu-id="5a185-123">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="5a185-123">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="5a185-124">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-124">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="5a185-125">auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a185-125">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="5a185-126">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5a185-126">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="5a185-127">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="5a185-127">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="5a185-128">String collection</span><span class="sxs-lookup"><span data-stu-id="5a185-128">String collection</span></span>|<span data-ttu-id="5a185-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a185-129">Not yet documented</span></span>|
|[<span data-ttu-id="5a185-130">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="5a185-130">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="5a185-131">String collection</span><span class="sxs-lookup"><span data-stu-id="5a185-131">String collection</span></span>|<span data-ttu-id="5a185-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a185-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a185-133">属性</span><span class="sxs-lookup"><span data-stu-id="5a185-133">Properties</span></span>
|<span data-ttu-id="5a185-134">属性</span><span class="sxs-lookup"><span data-stu-id="5a185-134">Property</span></span>|<span data-ttu-id="5a185-135">类型</span><span class="sxs-lookup"><span data-stu-id="5a185-135">Type</span></span>|<span data-ttu-id="5a185-136">说明</span><span class="sxs-lookup"><span data-stu-id="5a185-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a185-137">id</span><span class="sxs-lookup"><span data-stu-id="5a185-137">id</span></span>|<span data-ttu-id="5a185-138">String</span><span class="sxs-lookup"><span data-stu-id="5a185-138">String</span></span>|<span data-ttu-id="5a185-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5a185-139">Key of the entity.</span></span>|
|<span data-ttu-id="5a185-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5a185-140">displayName</span></span>|<span data-ttu-id="5a185-141">String</span><span class="sxs-lookup"><span data-stu-id="5a185-141">String</span></span>|<span data-ttu-id="5a185-142">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="5a185-142">Event display name.</span></span>|
|<span data-ttu-id="5a185-143">componentName</span><span class="sxs-lookup"><span data-stu-id="5a185-143">componentName</span></span>|<span data-ttu-id="5a185-144">String</span><span class="sxs-lookup"><span data-stu-id="5a185-144">String</span></span>|<span data-ttu-id="5a185-145">组件名称。</span><span class="sxs-lookup"><span data-stu-id="5a185-145">Component name.</span></span>|
|<span data-ttu-id="5a185-146">actor</span><span class="sxs-lookup"><span data-stu-id="5a185-146">actor</span></span>|[<span data-ttu-id="5a185-147">auditActor</span><span class="sxs-lookup"><span data-stu-id="5a185-147">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="5a185-148">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="5a185-148">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="5a185-149">activity</span><span class="sxs-lookup"><span data-stu-id="5a185-149">activity</span></span>|<span data-ttu-id="5a185-150">String</span><span class="sxs-lookup"><span data-stu-id="5a185-150">String</span></span>|<span data-ttu-id="5a185-151">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5a185-151">Friendly name of the activity.</span></span>|
|<span data-ttu-id="5a185-152">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="5a185-152">activityDateTime</span></span>|<span data-ttu-id="5a185-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a185-153">DateTimeOffset</span></span>|<span data-ttu-id="5a185-154">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="5a185-154">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="5a185-155">activityType</span><span class="sxs-lookup"><span data-stu-id="5a185-155">activityType</span></span>|<span data-ttu-id="5a185-156">String</span><span class="sxs-lookup"><span data-stu-id="5a185-156">String</span></span>|<span data-ttu-id="5a185-157">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="5a185-157">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="5a185-158">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="5a185-158">activityOperationType</span></span>|<span data-ttu-id="5a185-159">String</span><span class="sxs-lookup"><span data-stu-id="5a185-159">String</span></span>|<span data-ttu-id="5a185-160">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="5a185-160">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="5a185-161">activityResult</span><span class="sxs-lookup"><span data-stu-id="5a185-161">activityResult</span></span>|<span data-ttu-id="5a185-162">String</span><span class="sxs-lookup"><span data-stu-id="5a185-162">String</span></span>|<span data-ttu-id="5a185-163">活动结果。</span><span class="sxs-lookup"><span data-stu-id="5a185-163">The result of the activity.</span></span>|
|<span data-ttu-id="5a185-164">correlationId</span><span class="sxs-lookup"><span data-stu-id="5a185-164">correlationId</span></span>|<span data-ttu-id="5a185-165">Guid</span><span class="sxs-lookup"><span data-stu-id="5a185-165">Guid</span></span>|<span data-ttu-id="5a185-166">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="5a185-166">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="5a185-167">resources</span><span class="sxs-lookup"><span data-stu-id="5a185-167">resources</span></span>|<span data-ttu-id="5a185-168">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a185-168">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="5a185-169">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="5a185-169">Resources being modified.</span></span>|
|<span data-ttu-id="5a185-170">“类别”</span><span class="sxs-lookup"><span data-stu-id="5a185-170">category</span></span>|<span data-ttu-id="5a185-171">String</span><span class="sxs-lookup"><span data-stu-id="5a185-171">String</span></span>|<span data-ttu-id="5a185-172">审核类别。</span><span class="sxs-lookup"><span data-stu-id="5a185-172">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a185-173">关系</span><span class="sxs-lookup"><span data-stu-id="5a185-173">Relationships</span></span>
<span data-ttu-id="5a185-174">无</span><span class="sxs-lookup"><span data-stu-id="5a185-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a185-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a185-175">JSON Representation</span></span>
<span data-ttu-id="5a185-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a185-176">Here is a JSON representation of the resource.</span></span>
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
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
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



