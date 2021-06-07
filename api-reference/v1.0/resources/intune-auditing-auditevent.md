---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f5501db74d088283127fde36ea65275257da689
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756433"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="ae4b7-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae4b7-103">auditEvent resource type</span></span>

<span data-ttu-id="ae4b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae4b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae4b7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae4b7-106">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-106">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="ae4b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="ae4b7-107">Methods</span></span>
|<span data-ttu-id="ae4b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="ae4b7-108">Method</span></span>|<span data-ttu-id="ae4b7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ae4b7-109">Return Type</span></span>|<span data-ttu-id="ae4b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="ae4b7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae4b7-111">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="ae4b7-111">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="ae4b7-112">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ae4b7-112">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="ae4b7-113">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-113">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="ae4b7-114">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-114">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="ae4b7-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-115">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="ae4b7-116">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-116">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="ae4b7-117">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-117">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="ae4b7-118">auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-118">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="ae4b7-119">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-119">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="ae4b7-120">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-120">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="ae4b7-121">无</span><span class="sxs-lookup"><span data-stu-id="ae4b7-121">None</span></span>|<span data-ttu-id="ae4b7-122">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-122">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="ae4b7-123">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-123">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="ae4b7-124">auditEvent</span><span class="sxs-lookup"><span data-stu-id="ae4b7-124">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="ae4b7-125">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-125">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="ae4b7-126">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="ae4b7-126">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="ae4b7-127">String collection</span><span class="sxs-lookup"><span data-stu-id="ae4b7-127">String collection</span></span>|<span data-ttu-id="ae4b7-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ae4b7-128">Not yet documented</span></span>|
|[<span data-ttu-id="ae4b7-129">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="ae4b7-129">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="ae4b7-130">String collection</span><span class="sxs-lookup"><span data-stu-id="ae4b7-130">String collection</span></span>|<span data-ttu-id="ae4b7-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ae4b7-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ae4b7-132">属性</span><span class="sxs-lookup"><span data-stu-id="ae4b7-132">Properties</span></span>
|<span data-ttu-id="ae4b7-133">属性</span><span class="sxs-lookup"><span data-stu-id="ae4b7-133">Property</span></span>|<span data-ttu-id="ae4b7-134">类型</span><span class="sxs-lookup"><span data-stu-id="ae4b7-134">Type</span></span>|<span data-ttu-id="ae4b7-135">说明</span><span class="sxs-lookup"><span data-stu-id="ae4b7-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae4b7-136">id</span><span class="sxs-lookup"><span data-stu-id="ae4b7-136">id</span></span>|<span data-ttu-id="ae4b7-137">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-137">String</span></span>|<span data-ttu-id="ae4b7-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-138">Key of the entity.</span></span>|
|<span data-ttu-id="ae4b7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ae4b7-139">displayName</span></span>|<span data-ttu-id="ae4b7-140">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-140">String</span></span>|<span data-ttu-id="ae4b7-141">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-141">Event display name.</span></span>|
|<span data-ttu-id="ae4b7-142">componentName</span><span class="sxs-lookup"><span data-stu-id="ae4b7-142">componentName</span></span>|<span data-ttu-id="ae4b7-143">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-143">String</span></span>|<span data-ttu-id="ae4b7-144">组件名称。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-144">Component name.</span></span>|
|<span data-ttu-id="ae4b7-145">actor</span><span class="sxs-lookup"><span data-stu-id="ae4b7-145">actor</span></span>|[<span data-ttu-id="ae4b7-146">auditActor</span><span class="sxs-lookup"><span data-stu-id="ae4b7-146">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="ae4b7-147">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-147">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="ae4b7-148">activity</span><span class="sxs-lookup"><span data-stu-id="ae4b7-148">activity</span></span>|<span data-ttu-id="ae4b7-149">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-149">String</span></span>|<span data-ttu-id="ae4b7-150">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-150">Friendly name of the activity.</span></span>|
|<span data-ttu-id="ae4b7-151">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="ae4b7-151">activityDateTime</span></span>|<span data-ttu-id="ae4b7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae4b7-152">DateTimeOffset</span></span>|<span data-ttu-id="ae4b7-153">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-153">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="ae4b7-154">activityType</span><span class="sxs-lookup"><span data-stu-id="ae4b7-154">activityType</span></span>|<span data-ttu-id="ae4b7-155">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-155">String</span></span>|<span data-ttu-id="ae4b7-156">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-156">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="ae4b7-157">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="ae4b7-157">activityOperationType</span></span>|<span data-ttu-id="ae4b7-158">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-158">String</span></span>|<span data-ttu-id="ae4b7-159">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-159">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="ae4b7-160">activityResult</span><span class="sxs-lookup"><span data-stu-id="ae4b7-160">activityResult</span></span>|<span data-ttu-id="ae4b7-161">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-161">String</span></span>|<span data-ttu-id="ae4b7-162">活动结果。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-162">The result of the activity.</span></span>|
|<span data-ttu-id="ae4b7-163">correlationId</span><span class="sxs-lookup"><span data-stu-id="ae4b7-163">correlationId</span></span>|<span data-ttu-id="ae4b7-164">Guid</span><span class="sxs-lookup"><span data-stu-id="ae4b7-164">Guid</span></span>|<span data-ttu-id="ae4b7-165">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-165">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="ae4b7-166">resources</span><span class="sxs-lookup"><span data-stu-id="ae4b7-166">resources</span></span>|<span data-ttu-id="ae4b7-167">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ae4b7-167">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="ae4b7-168">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-168">Resources being modified.</span></span>|
|<span data-ttu-id="ae4b7-169">“类别”</span><span class="sxs-lookup"><span data-stu-id="ae4b7-169">category</span></span>|<span data-ttu-id="ae4b7-170">String</span><span class="sxs-lookup"><span data-stu-id="ae4b7-170">String</span></span>|<span data-ttu-id="ae4b7-171">审核类别。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-171">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae4b7-172">关系</span><span class="sxs-lookup"><span data-stu-id="ae4b7-172">Relationships</span></span>
<span data-ttu-id="ae4b7-173">无</span><span class="sxs-lookup"><span data-stu-id="ae4b7-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae4b7-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae4b7-174">JSON Representation</span></span>
<span data-ttu-id="ae4b7-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae4b7-175">Here is a JSON representation of the resource.</span></span>
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




