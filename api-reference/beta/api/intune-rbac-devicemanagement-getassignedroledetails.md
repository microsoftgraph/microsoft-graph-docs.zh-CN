---
title: getAssignedRoleDetails 函数
description: 检索当前已通过身份验证的用户分配的角色定义和角色分配。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 225921eac6fefc68e8f697d45fa8ae751fc74221
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189569"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="208d5-103">getAssignedRoleDetails 函数</span><span class="sxs-lookup"><span data-stu-id="208d5-103">getAssignedRoleDetails function</span></span>

> <span data-ttu-id="208d5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="208d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="208d5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="208d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="208d5-106">检索当前已通过身份验证的用户分配的角色定义和角色分配。</span><span class="sxs-lookup"><span data-stu-id="208d5-106">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="208d5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="208d5-107">Prerequisites</span></span>
<span data-ttu-id="208d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="208d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="208d5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="208d5-110">Permission type</span></span>|<span data-ttu-id="208d5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="208d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="208d5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="208d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="208d5-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="208d5-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="208d5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="208d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="208d5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="208d5-115">Not supported.</span></span>|
|<span data-ttu-id="208d5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="208d5-116">Application</span></span>|<span data-ttu-id="208d5-117">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="208d5-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="208d5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="208d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="208d5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="208d5-119">Request headers</span></span>
|<span data-ttu-id="208d5-120">标头</span><span class="sxs-lookup"><span data-stu-id="208d5-120">Header</span></span>|<span data-ttu-id="208d5-121">值</span><span class="sxs-lookup"><span data-stu-id="208d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="208d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="208d5-122">Authorization</span></span>|<span data-ttu-id="208d5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="208d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="208d5-124">接受</span><span class="sxs-lookup"><span data-stu-id="208d5-124">Accept</span></span>|<span data-ttu-id="208d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="208d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="208d5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="208d5-126">Request body</span></span>
<span data-ttu-id="208d5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="208d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="208d5-128">响应</span><span class="sxs-lookup"><span data-stu-id="208d5-128">Response</span></span>
<span data-ttu-id="208d5-129">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) 。</span><span class="sxs-lookup"><span data-stu-id="208d5-129">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="208d5-130">示例</span><span class="sxs-lookup"><span data-stu-id="208d5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="208d5-131">请求</span><span class="sxs-lookup"><span data-stu-id="208d5-131">Request</span></span>
<span data-ttu-id="208d5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="208d5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="208d5-133">响应</span><span class="sxs-lookup"><span data-stu-id="208d5-133">Response</span></span>
<span data-ttu-id="208d5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="208d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
    "roleDefinitionIds": [
      "Role Definition Ids value"
    ],
    "roleAssignmentIds": [
      "Role Assignment Ids value"
    ]
  }
}
```




