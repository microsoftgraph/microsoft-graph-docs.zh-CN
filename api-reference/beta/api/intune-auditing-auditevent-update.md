---
title: 更新 auditEvent
description: 更新 auditEvent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a4b4a0e2ef8355450f039608a7769a613296cc2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450389"
---
# <a name="update-auditevent"></a><span data-ttu-id="06748-103">更新 auditEvent</span><span class="sxs-lookup"><span data-stu-id="06748-103">Update auditEvent</span></span>

<span data-ttu-id="06748-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="06748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06748-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06748-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06748-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06748-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06748-107">更新 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06748-107">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06748-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="06748-108">Prerequisites</span></span>
<span data-ttu-id="06748-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06748-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="06748-111">Permission type</span></span>|<span data-ttu-id="06748-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06748-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06748-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06748-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06748-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06748-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06748-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06748-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06748-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06748-116">Not supported.</span></span>|
|<span data-ttu-id="06748-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="06748-117">Application</span></span>|<span data-ttu-id="06748-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06748-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06748-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06748-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="06748-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="06748-120">Request headers</span></span>
|<span data-ttu-id="06748-121">标头</span><span class="sxs-lookup"><span data-stu-id="06748-121">Header</span></span>|<span data-ttu-id="06748-122">值</span><span class="sxs-lookup"><span data-stu-id="06748-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06748-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06748-123">Authorization</span></span>|<span data-ttu-id="06748-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06748-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06748-125">接受</span><span class="sxs-lookup"><span data-stu-id="06748-125">Accept</span></span>|<span data-ttu-id="06748-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06748-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06748-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="06748-127">Request body</span></span>
<span data-ttu-id="06748-128">在请求正文中，提供 [auditEvent](../resources/intune-auditing-auditevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06748-128">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="06748-129">下表显示了创建 [auditEvent](../resources/intune-auditing-auditevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06748-129">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="06748-130">属性</span><span class="sxs-lookup"><span data-stu-id="06748-130">Property</span></span>|<span data-ttu-id="06748-131">类型</span><span class="sxs-lookup"><span data-stu-id="06748-131">Type</span></span>|<span data-ttu-id="06748-132">说明</span><span class="sxs-lookup"><span data-stu-id="06748-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06748-133">id</span><span class="sxs-lookup"><span data-stu-id="06748-133">id</span></span>|<span data-ttu-id="06748-134">String</span><span class="sxs-lookup"><span data-stu-id="06748-134">String</span></span>|<span data-ttu-id="06748-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06748-135">Key of the entity.</span></span>|
|<span data-ttu-id="06748-136">displayName</span><span class="sxs-lookup"><span data-stu-id="06748-136">displayName</span></span>|<span data-ttu-id="06748-137">String</span><span class="sxs-lookup"><span data-stu-id="06748-137">String</span></span>|<span data-ttu-id="06748-138">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="06748-138">Event display name.</span></span>|
|<span data-ttu-id="06748-139">componentName</span><span class="sxs-lookup"><span data-stu-id="06748-139">componentName</span></span>|<span data-ttu-id="06748-140">String</span><span class="sxs-lookup"><span data-stu-id="06748-140">String</span></span>|<span data-ttu-id="06748-141">组件名称。</span><span class="sxs-lookup"><span data-stu-id="06748-141">Component name.</span></span>|
|<span data-ttu-id="06748-142">actor</span><span class="sxs-lookup"><span data-stu-id="06748-142">actor</span></span>|[<span data-ttu-id="06748-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="06748-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="06748-144">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="06748-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="06748-145">activity</span><span class="sxs-lookup"><span data-stu-id="06748-145">activity</span></span>|<span data-ttu-id="06748-146">String</span><span class="sxs-lookup"><span data-stu-id="06748-146">String</span></span>|<span data-ttu-id="06748-147">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="06748-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="06748-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="06748-148">activityDateTime</span></span>|<span data-ttu-id="06748-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06748-149">DateTimeOffset</span></span>|<span data-ttu-id="06748-150">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="06748-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="06748-151">activityType</span><span class="sxs-lookup"><span data-stu-id="06748-151">activityType</span></span>|<span data-ttu-id="06748-152">String</span><span class="sxs-lookup"><span data-stu-id="06748-152">String</span></span>|<span data-ttu-id="06748-153">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="06748-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="06748-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="06748-154">activityOperationType</span></span>|<span data-ttu-id="06748-155">String</span><span class="sxs-lookup"><span data-stu-id="06748-155">String</span></span>|<span data-ttu-id="06748-156">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="06748-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="06748-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="06748-157">activityResult</span></span>|<span data-ttu-id="06748-158">String</span><span class="sxs-lookup"><span data-stu-id="06748-158">String</span></span>|<span data-ttu-id="06748-159">活动结果。</span><span class="sxs-lookup"><span data-stu-id="06748-159">The result of the activity.</span></span>|
|<span data-ttu-id="06748-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="06748-160">correlationId</span></span>|<span data-ttu-id="06748-161">Guid</span><span class="sxs-lookup"><span data-stu-id="06748-161">Guid</span></span>|<span data-ttu-id="06748-162">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="06748-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="06748-163">resources</span><span class="sxs-lookup"><span data-stu-id="06748-163">resources</span></span>|<span data-ttu-id="06748-164">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06748-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="06748-165">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="06748-165">Resources being modified.</span></span>|
|<span data-ttu-id="06748-166">“类别”</span><span class="sxs-lookup"><span data-stu-id="06748-166">category</span></span>|<span data-ttu-id="06748-167">String</span><span class="sxs-lookup"><span data-stu-id="06748-167">String</span></span>|<span data-ttu-id="06748-168">审核类别。</span><span class="sxs-lookup"><span data-stu-id="06748-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="06748-169">响应</span><span class="sxs-lookup"><span data-stu-id="06748-169">Response</span></span>
<span data-ttu-id="06748-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06748-170">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06748-171">示例</span><span class="sxs-lookup"><span data-stu-id="06748-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="06748-172">请求</span><span class="sxs-lookup"><span data-stu-id="06748-172">Request</span></span>
<span data-ttu-id="06748-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06748-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
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

### <a name="response"></a><span data-ttu-id="06748-174">响应</span><span class="sxs-lookup"><span data-stu-id="06748-174">Response</span></span>
<span data-ttu-id="06748-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





