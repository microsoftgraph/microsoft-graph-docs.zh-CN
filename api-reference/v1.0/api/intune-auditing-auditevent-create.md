---
title: 创建 auditEvent
description: 创建新的 auditEvent 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a08e7266070e3cbaaa0f639660d806d487ef6cb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987627"
---
# <a name="create-auditevent"></a><span data-ttu-id="65b9c-103">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="65b9c-103">Create auditEvent</span></span>

> <span data-ttu-id="65b9c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65b9c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65b9c-105">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65b9c-105">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65b9c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="65b9c-106">Prerequisites</span></span>
<span data-ttu-id="65b9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65b9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65b9c-109">Permission type</span></span>|<span data-ttu-id="65b9c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65b9c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65b9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65b9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65b9c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b9c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65b9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65b9c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65b9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65b9c-114">Not supported.</span></span>|
|<span data-ttu-id="65b9c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65b9c-115">Application</span></span>|<span data-ttu-id="65b9c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65b9c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65b9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65b9c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="65b9c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65b9c-118">Request headers</span></span>
|<span data-ttu-id="65b9c-119">标头</span><span class="sxs-lookup"><span data-stu-id="65b9c-119">Header</span></span>|<span data-ttu-id="65b9c-120">值</span><span class="sxs-lookup"><span data-stu-id="65b9c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65b9c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b9c-121">Authorization</span></span>|<span data-ttu-id="65b9c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65b9c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65b9c-123">接受</span><span class="sxs-lookup"><span data-stu-id="65b9c-123">Accept</span></span>|<span data-ttu-id="65b9c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65b9c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b9c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="65b9c-125">Request body</span></span>
<span data-ttu-id="65b9c-126">在请求正文中，提供 auditEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65b9c-126">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="65b9c-127">下表显示了创建 auditEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65b9c-127">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="65b9c-128">属性</span><span class="sxs-lookup"><span data-stu-id="65b9c-128">Property</span></span>|<span data-ttu-id="65b9c-129">类型</span><span class="sxs-lookup"><span data-stu-id="65b9c-129">Type</span></span>|<span data-ttu-id="65b9c-130">说明</span><span class="sxs-lookup"><span data-stu-id="65b9c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b9c-131">id</span><span class="sxs-lookup"><span data-stu-id="65b9c-131">id</span></span>|<span data-ttu-id="65b9c-132">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-132">String</span></span>|<span data-ttu-id="65b9c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65b9c-133">Key of the entity.</span></span>|
|<span data-ttu-id="65b9c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="65b9c-134">displayName</span></span>|<span data-ttu-id="65b9c-135">字符串</span><span class="sxs-lookup"><span data-stu-id="65b9c-135">String</span></span>|<span data-ttu-id="65b9c-136">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="65b9c-136">Event display name.</span></span>|
|<span data-ttu-id="65b9c-137">componentName</span><span class="sxs-lookup"><span data-stu-id="65b9c-137">componentName</span></span>|<span data-ttu-id="65b9c-138">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-138">String</span></span>|<span data-ttu-id="65b9c-139">组件名称。</span><span class="sxs-lookup"><span data-stu-id="65b9c-139">Component name.</span></span>|
|<span data-ttu-id="65b9c-140">actor</span><span class="sxs-lookup"><span data-stu-id="65b9c-140">actor</span></span>|[<span data-ttu-id="65b9c-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="65b9c-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="65b9c-142">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="65b9c-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="65b9c-143">activity</span><span class="sxs-lookup"><span data-stu-id="65b9c-143">activity</span></span>|<span data-ttu-id="65b9c-144">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-144">String</span></span>|<span data-ttu-id="65b9c-145">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="65b9c-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="65b9c-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="65b9c-146">activityDateTime</span></span>|<span data-ttu-id="65b9c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65b9c-147">DateTimeOffset</span></span>|<span data-ttu-id="65b9c-148">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="65b9c-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="65b9c-149">activityType</span><span class="sxs-lookup"><span data-stu-id="65b9c-149">activityType</span></span>|<span data-ttu-id="65b9c-150">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-150">String</span></span>|<span data-ttu-id="65b9c-151">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="65b9c-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="65b9c-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="65b9c-152">activityOperationType</span></span>|<span data-ttu-id="65b9c-153">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-153">String</span></span>|<span data-ttu-id="65b9c-154">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="65b9c-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="65b9c-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="65b9c-155">activityResult</span></span>|<span data-ttu-id="65b9c-156">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-156">String</span></span>|<span data-ttu-id="65b9c-157">活动结果。</span><span class="sxs-lookup"><span data-stu-id="65b9c-157">The result of the activity.</span></span>|
|<span data-ttu-id="65b9c-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="65b9c-158">correlationId</span></span>|<span data-ttu-id="65b9c-159">Guid</span><span class="sxs-lookup"><span data-stu-id="65b9c-159">Guid</span></span>|<span data-ttu-id="65b9c-160">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="65b9c-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="65b9c-161">resources</span><span class="sxs-lookup"><span data-stu-id="65b9c-161">resources</span></span>|<span data-ttu-id="65b9c-162">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65b9c-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="65b9c-163">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="65b9c-163">Resources being modified.</span></span>|
|<span data-ttu-id="65b9c-164">category</span><span class="sxs-lookup"><span data-stu-id="65b9c-164">category</span></span>|<span data-ttu-id="65b9c-165">String</span><span class="sxs-lookup"><span data-stu-id="65b9c-165">String</span></span>|<span data-ttu-id="65b9c-166">审核类别。</span><span class="sxs-lookup"><span data-stu-id="65b9c-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="65b9c-167">响应</span><span class="sxs-lookup"><span data-stu-id="65b9c-167">Response</span></span>
<span data-ttu-id="65b9c-168">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65b9c-168">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65b9c-169">示例</span><span class="sxs-lookup"><span data-stu-id="65b9c-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="65b9c-170">请求</span><span class="sxs-lookup"><span data-stu-id="65b9c-170">Request</span></span>
<span data-ttu-id="65b9c-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65b9c-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1390

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
    "userId": "User Id value"
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

### <a name="response"></a><span data-ttu-id="65b9c-172">响应</span><span class="sxs-lookup"><span data-stu-id="65b9c-172">Response</span></span>
<span data-ttu-id="65b9c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65b9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

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
    "userId": "User Id value"
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



