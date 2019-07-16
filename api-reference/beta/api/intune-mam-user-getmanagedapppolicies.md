---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93161a696d572742d820074fcded9a537ea47ea1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725913"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="08c85-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="08c85-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="08c85-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08c85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08c85-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08c85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08c85-106">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="08c85-106">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08c85-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08c85-107">Prerequisites</span></span>
<span data-ttu-id="08c85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08c85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08c85-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08c85-110">Permission type</span></span>|<span data-ttu-id="08c85-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08c85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08c85-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08c85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08c85-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="08c85-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="08c85-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08c85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08c85-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c85-115">Not supported.</span></span>|
|<span data-ttu-id="08c85-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="08c85-116">Application</span></span>|<span data-ttu-id="08c85-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c85-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08c85-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08c85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="08c85-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="08c85-119">Request headers</span></span>
|<span data-ttu-id="08c85-120">标头</span><span class="sxs-lookup"><span data-stu-id="08c85-120">Header</span></span>|<span data-ttu-id="08c85-121">值</span><span class="sxs-lookup"><span data-stu-id="08c85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08c85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c85-122">Authorization</span></span>|<span data-ttu-id="08c85-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08c85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08c85-124">接受</span><span class="sxs-lookup"><span data-stu-id="08c85-124">Accept</span></span>|<span data-ttu-id="08c85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08c85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c85-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08c85-126">Request body</span></span>
<span data-ttu-id="08c85-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08c85-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08c85-128">响应</span><span class="sxs-lookup"><span data-stu-id="08c85-128">Response</span></span>
<span data-ttu-id="08c85-129">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="08c85-129">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08c85-130">示例</span><span class="sxs-lookup"><span data-stu-id="08c85-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="08c85-131">请求</span><span class="sxs-lookup"><span data-stu-id="08c85-131">Request</span></span>
<span data-ttu-id="08c85-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08c85-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="08c85-133">响应</span><span class="sxs-lookup"><span data-stu-id="08c85-133">Response</span></span>
<span data-ttu-id="08c85-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08c85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```





