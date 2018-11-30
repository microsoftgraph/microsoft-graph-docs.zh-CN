---
title: 获取 deviceAndAppManagementRoleAssignment
description: 读取 deviceAndAppManagementRoleAssignment 对象的属性和关系。
ms.openlocfilehash: 9791019c586b322c96506059ab36bc7c6705c980
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009268"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="dd0cf-103">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="dd0cf-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="dd0cf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd0cf-105">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd0cf-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd0cf-106">Prerequisites</span></span>
<span data-ttu-id="dd0cf-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="dd0cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd0cf-109">Permission type</span></span>|<span data-ttu-id="dd0cf-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd0cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd0cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd0cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd0cf-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0cf-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="dd0cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd0cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd0cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-114">Not supported.</span></span>|
|<span data-ttu-id="dd0cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd0cf-115">Application</span></span>|<span data-ttu-id="dd0cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd0cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd0cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd0cf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dd0cf-118">Optional query parameters</span></span>
<span data-ttu-id="dd0cf-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dd0cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd0cf-120">Request headers</span></span>
|<span data-ttu-id="dd0cf-121">标头</span><span class="sxs-lookup"><span data-stu-id="dd0cf-121">Header</span></span>|<span data-ttu-id="dd0cf-122">值</span><span class="sxs-lookup"><span data-stu-id="dd0cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd0cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd0cf-123">Authorization</span></span>|<span data-ttu-id="dd0cf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd0cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd0cf-125">Accept</span></span>|<span data-ttu-id="dd0cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd0cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd0cf-127">Request body</span></span>
<span data-ttu-id="dd0cf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd0cf-129">响应</span><span class="sxs-lookup"><span data-stu-id="dd0cf-129">Response</span></span>
<span data-ttu-id="dd0cf-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd0cf-131">示例</span><span class="sxs-lookup"><span data-stu-id="dd0cf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd0cf-132">请求</span><span class="sxs-lookup"><span data-stu-id="dd0cf-132">Request</span></span>
<span data-ttu-id="dd0cf-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="dd0cf-134">响应</span><span class="sxs-lookup"><span data-stu-id="dd0cf-134">Response</span></span>
<span data-ttu-id="dd0cf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd0cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```



