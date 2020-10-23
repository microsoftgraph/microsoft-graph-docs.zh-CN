---
title: getAssignedRoleIdsForLoggedInUser 函数
description: 检索当前已通过身份验证的用户分配的角色定义和角色分配。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2000082fc45ac040a66db8e5df16262694d07949
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732042"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="efd64-103">getAssignedRoleIdsForLoggedInUser 函数</span><span class="sxs-lookup"><span data-stu-id="efd64-103">getAssignedRoleIdsForLoggedInUser function</span></span>

<span data-ttu-id="efd64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efd64-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="efd64-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="efd64-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="efd64-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efd64-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efd64-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd64-108">检索当前已通过身份验证的用户分配的角色定义和角色分配。</span><span class="sxs-lookup"><span data-stu-id="efd64-108">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efd64-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="efd64-109">Prerequisites</span></span>
<span data-ttu-id="efd64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd64-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd64-112">Permission type</span></span>|<span data-ttu-id="efd64-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efd64-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efd64-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd64-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="efd64-115">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="efd64-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="efd64-116">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="efd64-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="efd64-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd64-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efd64-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd64-118">Not supported.</span></span>|
|<span data-ttu-id="efd64-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd64-119">Application</span></span>||
| <span data-ttu-id="efd64-120">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="efd64-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="efd64-121">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="efd64-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="efd64-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd64-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="efd64-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd64-123">Request headers</span></span>
|<span data-ttu-id="efd64-124">标头</span><span class="sxs-lookup"><span data-stu-id="efd64-124">Header</span></span>|<span data-ttu-id="efd64-125">值</span><span class="sxs-lookup"><span data-stu-id="efd64-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efd64-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd64-126">Authorization</span></span>|<span data-ttu-id="efd64-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efd64-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efd64-128">接受</span><span class="sxs-lookup"><span data-stu-id="efd64-128">Accept</span></span>|<span data-ttu-id="efd64-129">application/json</span><span class="sxs-lookup"><span data-stu-id="efd64-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd64-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd64-130">Request body</span></span>
<span data-ttu-id="efd64-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efd64-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efd64-132">响应</span><span class="sxs-lookup"><span data-stu-id="efd64-132">Response</span></span>
<span data-ttu-id="efd64-133">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 **deviceAndAppManagementAssignedRoleId** 。</span><span class="sxs-lookup"><span data-stu-id="efd64-133">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd64-134">示例</span><span class="sxs-lookup"><span data-stu-id="efd64-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="efd64-135">请求</span><span class="sxs-lookup"><span data-stu-id="efd64-135">Request</span></span>
<span data-ttu-id="efd64-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efd64-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="efd64-137">响应</span><span class="sxs-lookup"><span data-stu-id="efd64-137">Response</span></span>
<span data-ttu-id="efd64-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efd64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds",
    "roleDefinitionIds": [
      "df52f163-f163-df52-63f1-52df63f152df"
    ],
    "roleAssignmentIds": [
      "1f35d53d-d53d-1f35-3dd5-351f3dd5351f"
    ]
  }
}
```













