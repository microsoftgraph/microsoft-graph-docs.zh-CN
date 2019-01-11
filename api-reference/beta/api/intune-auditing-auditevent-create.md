---
title: 创建 auditEvent
description: 创建新的 auditEvent 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dcc7a84e22b86e4ec0f9e5d17eb05f75cbe83c6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837882"
---
# <a name="create-auditevent"></a><span data-ttu-id="c3965-103">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="c3965-103">Create auditEvent</span></span>

> <span data-ttu-id="c3965-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c3965-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3965-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3965-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3965-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c3965-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3965-107">创建新的 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3965-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3965-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3965-108">Prerequisites</span></span>
<span data-ttu-id="c3965-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c3965-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3965-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3965-111">Permission type</span></span>|<span data-ttu-id="c3965-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3965-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3965-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3965-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3965-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3965-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3965-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3965-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3965-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3965-116">Not supported.</span></span>|
|<span data-ttu-id="c3965-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3965-117">Application</span></span>|<span data-ttu-id="c3965-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3965-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3965-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3965-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="c3965-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3965-120">Request headers</span></span>
|<span data-ttu-id="c3965-121">标头</span><span class="sxs-lookup"><span data-stu-id="c3965-121">Header</span></span>|<span data-ttu-id="c3965-122">值</span><span class="sxs-lookup"><span data-stu-id="c3965-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3965-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3965-123">Authorization</span></span>|<span data-ttu-id="c3965-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3965-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3965-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3965-125">Accept</span></span>|<span data-ttu-id="c3965-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3965-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3965-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3965-127">Request body</span></span>
<span data-ttu-id="c3965-128">在请求正文中，提供 auditEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3965-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="c3965-129">下表显示了创建 auditEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3965-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="c3965-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3965-130">Property</span></span>|<span data-ttu-id="c3965-131">类型</span><span class="sxs-lookup"><span data-stu-id="c3965-131">Type</span></span>|<span data-ttu-id="c3965-132">说明</span><span class="sxs-lookup"><span data-stu-id="c3965-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3965-133">id</span><span class="sxs-lookup"><span data-stu-id="c3965-133">id</span></span>|<span data-ttu-id="c3965-134">String</span><span class="sxs-lookup"><span data-stu-id="c3965-134">String</span></span>|<span data-ttu-id="c3965-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3965-135">Key of the entity.</span></span>|
|<span data-ttu-id="c3965-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c3965-136">displayName</span></span>|<span data-ttu-id="c3965-137">String</span><span class="sxs-lookup"><span data-stu-id="c3965-137">String</span></span>|<span data-ttu-id="c3965-138">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3965-138">Event display name.</span></span>|
|<span data-ttu-id="c3965-139">componentName</span><span class="sxs-lookup"><span data-stu-id="c3965-139">componentName</span></span>|<span data-ttu-id="c3965-140">String</span><span class="sxs-lookup"><span data-stu-id="c3965-140">String</span></span>|<span data-ttu-id="c3965-141">组件名称。</span><span class="sxs-lookup"><span data-stu-id="c3965-141">Component name.</span></span>|
|<span data-ttu-id="c3965-142">actor</span><span class="sxs-lookup"><span data-stu-id="c3965-142">actor</span></span>|[<span data-ttu-id="c3965-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="c3965-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="c3965-144">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="c3965-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="c3965-145">activity</span><span class="sxs-lookup"><span data-stu-id="c3965-145">activity</span></span>|<span data-ttu-id="c3965-146">String</span><span class="sxs-lookup"><span data-stu-id="c3965-146">String</span></span>|<span data-ttu-id="c3965-147">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="c3965-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="c3965-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="c3965-148">activityDateTime</span></span>|<span data-ttu-id="c3965-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3965-149">DateTimeOffset</span></span>|<span data-ttu-id="c3965-150">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="c3965-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="c3965-151">activityType</span><span class="sxs-lookup"><span data-stu-id="c3965-151">activityType</span></span>|<span data-ttu-id="c3965-152">String</span><span class="sxs-lookup"><span data-stu-id="c3965-152">String</span></span>|<span data-ttu-id="c3965-153">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="c3965-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="c3965-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="c3965-154">activityOperationType</span></span>|<span data-ttu-id="c3965-155">String</span><span class="sxs-lookup"><span data-stu-id="c3965-155">String</span></span>|<span data-ttu-id="c3965-156">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="c3965-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="c3965-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="c3965-157">activityResult</span></span>|<span data-ttu-id="c3965-158">String</span><span class="sxs-lookup"><span data-stu-id="c3965-158">String</span></span>|<span data-ttu-id="c3965-159">活动结果。</span><span class="sxs-lookup"><span data-stu-id="c3965-159">The result of the activity.</span></span>|
|<span data-ttu-id="c3965-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="c3965-160">correlationId</span></span>|<span data-ttu-id="c3965-161">Guid</span><span class="sxs-lookup"><span data-stu-id="c3965-161">Guid</span></span>|<span data-ttu-id="c3965-162">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="c3965-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="c3965-163">resources</span><span class="sxs-lookup"><span data-stu-id="c3965-163">resources</span></span>|<span data-ttu-id="c3965-164">[auditResource](../resources/intune-auditing-auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3965-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="c3965-165">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="c3965-165">Resources being modified.</span></span>|
|<span data-ttu-id="c3965-166">category</span><span class="sxs-lookup"><span data-stu-id="c3965-166">category</span></span>|<span data-ttu-id="c3965-167">String</span><span class="sxs-lookup"><span data-stu-id="c3965-167">String</span></span>|<span data-ttu-id="c3965-168">审核类别。</span><span class="sxs-lookup"><span data-stu-id="c3965-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="c3965-169">响应</span><span class="sxs-lookup"><span data-stu-id="c3965-169">Response</span></span>
<span data-ttu-id="c3965-170">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [auditEvent](../resources/intune-auditing-auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3965-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3965-171">示例</span><span class="sxs-lookup"><span data-stu-id="c3965-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3965-172">请求</span><span class="sxs-lookup"><span data-stu-id="c3965-172">Request</span></span>
<span data-ttu-id="c3965-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3965-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
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

### <a name="response"></a><span data-ttu-id="c3965-174">响应</span><span class="sxs-lookup"><span data-stu-id="c3965-174">Response</span></span>
<span data-ttu-id="c3965-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3965-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





