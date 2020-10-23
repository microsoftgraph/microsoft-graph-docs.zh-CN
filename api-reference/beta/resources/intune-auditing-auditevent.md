---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0695d951aaa8825153e7a20dac60f30351907e2c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706070"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="6de9c-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="6de9c-103">auditEvent resource type</span></span>

<span data-ttu-id="6de9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6de9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6de9c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6de9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6de9c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6de9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6de9c-107">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="6de9c-107">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="6de9c-108">Methods</span><span class="sxs-lookup"><span data-stu-id="6de9c-108">Methods</span></span>
|<span data-ttu-id="6de9c-109">方法</span><span class="sxs-lookup"><span data-stu-id="6de9c-109">Method</span></span>|<span data-ttu-id="6de9c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6de9c-110">Return Type</span></span>|<span data-ttu-id="6de9c-111">说明</span><span class="sxs-lookup"><span data-stu-id="6de9c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6de9c-112">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="6de9c-112">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="6de9c-113">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6de9c-113">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="6de9c-114">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6de9c-114">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="6de9c-115">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-115">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="6de9c-116">auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-116">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="6de9c-117">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6de9c-117">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="6de9c-118">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-118">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="6de9c-119">auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-119">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="6de9c-120">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6de9c-120">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="6de9c-121">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-121">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="6de9c-122">无</span><span class="sxs-lookup"><span data-stu-id="6de9c-122">None</span></span>|<span data-ttu-id="6de9c-123">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="6de9c-123">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="6de9c-124">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-124">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="6de9c-125">auditEvent</span><span class="sxs-lookup"><span data-stu-id="6de9c-125">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="6de9c-126">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6de9c-126">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="6de9c-127">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="6de9c-127">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="6de9c-128">String collection</span><span class="sxs-lookup"><span data-stu-id="6de9c-128">String collection</span></span>|<span data-ttu-id="6de9c-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6de9c-129">Not yet documented</span></span>|
|[<span data-ttu-id="6de9c-130">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="6de9c-130">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="6de9c-131">String collection</span><span class="sxs-lookup"><span data-stu-id="6de9c-131">String collection</span></span>|<span data-ttu-id="6de9c-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6de9c-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6de9c-133">属性</span><span class="sxs-lookup"><span data-stu-id="6de9c-133">Properties</span></span>
|<span data-ttu-id="6de9c-134">属性</span><span class="sxs-lookup"><span data-stu-id="6de9c-134">Property</span></span>|<span data-ttu-id="6de9c-135">类型</span><span class="sxs-lookup"><span data-stu-id="6de9c-135">Type</span></span>|<span data-ttu-id="6de9c-136">说明</span><span class="sxs-lookup"><span data-stu-id="6de9c-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de9c-137">id</span><span class="sxs-lookup"><span data-stu-id="6de9c-137">id</span></span>|<span data-ttu-id="6de9c-138">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-138">String</span></span>|<span data-ttu-id="6de9c-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6de9c-139">Key of the entity.</span></span>|
|<span data-ttu-id="6de9c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="6de9c-140">displayName</span></span>|<span data-ttu-id="6de9c-141">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-141">String</span></span>|<span data-ttu-id="6de9c-142">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="6de9c-142">Event display name.</span></span>|
|<span data-ttu-id="6de9c-143">componentName</span><span class="sxs-lookup"><span data-stu-id="6de9c-143">componentName</span></span>|<span data-ttu-id="6de9c-144">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-144">String</span></span>|<span data-ttu-id="6de9c-145">组件名称。</span><span class="sxs-lookup"><span data-stu-id="6de9c-145">Component name.</span></span>|
|<span data-ttu-id="6de9c-146">actor</span><span class="sxs-lookup"><span data-stu-id="6de9c-146">actor</span></span>|[<span data-ttu-id="6de9c-147">auditActor</span><span class="sxs-lookup"><span data-stu-id="6de9c-147">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="6de9c-148">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="6de9c-148">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="6de9c-149">activity</span><span class="sxs-lookup"><span data-stu-id="6de9c-149">activity</span></span>|<span data-ttu-id="6de9c-150">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-150">String</span></span>|<span data-ttu-id="6de9c-151">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="6de9c-151">Friendly name of the activity.</span></span>|
|<span data-ttu-id="6de9c-152">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6de9c-152">activityDateTime</span></span>|<span data-ttu-id="6de9c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6de9c-153">DateTimeOffset</span></span>|<span data-ttu-id="6de9c-154">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="6de9c-154">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="6de9c-155">activityType</span><span class="sxs-lookup"><span data-stu-id="6de9c-155">activityType</span></span>|<span data-ttu-id="6de9c-156">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-156">String</span></span>|<span data-ttu-id="6de9c-157">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="6de9c-157">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="6de9c-158">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="6de9c-158">activityOperationType</span></span>|<span data-ttu-id="6de9c-159">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-159">String</span></span>|<span data-ttu-id="6de9c-160">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="6de9c-160">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="6de9c-161">activityResult</span><span class="sxs-lookup"><span data-stu-id="6de9c-161">activityResult</span></span>|<span data-ttu-id="6de9c-162">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-162">String</span></span>|<span data-ttu-id="6de9c-163">活动结果。</span><span class="sxs-lookup"><span data-stu-id="6de9c-163">The result of the activity.</span></span>|
|<span data-ttu-id="6de9c-164">correlationId</span><span class="sxs-lookup"><span data-stu-id="6de9c-164">correlationId</span></span>|<span data-ttu-id="6de9c-165">Guid</span><span class="sxs-lookup"><span data-stu-id="6de9c-165">Guid</span></span>|<span data-ttu-id="6de9c-166">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="6de9c-166">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="6de9c-167">resources</span><span class="sxs-lookup"><span data-stu-id="6de9c-167">resources</span></span>|<span data-ttu-id="6de9c-168">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6de9c-168">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="6de9c-169">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="6de9c-169">Resources being modified.</span></span>|
|<span data-ttu-id="6de9c-170">“类别”</span><span class="sxs-lookup"><span data-stu-id="6de9c-170">category</span></span>|<span data-ttu-id="6de9c-171">String</span><span class="sxs-lookup"><span data-stu-id="6de9c-171">String</span></span>|<span data-ttu-id="6de9c-172">审核类别。</span><span class="sxs-lookup"><span data-stu-id="6de9c-172">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6de9c-173">关系</span><span class="sxs-lookup"><span data-stu-id="6de9c-173">Relationships</span></span>
<span data-ttu-id="6de9c-174">无</span><span class="sxs-lookup"><span data-stu-id="6de9c-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6de9c-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6de9c-175">JSON Representation</span></span>
<span data-ttu-id="6de9c-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6de9c-176">Here is a JSON representation of the resource.</span></span>
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





