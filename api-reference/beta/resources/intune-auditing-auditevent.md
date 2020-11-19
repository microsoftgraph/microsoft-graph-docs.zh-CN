---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 432d61b4c8d23c013f4920094f9cba5fab6a078d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295542"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="82a25-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="82a25-103">auditEvent resource type</span></span>

<span data-ttu-id="82a25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82a25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82a25-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82a25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82a25-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82a25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82a25-107">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="82a25-107">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="82a25-108">Methods</span><span class="sxs-lookup"><span data-stu-id="82a25-108">Methods</span></span>
|<span data-ttu-id="82a25-109">方法</span><span class="sxs-lookup"><span data-stu-id="82a25-109">Method</span></span>|<span data-ttu-id="82a25-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="82a25-110">Return Type</span></span>|<span data-ttu-id="82a25-111">Description</span><span class="sxs-lookup"><span data-stu-id="82a25-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="82a25-112">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="82a25-112">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="82a25-113">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82a25-113">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="82a25-114">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82a25-114">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="82a25-115">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-115">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="82a25-116">auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-116">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="82a25-117">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82a25-117">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="82a25-118">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-118">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="82a25-119">auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-119">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="82a25-120">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82a25-120">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="82a25-121">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-121">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="82a25-122">无</span><span class="sxs-lookup"><span data-stu-id="82a25-122">None</span></span>|<span data-ttu-id="82a25-123">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="82a25-123">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="82a25-124">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-124">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="82a25-125">auditEvent</span><span class="sxs-lookup"><span data-stu-id="82a25-125">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="82a25-126">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82a25-126">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="82a25-127">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="82a25-127">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="82a25-128">String collection</span><span class="sxs-lookup"><span data-stu-id="82a25-128">String collection</span></span>|<span data-ttu-id="82a25-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="82a25-129">Not yet documented</span></span>|
|[<span data-ttu-id="82a25-130">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="82a25-130">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="82a25-131">String collection</span><span class="sxs-lookup"><span data-stu-id="82a25-131">String collection</span></span>|<span data-ttu-id="82a25-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="82a25-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="82a25-133">属性</span><span class="sxs-lookup"><span data-stu-id="82a25-133">Properties</span></span>
|<span data-ttu-id="82a25-134">属性</span><span class="sxs-lookup"><span data-stu-id="82a25-134">Property</span></span>|<span data-ttu-id="82a25-135">类型</span><span class="sxs-lookup"><span data-stu-id="82a25-135">Type</span></span>|<span data-ttu-id="82a25-136">说明</span><span class="sxs-lookup"><span data-stu-id="82a25-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82a25-137">id</span><span class="sxs-lookup"><span data-stu-id="82a25-137">id</span></span>|<span data-ttu-id="82a25-138">字符串</span><span class="sxs-lookup"><span data-stu-id="82a25-138">String</span></span>|<span data-ttu-id="82a25-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="82a25-139">Key of the entity.</span></span>|
|<span data-ttu-id="82a25-140">displayName</span><span class="sxs-lookup"><span data-stu-id="82a25-140">displayName</span></span>|<span data-ttu-id="82a25-141">字符串</span><span class="sxs-lookup"><span data-stu-id="82a25-141">String</span></span>|<span data-ttu-id="82a25-142">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="82a25-142">Event display name.</span></span>|
|<span data-ttu-id="82a25-143">componentName</span><span class="sxs-lookup"><span data-stu-id="82a25-143">componentName</span></span>|<span data-ttu-id="82a25-144">String</span><span class="sxs-lookup"><span data-stu-id="82a25-144">String</span></span>|<span data-ttu-id="82a25-145">组件名称。</span><span class="sxs-lookup"><span data-stu-id="82a25-145">Component name.</span></span>|
|<span data-ttu-id="82a25-146">actor</span><span class="sxs-lookup"><span data-stu-id="82a25-146">actor</span></span>|[<span data-ttu-id="82a25-147">auditActor</span><span class="sxs-lookup"><span data-stu-id="82a25-147">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="82a25-148">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="82a25-148">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="82a25-149">activity</span><span class="sxs-lookup"><span data-stu-id="82a25-149">activity</span></span>|<span data-ttu-id="82a25-150">String</span><span class="sxs-lookup"><span data-stu-id="82a25-150">String</span></span>|<span data-ttu-id="82a25-151">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="82a25-151">Friendly name of the activity.</span></span>|
|<span data-ttu-id="82a25-152">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="82a25-152">activityDateTime</span></span>|<span data-ttu-id="82a25-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82a25-153">DateTimeOffset</span></span>|<span data-ttu-id="82a25-154">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="82a25-154">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="82a25-155">activityType</span><span class="sxs-lookup"><span data-stu-id="82a25-155">activityType</span></span>|<span data-ttu-id="82a25-156">String</span><span class="sxs-lookup"><span data-stu-id="82a25-156">String</span></span>|<span data-ttu-id="82a25-157">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="82a25-157">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="82a25-158">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="82a25-158">activityOperationType</span></span>|<span data-ttu-id="82a25-159">String</span><span class="sxs-lookup"><span data-stu-id="82a25-159">String</span></span>|<span data-ttu-id="82a25-160">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="82a25-160">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="82a25-161">activityResult</span><span class="sxs-lookup"><span data-stu-id="82a25-161">activityResult</span></span>|<span data-ttu-id="82a25-162">String</span><span class="sxs-lookup"><span data-stu-id="82a25-162">String</span></span>|<span data-ttu-id="82a25-163">活动结果。</span><span class="sxs-lookup"><span data-stu-id="82a25-163">The result of the activity.</span></span>|
|<span data-ttu-id="82a25-164">correlationId</span><span class="sxs-lookup"><span data-stu-id="82a25-164">correlationId</span></span>|<span data-ttu-id="82a25-165">Guid</span><span class="sxs-lookup"><span data-stu-id="82a25-165">Guid</span></span>|<span data-ttu-id="82a25-166">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="82a25-166">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="82a25-167">resources</span><span class="sxs-lookup"><span data-stu-id="82a25-167">resources</span></span>|<span data-ttu-id="82a25-168">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82a25-168">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="82a25-169">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="82a25-169">Resources being modified.</span></span>|
|<span data-ttu-id="82a25-170">“类别”</span><span class="sxs-lookup"><span data-stu-id="82a25-170">category</span></span>|<span data-ttu-id="82a25-171">字符串</span><span class="sxs-lookup"><span data-stu-id="82a25-171">String</span></span>|<span data-ttu-id="82a25-172">审核类别。</span><span class="sxs-lookup"><span data-stu-id="82a25-172">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82a25-173">关系</span><span class="sxs-lookup"><span data-stu-id="82a25-173">Relationships</span></span>
<span data-ttu-id="82a25-174">无</span><span class="sxs-lookup"><span data-stu-id="82a25-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82a25-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82a25-175">JSON Representation</span></span>
<span data-ttu-id="82a25-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82a25-176">Here is a JSON representation of the resource.</span></span>
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




