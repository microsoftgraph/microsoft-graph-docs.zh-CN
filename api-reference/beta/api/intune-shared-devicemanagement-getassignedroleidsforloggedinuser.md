---
title: getAssignedRoleIdsForLoggedInUser 函数
description: 检索已分配的角色定义和角色分配的当前经过身份验证的用户。
author: tfitzmac
ms.openlocfilehash: 0e9cf6e45c0f7ce7e321d746d12648a598109df5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331092"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="cd74b-103">getAssignedRoleIdsForLoggedInUser 函数</span><span class="sxs-lookup"><span data-stu-id="cd74b-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="cd74b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cd74b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd74b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cd74b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd74b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cd74b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd74b-107">检索已分配的角色定义和角色分配的当前经过身份验证的用户。</span><span class="sxs-lookup"><span data-stu-id="cd74b-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd74b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd74b-108">Prerequisites</span></span>
<span data-ttu-id="cd74b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cd74b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd74b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd74b-111">Permission type</span></span>|<span data-ttu-id="cd74b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd74b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd74b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd74b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cd74b-114">&nbsp;&nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="cd74b-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="cd74b-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd74b-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="cd74b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd74b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd74b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd74b-117">Not supported.</span></span>|
|<span data-ttu-id="cd74b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd74b-118">Application</span></span>|<span data-ttu-id="cd74b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd74b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd74b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd74b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="cd74b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd74b-121">Request headers</span></span>
|<span data-ttu-id="cd74b-122">标头</span><span class="sxs-lookup"><span data-stu-id="cd74b-122">Header</span></span>|<span data-ttu-id="cd74b-123">值</span><span class="sxs-lookup"><span data-stu-id="cd74b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd74b-124">授权</span><span class="sxs-lookup"><span data-stu-id="cd74b-124">Authorization</span></span>|<span data-ttu-id="cd74b-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd74b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd74b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cd74b-126">Accept</span></span>|<span data-ttu-id="cd74b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cd74b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd74b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd74b-128">Request body</span></span>
<span data-ttu-id="cd74b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd74b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd74b-130">响应</span><span class="sxs-lookup"><span data-stu-id="cd74b-130">Response</span></span>
<span data-ttu-id="cd74b-131">如果成功，此函数返回`200 OK`响应代码和响应正文中[deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) 。</span><span class="sxs-lookup"><span data-stu-id="cd74b-131">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd74b-132">示例</span><span class="sxs-lookup"><span data-stu-id="cd74b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd74b-133">请求</span><span class="sxs-lookup"><span data-stu-id="cd74b-133">Request</span></span>
<span data-ttu-id="cd74b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd74b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="cd74b-135">响应</span><span class="sxs-lookup"><span data-stu-id="cd74b-135">Response</span></span>
<span data-ttu-id="cd74b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd74b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





