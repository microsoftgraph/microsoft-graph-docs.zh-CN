---
title: 创建 auditEvent
description: 创建新的 auditEvent 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1661c85ee331dfc2c4c1ac6120f228d43185d7f0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128528"
---
# <a name="create-auditevent"></a><span data-ttu-id="41a16-103">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="41a16-103">Create auditEvent</span></span>

<span data-ttu-id="41a16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41a16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41a16-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41a16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41a16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41a16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41a16-107">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41a16-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41a16-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41a16-108">Prerequisites</span></span>
<span data-ttu-id="41a16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41a16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41a16-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41a16-111">Permission type</span></span>|<span data-ttu-id="41a16-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41a16-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41a16-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41a16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41a16-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41a16-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41a16-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41a16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41a16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41a16-116">Not supported.</span></span>|
|<span data-ttu-id="41a16-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41a16-117">Application</span></span>|<span data-ttu-id="41a16-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41a16-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41a16-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41a16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="41a16-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41a16-120">Request headers</span></span>
|<span data-ttu-id="41a16-121">标头</span><span class="sxs-lookup"><span data-stu-id="41a16-121">Header</span></span>|<span data-ttu-id="41a16-122">值</span><span class="sxs-lookup"><span data-stu-id="41a16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41a16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41a16-123">Authorization</span></span>|<span data-ttu-id="41a16-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41a16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41a16-125">接受</span><span class="sxs-lookup"><span data-stu-id="41a16-125">Accept</span></span>|<span data-ttu-id="41a16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41a16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41a16-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41a16-127">Request body</span></span>
<span data-ttu-id="41a16-128">在请求正文中，提供 auditEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41a16-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="41a16-129">下表显示了创建 auditEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41a16-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="41a16-130">属性</span><span class="sxs-lookup"><span data-stu-id="41a16-130">Property</span></span>|<span data-ttu-id="41a16-131">类型</span><span class="sxs-lookup"><span data-stu-id="41a16-131">Type</span></span>|<span data-ttu-id="41a16-132">说明</span><span class="sxs-lookup"><span data-stu-id="41a16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41a16-133">id</span><span class="sxs-lookup"><span data-stu-id="41a16-133">id</span></span>|<span data-ttu-id="41a16-134">String</span><span class="sxs-lookup"><span data-stu-id="41a16-134">String</span></span>|<span data-ttu-id="41a16-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41a16-135">Key of the entity.</span></span>|
|<span data-ttu-id="41a16-136">displayName</span><span class="sxs-lookup"><span data-stu-id="41a16-136">displayName</span></span>|<span data-ttu-id="41a16-137">String</span><span class="sxs-lookup"><span data-stu-id="41a16-137">String</span></span>|<span data-ttu-id="41a16-138">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="41a16-138">Event display name.</span></span>|
|<span data-ttu-id="41a16-139">componentName</span><span class="sxs-lookup"><span data-stu-id="41a16-139">componentName</span></span>|<span data-ttu-id="41a16-140">String</span><span class="sxs-lookup"><span data-stu-id="41a16-140">String</span></span>|<span data-ttu-id="41a16-141">组件名称。</span><span class="sxs-lookup"><span data-stu-id="41a16-141">Component name.</span></span>|
|<span data-ttu-id="41a16-142">actor</span><span class="sxs-lookup"><span data-stu-id="41a16-142">actor</span></span>|[<span data-ttu-id="41a16-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="41a16-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="41a16-144">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="41a16-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="41a16-145">activity</span><span class="sxs-lookup"><span data-stu-id="41a16-145">activity</span></span>|<span data-ttu-id="41a16-146">String</span><span class="sxs-lookup"><span data-stu-id="41a16-146">String</span></span>|<span data-ttu-id="41a16-147">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="41a16-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="41a16-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="41a16-148">activityDateTime</span></span>|<span data-ttu-id="41a16-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41a16-149">DateTimeOffset</span></span>|<span data-ttu-id="41a16-150">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="41a16-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="41a16-151">activityType</span><span class="sxs-lookup"><span data-stu-id="41a16-151">activityType</span></span>|<span data-ttu-id="41a16-152">String</span><span class="sxs-lookup"><span data-stu-id="41a16-152">String</span></span>|<span data-ttu-id="41a16-153">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="41a16-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="41a16-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="41a16-154">activityOperationType</span></span>|<span data-ttu-id="41a16-155">String</span><span class="sxs-lookup"><span data-stu-id="41a16-155">String</span></span>|<span data-ttu-id="41a16-156">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="41a16-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="41a16-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="41a16-157">activityResult</span></span>|<span data-ttu-id="41a16-158">String</span><span class="sxs-lookup"><span data-stu-id="41a16-158">String</span></span>|<span data-ttu-id="41a16-159">活动结果。</span><span class="sxs-lookup"><span data-stu-id="41a16-159">The result of the activity.</span></span>|
|<span data-ttu-id="41a16-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="41a16-160">correlationId</span></span>|<span data-ttu-id="41a16-161">Guid</span><span class="sxs-lookup"><span data-stu-id="41a16-161">Guid</span></span>|<span data-ttu-id="41a16-162">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="41a16-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="41a16-163">resources</span><span class="sxs-lookup"><span data-stu-id="41a16-163">resources</span></span>|<span data-ttu-id="41a16-164">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41a16-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="41a16-165">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="41a16-165">Resources being modified.</span></span>|
|<span data-ttu-id="41a16-166">“类别”</span><span class="sxs-lookup"><span data-stu-id="41a16-166">category</span></span>|<span data-ttu-id="41a16-167">String</span><span class="sxs-lookup"><span data-stu-id="41a16-167">String</span></span>|<span data-ttu-id="41a16-168">审核类别。</span><span class="sxs-lookup"><span data-stu-id="41a16-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="41a16-169">响应</span><span class="sxs-lookup"><span data-stu-id="41a16-169">Response</span></span>
<span data-ttu-id="41a16-170">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41a16-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41a16-171">示例</span><span class="sxs-lookup"><span data-stu-id="41a16-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="41a16-172">请求</span><span class="sxs-lookup"><span data-stu-id="41a16-172">Request</span></span>
<span data-ttu-id="41a16-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41a16-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1697

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
    ],
    "remoteTenantId": "Remote Tenant Id value",
    "remoteUserId": "Remote User Id value"
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

### <a name="response"></a><span data-ttu-id="41a16-174">响应</span><span class="sxs-lookup"><span data-stu-id="41a16-174">Response</span></span>
<span data-ttu-id="41a16-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41a16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1746

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
    ],
    "remoteTenantId": "Remote Tenant Id value",
    "remoteUserId": "Remote User Id value"
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




