---
title: 创建 auditEvent
description: 创建新的 auditEvent 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92ebeabe17d9d3f59ff5abda95daabd09fbf7f2b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760604"
---
# <a name="create-auditevent"></a><span data-ttu-id="32161-103">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="32161-103">Create auditEvent</span></span>

> <span data-ttu-id="32161-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32161-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32161-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32161-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32161-106">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32161-106">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32161-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="32161-107">Prerequisites</span></span>
<span data-ttu-id="32161-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32161-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32161-110">Permission type</span></span>|<span data-ttu-id="32161-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32161-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32161-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32161-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32161-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32161-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32161-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32161-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32161-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32161-115">Not supported.</span></span>|
|<span data-ttu-id="32161-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32161-116">Application</span></span>|<span data-ttu-id="32161-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32161-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32161-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32161-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="32161-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="32161-119">Request headers</span></span>
|<span data-ttu-id="32161-120">标头</span><span class="sxs-lookup"><span data-stu-id="32161-120">Header</span></span>|<span data-ttu-id="32161-121">值</span><span class="sxs-lookup"><span data-stu-id="32161-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32161-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32161-122">Authorization</span></span>|<span data-ttu-id="32161-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32161-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32161-124">接受</span><span class="sxs-lookup"><span data-stu-id="32161-124">Accept</span></span>|<span data-ttu-id="32161-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32161-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32161-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="32161-126">Request body</span></span>
<span data-ttu-id="32161-127">在请求正文中，提供 auditEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32161-127">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="32161-128">下表显示了创建 auditEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="32161-128">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="32161-129">属性</span><span class="sxs-lookup"><span data-stu-id="32161-129">Property</span></span>|<span data-ttu-id="32161-130">类型</span><span class="sxs-lookup"><span data-stu-id="32161-130">Type</span></span>|<span data-ttu-id="32161-131">说明</span><span class="sxs-lookup"><span data-stu-id="32161-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32161-132">id</span><span class="sxs-lookup"><span data-stu-id="32161-132">id</span></span>|<span data-ttu-id="32161-133">String</span><span class="sxs-lookup"><span data-stu-id="32161-133">String</span></span>|<span data-ttu-id="32161-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="32161-134">Key of the entity.</span></span>|
|<span data-ttu-id="32161-135">displayName</span><span class="sxs-lookup"><span data-stu-id="32161-135">displayName</span></span>|<span data-ttu-id="32161-136">String</span><span class="sxs-lookup"><span data-stu-id="32161-136">String</span></span>|<span data-ttu-id="32161-137">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="32161-137">Event display name.</span></span>|
|<span data-ttu-id="32161-138">componentName</span><span class="sxs-lookup"><span data-stu-id="32161-138">componentName</span></span>|<span data-ttu-id="32161-139">String</span><span class="sxs-lookup"><span data-stu-id="32161-139">String</span></span>|<span data-ttu-id="32161-140">组件名称。</span><span class="sxs-lookup"><span data-stu-id="32161-140">Component name.</span></span>|
|<span data-ttu-id="32161-141">actor</span><span class="sxs-lookup"><span data-stu-id="32161-141">actor</span></span>|[<span data-ttu-id="32161-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="32161-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="32161-143">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="32161-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="32161-144">activity</span><span class="sxs-lookup"><span data-stu-id="32161-144">activity</span></span>|<span data-ttu-id="32161-145">String</span><span class="sxs-lookup"><span data-stu-id="32161-145">String</span></span>|<span data-ttu-id="32161-146">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="32161-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="32161-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="32161-147">activityDateTime</span></span>|<span data-ttu-id="32161-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32161-148">DateTimeOffset</span></span>|<span data-ttu-id="32161-149">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="32161-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="32161-150">activityType</span><span class="sxs-lookup"><span data-stu-id="32161-150">activityType</span></span>|<span data-ttu-id="32161-151">String</span><span class="sxs-lookup"><span data-stu-id="32161-151">String</span></span>|<span data-ttu-id="32161-152">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="32161-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="32161-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="32161-153">activityOperationType</span></span>|<span data-ttu-id="32161-154">String</span><span class="sxs-lookup"><span data-stu-id="32161-154">String</span></span>|<span data-ttu-id="32161-155">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="32161-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="32161-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="32161-156">activityResult</span></span>|<span data-ttu-id="32161-157">String</span><span class="sxs-lookup"><span data-stu-id="32161-157">String</span></span>|<span data-ttu-id="32161-158">活动结果。</span><span class="sxs-lookup"><span data-stu-id="32161-158">The result of the activity.</span></span>|
|<span data-ttu-id="32161-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="32161-159">correlationId</span></span>|<span data-ttu-id="32161-160">Guid</span><span class="sxs-lookup"><span data-stu-id="32161-160">Guid</span></span>|<span data-ttu-id="32161-161">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="32161-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="32161-162">resources</span><span class="sxs-lookup"><span data-stu-id="32161-162">resources</span></span>|<span data-ttu-id="32161-163">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32161-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="32161-164">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="32161-164">Resources being modified.</span></span>|
|<span data-ttu-id="32161-165">“类别”</span><span class="sxs-lookup"><span data-stu-id="32161-165">category</span></span>|<span data-ttu-id="32161-166">String</span><span class="sxs-lookup"><span data-stu-id="32161-166">String</span></span>|<span data-ttu-id="32161-167">审核类别。</span><span class="sxs-lookup"><span data-stu-id="32161-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="32161-168">响应</span><span class="sxs-lookup"><span data-stu-id="32161-168">Response</span></span>
<span data-ttu-id="32161-169">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32161-169">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32161-170">示例</span><span class="sxs-lookup"><span data-stu-id="32161-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="32161-171">请求</span><span class="sxs-lookup"><span data-stu-id="32161-171">Request</span></span>
<span data-ttu-id="32161-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32161-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1603

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "Display Name value",
        "roleScopeTagId": "Role Scope Tag Id value"
      }
    ]
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="32161-173">响应</span><span class="sxs-lookup"><span data-stu-id="32161-173">Response</span></span>
<span data-ttu-id="32161-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32161-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1652

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "Display Name value",
        "roleScopeTagId": "Role Scope Tag Id value"
      }
    ]
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```




