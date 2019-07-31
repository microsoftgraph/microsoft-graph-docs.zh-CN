---
title: auditEvent 资源类型
description: 包含审核事件的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85ce910b963b10d024943bd95a5d1930ef9eaf39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012084"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="fbfc3-103">auditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbfc3-103">auditEvent resource type</span></span>

> <span data-ttu-id="fbfc3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbfc3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbfc3-106">包含审核事件的属性的类。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-106">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="fbfc3-107">方法</span><span class="sxs-lookup"><span data-stu-id="fbfc3-107">Methods</span></span>
|<span data-ttu-id="fbfc3-108">方法</span><span class="sxs-lookup"><span data-stu-id="fbfc3-108">Method</span></span>|<span data-ttu-id="fbfc3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fbfc3-109">Return Type</span></span>|<span data-ttu-id="fbfc3-110">说明</span><span class="sxs-lookup"><span data-stu-id="fbfc3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fbfc3-111">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="fbfc3-111">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="fbfc3-112">[auditEvent](../resources/intune-auditing-auditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbfc3-112">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="fbfc3-113">列出 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-113">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="fbfc3-114">获取 auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-114">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="fbfc3-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-115">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="fbfc3-116">读取 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-116">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="fbfc3-117">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-117">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="fbfc3-118">auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-118">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="fbfc3-119">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-119">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="fbfc3-120">删除 auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-120">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="fbfc3-121">无</span><span class="sxs-lookup"><span data-stu-id="fbfc3-121">None</span></span>|<span data-ttu-id="fbfc3-122">删除 [auditEvent](../resources/intune-auditing-auditevent.md)。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-122">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="fbfc3-123">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-123">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="fbfc3-124">auditEvent</span><span class="sxs-lookup"><span data-stu-id="fbfc3-124">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="fbfc3-125">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-125">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="fbfc3-126">getAuditCategories 函数</span><span class="sxs-lookup"><span data-stu-id="fbfc3-126">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="fbfc3-127">String collection</span><span class="sxs-lookup"><span data-stu-id="fbfc3-127">String collection</span></span>|<span data-ttu-id="fbfc3-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fbfc3-128">Not yet documented</span></span>|
|[<span data-ttu-id="fbfc3-129">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="fbfc3-129">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="fbfc3-130">String collection</span><span class="sxs-lookup"><span data-stu-id="fbfc3-130">String collection</span></span>|<span data-ttu-id="fbfc3-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fbfc3-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fbfc3-132">属性</span><span class="sxs-lookup"><span data-stu-id="fbfc3-132">Properties</span></span>
|<span data-ttu-id="fbfc3-133">属性</span><span class="sxs-lookup"><span data-stu-id="fbfc3-133">Property</span></span>|<span data-ttu-id="fbfc3-134">类型</span><span class="sxs-lookup"><span data-stu-id="fbfc3-134">Type</span></span>|<span data-ttu-id="fbfc3-135">说明</span><span class="sxs-lookup"><span data-stu-id="fbfc3-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbfc3-136">id</span><span class="sxs-lookup"><span data-stu-id="fbfc3-136">id</span></span>|<span data-ttu-id="fbfc3-137">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-137">String</span></span>|<span data-ttu-id="fbfc3-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-138">Key of the entity.</span></span>|
|<span data-ttu-id="fbfc3-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fbfc3-139">displayName</span></span>|<span data-ttu-id="fbfc3-140">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-140">String</span></span>|<span data-ttu-id="fbfc3-141">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-141">Event display name.</span></span>|
|<span data-ttu-id="fbfc3-142">componentName</span><span class="sxs-lookup"><span data-stu-id="fbfc3-142">componentName</span></span>|<span data-ttu-id="fbfc3-143">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-143">String</span></span>|<span data-ttu-id="fbfc3-144">组件名称。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-144">Component name.</span></span>|
|<span data-ttu-id="fbfc3-145">actor</span><span class="sxs-lookup"><span data-stu-id="fbfc3-145">actor</span></span>|[<span data-ttu-id="fbfc3-146">auditActor</span><span class="sxs-lookup"><span data-stu-id="fbfc3-146">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="fbfc3-147">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-147">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="fbfc3-148">activity</span><span class="sxs-lookup"><span data-stu-id="fbfc3-148">activity</span></span>|<span data-ttu-id="fbfc3-149">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-149">String</span></span>|<span data-ttu-id="fbfc3-150">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-150">Friendly name of the activity.</span></span>|
|<span data-ttu-id="fbfc3-151">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="fbfc3-151">activityDateTime</span></span>|<span data-ttu-id="fbfc3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbfc3-152">DateTimeOffset</span></span>|<span data-ttu-id="fbfc3-153">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-153">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="fbfc3-154">activityType</span><span class="sxs-lookup"><span data-stu-id="fbfc3-154">activityType</span></span>|<span data-ttu-id="fbfc3-155">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-155">String</span></span>|<span data-ttu-id="fbfc3-156">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-156">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="fbfc3-157">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="fbfc3-157">activityOperationType</span></span>|<span data-ttu-id="fbfc3-158">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-158">String</span></span>|<span data-ttu-id="fbfc3-159">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-159">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="fbfc3-160">activityResult</span><span class="sxs-lookup"><span data-stu-id="fbfc3-160">activityResult</span></span>|<span data-ttu-id="fbfc3-161">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-161">String</span></span>|<span data-ttu-id="fbfc3-162">活动结果。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-162">The result of the activity.</span></span>|
|<span data-ttu-id="fbfc3-163">correlationId</span><span class="sxs-lookup"><span data-stu-id="fbfc3-163">correlationId</span></span>|<span data-ttu-id="fbfc3-164">Guid</span><span class="sxs-lookup"><span data-stu-id="fbfc3-164">Guid</span></span>|<span data-ttu-id="fbfc3-165">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-165">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="fbfc3-166">resources</span><span class="sxs-lookup"><span data-stu-id="fbfc3-166">resources</span></span>|<span data-ttu-id="fbfc3-167">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbfc3-167">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="fbfc3-168">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-168">Resources being modified.</span></span>|
|<span data-ttu-id="fbfc3-169">“类别”</span><span class="sxs-lookup"><span data-stu-id="fbfc3-169">category</span></span>|<span data-ttu-id="fbfc3-170">String</span><span class="sxs-lookup"><span data-stu-id="fbfc3-170">String</span></span>|<span data-ttu-id="fbfc3-171">审核类别。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-171">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbfc3-172">关系</span><span class="sxs-lookup"><span data-stu-id="fbfc3-172">Relationships</span></span>
<span data-ttu-id="fbfc3-173">无</span><span class="sxs-lookup"><span data-stu-id="fbfc3-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbfc3-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbfc3-174">JSON Representation</span></span>
<span data-ttu-id="fbfc3-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbfc3-175">Here is a JSON representation of the resource.</span></span>
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





