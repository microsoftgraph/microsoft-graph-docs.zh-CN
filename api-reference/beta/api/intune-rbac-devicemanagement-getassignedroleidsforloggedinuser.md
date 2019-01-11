---
title: getAssignedRoleIdsForLoggedInUser 函数
description: 检索已分配的角色定义和角色分配的当前经过身份验证的用户。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3385d43eb8ee2680d5e2684ffc21690f627a5034
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823602"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="7c5bd-103">getAssignedRoleIdsForLoggedInUser 函数</span><span class="sxs-lookup"><span data-stu-id="7c5bd-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="7c5bd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c5bd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c5bd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c5bd-107">检索已分配的角色定义和角色分配的当前经过身份验证的用户。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c5bd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7c5bd-108">Prerequisites</span></span>
<span data-ttu-id="7c5bd-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7c5bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c5bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c5bd-111">Permission type</span></span>|<span data-ttu-id="7c5bd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7c5bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c5bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c5bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c5bd-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c5bd-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7c5bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c5bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c5bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-116">Not supported.</span></span>|
|<span data-ttu-id="7c5bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c5bd-117">Application</span></span>|<span data-ttu-id="7c5bd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c5bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c5bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="7c5bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c5bd-120">Request headers</span></span>
|<span data-ttu-id="7c5bd-121">标头</span><span class="sxs-lookup"><span data-stu-id="7c5bd-121">Header</span></span>|<span data-ttu-id="7c5bd-122">值</span><span class="sxs-lookup"><span data-stu-id="7c5bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c5bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c5bd-123">Authorization</span></span>|<span data-ttu-id="7c5bd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c5bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c5bd-125">Accept</span></span>|<span data-ttu-id="7c5bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c5bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c5bd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c5bd-127">Request body</span></span>
<span data-ttu-id="7c5bd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c5bd-129">响应</span><span class="sxs-lookup"><span data-stu-id="7c5bd-129">Response</span></span>
<span data-ttu-id="7c5bd-130">如果成功，此函数返回`200 OK`响应代码和响应正文中[deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) 。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-130">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c5bd-131">示例</span><span class="sxs-lookup"><span data-stu-id="7c5bd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c5bd-132">请求</span><span class="sxs-lookup"><span data-stu-id="7c5bd-132">Request</span></span>
<span data-ttu-id="7c5bd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="7c5bd-134">响应</span><span class="sxs-lookup"><span data-stu-id="7c5bd-134">Response</span></span>
<span data-ttu-id="7c5bd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c5bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





