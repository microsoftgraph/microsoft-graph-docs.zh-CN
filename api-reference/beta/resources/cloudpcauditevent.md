---
title: cloudPcAuditEvent 资源类型
description: 表示审核事件实体。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a863ea4128b7383c70bd14f025fcc5ce116dda25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211223"
---
# <a name="cloudpcauditevent-resource-type"></a><span data-ttu-id="805e8-103">cloudPcAuditEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="805e8-103">cloudPcAuditEvent resource type</span></span>

<span data-ttu-id="805e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="805e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="805e8-105">表示审核事件实体。</span><span class="sxs-lookup"><span data-stu-id="805e8-105">Represents the audit event entity.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="805e8-106">方法</span><span class="sxs-lookup"><span data-stu-id="805e8-106">Methods</span></span>

|<span data-ttu-id="805e8-107">方法</span><span class="sxs-lookup"><span data-stu-id="805e8-107">Method</span></span>|<span data-ttu-id="805e8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="805e8-108">Return type</span></span>|<span data-ttu-id="805e8-109">说明</span><span class="sxs-lookup"><span data-stu-id="805e8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="805e8-110">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="805e8-110">List auditEvents</span></span>](../api/virtualendpoint-list-auditevents.md)|<span data-ttu-id="805e8-111">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="805e8-111">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) collection</span></span>|<span data-ttu-id="805e8-112">列出租户 [中所有 cloudPcAuditEvent](../resources/cloudpcauditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="805e8-112">List all the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects in a tenant.</span></span>|
|[<span data-ttu-id="805e8-113">获取 cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="805e8-113">Get cloudPcAuditEvent</span></span>](../api/cloudpcauditevent-get.md)|[<span data-ttu-id="805e8-114">cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="805e8-114">cloudPcAuditEvent</span></span>](../resources/cloudpcauditevent.md)|<span data-ttu-id="805e8-115">读取 [cloudPcAuditEvent 对象的属性和](../resources/cloudpcauditevent.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="805e8-115">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>|
|[<span data-ttu-id="805e8-116">getAuditActivityTypes 函数</span><span class="sxs-lookup"><span data-stu-id="805e8-116">getAuditActivityTypes function</span></span>](../api/cloudpcauditevent-getauditactivitytypes.md)|<span data-ttu-id="805e8-117">String collection</span><span class="sxs-lookup"><span data-stu-id="805e8-117">String collection</span></span>|<span data-ttu-id="805e8-118">获取审核活动类型。</span><span class="sxs-lookup"><span data-stu-id="805e8-118">Get audit activity types.</span></span>|

## <a name="properties"></a><span data-ttu-id="805e8-119">属性</span><span class="sxs-lookup"><span data-stu-id="805e8-119">Properties</span></span>

|<span data-ttu-id="805e8-120">属性</span><span class="sxs-lookup"><span data-stu-id="805e8-120">Property</span></span>|<span data-ttu-id="805e8-121">类型</span><span class="sxs-lookup"><span data-stu-id="805e8-121">Type</span></span>|<span data-ttu-id="805e8-122">说明</span><span class="sxs-lookup"><span data-stu-id="805e8-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="805e8-123">id</span><span class="sxs-lookup"><span data-stu-id="805e8-123">id</span></span>|<span data-ttu-id="805e8-124">String</span><span class="sxs-lookup"><span data-stu-id="805e8-124">String</span></span>|<span data-ttu-id="805e8-125">审核实体的键。</span><span class="sxs-lookup"><span data-stu-id="805e8-125">Key of the audit entity.</span></span> <span data-ttu-id="805e8-126">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-126">Read-only.</span></span>|
|<span data-ttu-id="805e8-127">displayName</span><span class="sxs-lookup"><span data-stu-id="805e8-127">displayName</span></span>|<span data-ttu-id="805e8-128">String</span><span class="sxs-lookup"><span data-stu-id="805e8-128">String</span></span>|<span data-ttu-id="805e8-129">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="805e8-129">Event display name.</span></span> <span data-ttu-id="805e8-130">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-130">Read-only.</span></span>|
|<span data-ttu-id="805e8-131">componentName</span><span class="sxs-lookup"><span data-stu-id="805e8-131">componentName</span></span>|<span data-ttu-id="805e8-132">String</span><span class="sxs-lookup"><span data-stu-id="805e8-132">String</span></span>|<span data-ttu-id="805e8-133">组件名称。</span><span class="sxs-lookup"><span data-stu-id="805e8-133">Component name.</span></span> <span data-ttu-id="805e8-134">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-134">Read-only.</span></span>|
|<span data-ttu-id="805e8-135">actor</span><span class="sxs-lookup"><span data-stu-id="805e8-135">actor</span></span>|[<span data-ttu-id="805e8-136">cloudPcAuditActor</span><span class="sxs-lookup"><span data-stu-id="805e8-136">cloudPcAuditActor</span></span>](../resources/cloudpcauditactor.md)|<span data-ttu-id="805e8-137">与审核事件关联的 Azure AD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="805e8-137">Azure AD user and application associated with the audit event.</span></span> <span data-ttu-id="805e8-138">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-138">Read-only.</span></span>|
|<span data-ttu-id="805e8-139">activity</span><span class="sxs-lookup"><span data-stu-id="805e8-139">activity</span></span>|<span data-ttu-id="805e8-140">String</span><span class="sxs-lookup"><span data-stu-id="805e8-140">String</span></span>|<span data-ttu-id="805e8-141">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="805e8-141">Friendly name of the activity.</span></span><span data-ttu-id="805e8-142">可选。</span><span class="sxs-lookup"><span data-stu-id="805e8-142"> Optional.</span></span>|
|<span data-ttu-id="805e8-143">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="805e8-143">activityDateTime</span></span>|<span data-ttu-id="805e8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="805e8-144">DateTimeOffset</span></span>|<span data-ttu-id="805e8-145">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="805e8-145">The date time in UTC when the activity was performed.</span></span><span data-ttu-id="805e8-146">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-146"> Read-only.</span></span>|
|<span data-ttu-id="805e8-147">activityType</span><span class="sxs-lookup"><span data-stu-id="805e8-147">activityType</span></span>|<span data-ttu-id="805e8-148">String</span><span class="sxs-lookup"><span data-stu-id="805e8-148">String</span></span>|<span data-ttu-id="805e8-149">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="805e8-149">The type of activity that was performed.</span></span><span data-ttu-id="805e8-150">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-150"> Read-only.</span></span>|
|<span data-ttu-id="805e8-151">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="805e8-151">activityOperationType</span></span>|[<span data-ttu-id="805e8-152">cloudPcAuditActivityOperationType</span><span class="sxs-lookup"><span data-stu-id="805e8-152">cloudPcAuditActivityOperationType</span></span>](#cloudpcauditactivityoperationtype-values)|<span data-ttu-id="805e8-153">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="805e8-153">The HTTP operation type of the activity.</span></span> <span data-ttu-id="805e8-154">可能的值包括  `create` 、 `delete` 和 `patch` `other` 。</span><span class="sxs-lookup"><span data-stu-id="805e8-154">Possible values include `create`, `delete`, `patch` and `other`.</span></span> <span data-ttu-id="805e8-155">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-155">Read-only.</span></span>|
|<span data-ttu-id="805e8-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="805e8-156">activityResult</span></span>|[<span data-ttu-id="805e8-157">cloudPcAuditActivityResult</span><span class="sxs-lookup"><span data-stu-id="805e8-157">cloudPcAuditActivityResult</span></span>](#cloudpcauditactivityresult-values)|<span data-ttu-id="805e8-158">活动结果。</span><span class="sxs-lookup"><span data-stu-id="805e8-158">The result of the activity.</span></span><span data-ttu-id="805e8-159">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-159"> Read-only.</span></span>|
|<span data-ttu-id="805e8-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="805e8-160">correlationId</span></span>|<span data-ttu-id="805e8-161">String</span><span class="sxs-lookup"><span data-stu-id="805e8-161">String</span></span>|<span data-ttu-id="805e8-162">客户端请求标识符，用于关联系统内的活动。</span><span class="sxs-lookup"><span data-stu-id="805e8-162">The client request identifier, used to correlate activity within the system.</span></span><span data-ttu-id="805e8-163">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-163"> Read-only.</span></span>|
|<span data-ttu-id="805e8-164">resources</span><span class="sxs-lookup"><span data-stu-id="805e8-164">resources</span></span>|<span data-ttu-id="805e8-165">[cloudPcAuditResource](../resources/cloudpcauditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="805e8-165">[cloudPcAuditResource](../resources/cloudpcauditresource.md) collection</span></span>|<span data-ttu-id="805e8-166">cloudPcAuditResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="805e8-166">List of cloudPcAuditResource objects.</span></span><span data-ttu-id="805e8-167">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-167"> Read-only.</span></span>|
|<span data-ttu-id="805e8-168">“类别”</span><span class="sxs-lookup"><span data-stu-id="805e8-168">category</span></span>|[<span data-ttu-id="805e8-169">cloudPcAuditCategory</span><span class="sxs-lookup"><span data-stu-id="805e8-169">cloudPcAuditCategory</span></span>](#cloudpcauditcategory-values)|<span data-ttu-id="805e8-170">审核类别。</span><span class="sxs-lookup"><span data-stu-id="805e8-170">Audit category.</span></span> <span data-ttu-id="805e8-171">只读。</span><span class="sxs-lookup"><span data-stu-id="805e8-171">Read-only.</span></span>|

### <a name="cloudpcauditactivityoperationtype-values"></a><span data-ttu-id="805e8-172">cloudPcAuditActivityOperationType 值</span><span class="sxs-lookup"><span data-stu-id="805e8-172">cloudPcAuditActivityOperationType values</span></span>

|<span data-ttu-id="805e8-173">成员</span><span class="sxs-lookup"><span data-stu-id="805e8-173">Member</span></span>|<span data-ttu-id="805e8-174">说明</span><span class="sxs-lookup"><span data-stu-id="805e8-174">Description</span></span>|
|:---|:---|
|<span data-ttu-id="805e8-175">create</span><span class="sxs-lookup"><span data-stu-id="805e8-175">create</span></span>|<span data-ttu-id="805e8-176">创建操作。</span><span class="sxs-lookup"><span data-stu-id="805e8-176">Create operation.</span></span>|
|<span data-ttu-id="805e8-177">delete</span><span class="sxs-lookup"><span data-stu-id="805e8-177">delete</span></span>|<span data-ttu-id="805e8-178">删除操作。</span><span class="sxs-lookup"><span data-stu-id="805e8-178">Delete operation.</span></span>|
|<span data-ttu-id="805e8-179">patch</span><span class="sxs-lookup"><span data-stu-id="805e8-179">patch</span></span>|<span data-ttu-id="805e8-180">修补程序操作。</span><span class="sxs-lookup"><span data-stu-id="805e8-180">Patch operation.</span></span>|
|<span data-ttu-id="805e8-181">other</span><span class="sxs-lookup"><span data-stu-id="805e8-181">other</span></span>|<span data-ttu-id="805e8-182">其他操作。</span><span class="sxs-lookup"><span data-stu-id="805e8-182">Other operation.</span></span>|

### <a name="cloudpcauditactivityresult-values"></a><span data-ttu-id="805e8-183">cloudPcAuditActivityResult 值</span><span class="sxs-lookup"><span data-stu-id="805e8-183">cloudPcAuditActivityResult values</span></span>

|<span data-ttu-id="805e8-184">成员</span><span class="sxs-lookup"><span data-stu-id="805e8-184">Member</span></span>|<span data-ttu-id="805e8-185">说明</span><span class="sxs-lookup"><span data-stu-id="805e8-185">Description</span></span>|
|:---|:---|
|<span data-ttu-id="805e8-186">success</span><span class="sxs-lookup"><span data-stu-id="805e8-186">success</span></span>|<span data-ttu-id="805e8-187">操作成功。</span><span class="sxs-lookup"><span data-stu-id="805e8-187">Operation succeeded.</span></span>|
|<span data-ttu-id="805e8-188">clientError</span><span class="sxs-lookup"><span data-stu-id="805e8-188">clientError</span></span>|<span data-ttu-id="805e8-189">操作失败，出现客户端错误。</span><span class="sxs-lookup"><span data-stu-id="805e8-189">Operation failed with client error.</span></span>|
|<span data-ttu-id="805e8-190">failure</span><span class="sxs-lookup"><span data-stu-id="805e8-190">failure</span></span>|<span data-ttu-id="805e8-191">操作失败。</span><span class="sxs-lookup"><span data-stu-id="805e8-191">Operation failed.</span></span>|
|<span data-ttu-id="805e8-192">timeExceeded</span><span class="sxs-lookup"><span data-stu-id="805e8-192">timeExceeded</span></span>|<span data-ttu-id="805e8-193">操作失败，超时。</span><span class="sxs-lookup"><span data-stu-id="805e8-193">Operation failed with timeout.</span></span>|
|<span data-ttu-id="805e8-194">other</span><span class="sxs-lookup"><span data-stu-id="805e8-194">other</span></span>|<span data-ttu-id="805e8-195">其他结果。</span><span class="sxs-lookup"><span data-stu-id="805e8-195">Other result.</span></span>|

### <a name="cloudpcauditcategory-values"></a><span data-ttu-id="805e8-196">cloudPcAuditCategory 值</span><span class="sxs-lookup"><span data-stu-id="805e8-196">cloudPcAuditCategory values</span></span>

|<span data-ttu-id="805e8-197">成员</span><span class="sxs-lookup"><span data-stu-id="805e8-197">Member</span></span>|<span data-ttu-id="805e8-198">说明</span><span class="sxs-lookup"><span data-stu-id="805e8-198">Description</span></span>|
|:---|:---|
|<span data-ttu-id="805e8-199">cloudPC</span><span class="sxs-lookup"><span data-stu-id="805e8-199">cloudPC</span></span>|<span data-ttu-id="805e8-200">云电脑类别。</span><span class="sxs-lookup"><span data-stu-id="805e8-200">Cloud PC category.</span></span>|
|<span data-ttu-id="805e8-201">other</span><span class="sxs-lookup"><span data-stu-id="805e8-201">other</span></span> |<span data-ttu-id="805e8-202">其他类别。</span><span class="sxs-lookup"><span data-stu-id="805e8-202">Other category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="805e8-203">关系</span><span class="sxs-lookup"><span data-stu-id="805e8-203">Relationships</span></span>

<span data-ttu-id="805e8-204">无。</span><span class="sxs-lookup"><span data-stu-id="805e8-204">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="805e8-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="805e8-205">JSON representation</span></span>

<span data-ttu-id="805e8-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="805e8-206">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.cloudPcAuditActor",
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
        "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
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
  "correlationId": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditProperty",
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
