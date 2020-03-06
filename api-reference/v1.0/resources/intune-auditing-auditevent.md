---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ec433c2ad38e967d7772031ab654e35fafa7c8b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531036"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="a6ab6-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6ab6-103">auditEvent resource type</span></span>

<span data-ttu-id="a6ab6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6ab6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6ab6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ab6-106">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-106">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="a6ab6-107">Methods</span><span class="sxs-lookup"><span data-stu-id="a6ab6-107">Methods</span></span>
|<span data-ttu-id="a6ab6-108">方法</span><span class="sxs-lookup"><span data-stu-id="a6ab6-108">Method</span></span>|<span data-ttu-id="a6ab6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6ab6-109">Return Type</span></span>|<span data-ttu-id="a6ab6-110">说明</span><span class="sxs-lookup"><span data-stu-id="a6ab6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6ab6-111">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="a6ab6-111">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="a6ab6-112">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6ab6-112">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="a6ab6-113">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-113">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="a6ab6-114">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-114">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="a6ab6-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-115">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="a6ab6-116">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-116">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="a6ab6-117">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-117">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="a6ab6-118">auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-118">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="a6ab6-119">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-119">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="a6ab6-120">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-120">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="a6ab6-121">无</span><span class="sxs-lookup"><span data-stu-id="a6ab6-121">None</span></span>|<span data-ttu-id="a6ab6-122">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-122">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="a6ab6-123">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-123">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="a6ab6-124">auditEvent</span><span class="sxs-lookup"><span data-stu-id="a6ab6-124">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="a6ab6-125">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-125">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="a6ab6-126">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="a6ab6-126">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="a6ab6-127">String collection</span><span class="sxs-lookup"><span data-stu-id="a6ab6-127">String collection</span></span>|<span data-ttu-id="a6ab6-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6ab6-128">Not yet documented</span></span>|
|[<span data-ttu-id="a6ab6-129">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="a6ab6-129">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="a6ab6-130">String collection</span><span class="sxs-lookup"><span data-stu-id="a6ab6-130">String collection</span></span>|<span data-ttu-id="a6ab6-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6ab6-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a6ab6-132">属性</span><span class="sxs-lookup"><span data-stu-id="a6ab6-132">Properties</span></span>
|<span data-ttu-id="a6ab6-133">属性</span><span class="sxs-lookup"><span data-stu-id="a6ab6-133">Property</span></span>|<span data-ttu-id="a6ab6-134">类型</span><span class="sxs-lookup"><span data-stu-id="a6ab6-134">Type</span></span>|<span data-ttu-id="a6ab6-135">说明</span><span class="sxs-lookup"><span data-stu-id="a6ab6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6ab6-136">id</span><span class="sxs-lookup"><span data-stu-id="a6ab6-136">id</span></span>|<span data-ttu-id="a6ab6-137">String</span><span class="sxs-lookup"><span data-stu-id="a6ab6-137">String</span></span>|<span data-ttu-id="a6ab6-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-138">Key of the entity.</span></span>|
|<span data-ttu-id="a6ab6-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a6ab6-139">displayName</span></span>|<span data-ttu-id="a6ab6-140">字符串</span><span class="sxs-lookup"><span data-stu-id="a6ab6-140">String</span></span>|<span data-ttu-id="a6ab6-141">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-141">Event display name.</span></span>|
|<span data-ttu-id="a6ab6-142">componentName</span><span class="sxs-lookup"><span data-stu-id="a6ab6-142">componentName</span></span>|<span data-ttu-id="a6ab6-143">字符串</span><span class="sxs-lookup"><span data-stu-id="a6ab6-143">String</span></span>|<span data-ttu-id="a6ab6-144">组件名称。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-144">Component name.</span></span>|
|<span data-ttu-id="a6ab6-145">actor</span><span class="sxs-lookup"><span data-stu-id="a6ab6-145">actor</span></span>|[<span data-ttu-id="a6ab6-146">auditActor</span><span class="sxs-lookup"><span data-stu-id="a6ab6-146">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="a6ab6-147">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-147">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="a6ab6-148">activity</span><span class="sxs-lookup"><span data-stu-id="a6ab6-148">activity</span></span>|<span data-ttu-id="a6ab6-149">字符串</span><span class="sxs-lookup"><span data-stu-id="a6ab6-149">String</span></span>|<span data-ttu-id="a6ab6-150">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-150">Friendly name of the activity.</span></span>|
|<span data-ttu-id="a6ab6-151">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="a6ab6-151">activityDateTime</span></span>|<span data-ttu-id="a6ab6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6ab6-152">DateTimeOffset</span></span>|<span data-ttu-id="a6ab6-153">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-153">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="a6ab6-154">activityType</span><span class="sxs-lookup"><span data-stu-id="a6ab6-154">activityType</span></span>|<span data-ttu-id="a6ab6-155">字符串</span><span class="sxs-lookup"><span data-stu-id="a6ab6-155">String</span></span>|<span data-ttu-id="a6ab6-156">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-156">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="a6ab6-157">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="a6ab6-157">activityOperationType</span></span>|<span data-ttu-id="a6ab6-158">字符串</span><span class="sxs-lookup"><span data-stu-id="a6ab6-158">String</span></span>|<span data-ttu-id="a6ab6-159">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-159">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="a6ab6-160">activityResult</span><span class="sxs-lookup"><span data-stu-id="a6ab6-160">activityResult</span></span>|<span data-ttu-id="a6ab6-161">String</span><span class="sxs-lookup"><span data-stu-id="a6ab6-161">String</span></span>|<span data-ttu-id="a6ab6-162">活动结果。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-162">The result of the activity.</span></span>|
|<span data-ttu-id="a6ab6-163">correlationId</span><span class="sxs-lookup"><span data-stu-id="a6ab6-163">correlationId</span></span>|<span data-ttu-id="a6ab6-164">Guid</span><span class="sxs-lookup"><span data-stu-id="a6ab6-164">Guid</span></span>|<span data-ttu-id="a6ab6-165">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-165">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="a6ab6-166">resources</span><span class="sxs-lookup"><span data-stu-id="a6ab6-166">resources</span></span>|<span data-ttu-id="a6ab6-167">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6ab6-167">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="a6ab6-168">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-168">Resources being modified.</span></span>|
|<span data-ttu-id="a6ab6-169">“类别”</span><span class="sxs-lookup"><span data-stu-id="a6ab6-169">category</span></span>|<span data-ttu-id="a6ab6-170">字符串</span><span class="sxs-lookup"><span data-stu-id="a6ab6-170">String</span></span>|<span data-ttu-id="a6ab6-171">审核类别。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-171">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6ab6-172">关系</span><span class="sxs-lookup"><span data-stu-id="a6ab6-172">Relationships</span></span>
<span data-ttu-id="a6ab6-173">无</span><span class="sxs-lookup"><span data-stu-id="a6ab6-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6ab6-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6ab6-174">JSON Representation</span></span>
<span data-ttu-id="a6ab6-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6ab6-175">Here is a JSON representation of the resource.</span></span>
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




