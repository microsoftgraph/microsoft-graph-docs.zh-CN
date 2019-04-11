---
title: getRelatedAppStates 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 575a1d7c33801f474a23451cac900d612dc5bf65
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809172"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="d0471-103">getRelatedAppStates 函数</span><span class="sxs-lookup"><span data-stu-id="d0471-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="d0471-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0471-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0471-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0471-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0471-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0471-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0471-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0471-107">Prerequisites</span></span>
<span data-ttu-id="d0471-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0471-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0471-110">Permission type</span></span>|<span data-ttu-id="d0471-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0471-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0471-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0471-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0471-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0471-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d0471-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0471-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0471-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0471-115">Not supported.</span></span>|
|<span data-ttu-id="d0471-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0471-116">Application</span></span>|<span data-ttu-id="d0471-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0471-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0471-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0471-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="d0471-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0471-119">Request headers</span></span>
|<span data-ttu-id="d0471-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0471-120">Header</span></span>|<span data-ttu-id="d0471-121">值</span><span class="sxs-lookup"><span data-stu-id="d0471-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0471-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0471-122">Authorization</span></span>|<span data-ttu-id="d0471-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0471-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0471-124">接受</span><span class="sxs-lookup"><span data-stu-id="d0471-124">Accept</span></span>|<span data-ttu-id="d0471-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0471-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0471-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0471-126">Request body</span></span>
<span data-ttu-id="d0471-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="d0471-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d0471-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d0471-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d0471-129">属性</span><span class="sxs-lookup"><span data-stu-id="d0471-129">Property</span></span>|<span data-ttu-id="d0471-130">类型</span><span class="sxs-lookup"><span data-stu-id="d0471-130">Type</span></span>|<span data-ttu-id="d0471-131">说明</span><span class="sxs-lookup"><span data-stu-id="d0471-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0471-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0471-132">userPrincipalName</span></span>|<span data-ttu-id="d0471-133">String</span><span class="sxs-lookup"><span data-stu-id="d0471-133">String</span></span>|<span data-ttu-id="d0471-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0471-134">Not yet documented</span></span>|
|<span data-ttu-id="d0471-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="d0471-135">deviceId</span></span>|<span data-ttu-id="d0471-136">String</span><span class="sxs-lookup"><span data-stu-id="d0471-136">String</span></span>|<span data-ttu-id="d0471-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0471-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d0471-138">响应</span><span class="sxs-lookup"><span data-stu-id="d0471-138">Response</span></span>
<span data-ttu-id="d0471-139">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)集合。</span><span class="sxs-lookup"><span data-stu-id="d0471-139">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0471-140">示例</span><span class="sxs-lookup"><span data-stu-id="d0471-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0471-141">请求</span><span class="sxs-lookup"><span data-stu-id="d0471-141">Request</span></span>
<span data-ttu-id="d0471-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0471-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d0471-143">响应</span><span class="sxs-lookup"><span data-stu-id="d0471-143">Response</span></span>
<span data-ttu-id="d0471-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0471-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 481

{
  "value": [
    {
      "@odata.type": "microsoft.graph.mobileAppRelationshipState",
      "sourceIds": [
        "Source Ids value"
      ],
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "deviceId": "Device Id value",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "targetLastSyncDateTime": "2017-01-01T00:02:09.7809949-08:00"
    }
  ]
}
```





