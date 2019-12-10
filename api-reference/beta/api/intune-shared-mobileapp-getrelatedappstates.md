---
title: getRelatedAppStates 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87a732572ac2f4bc1d6a5f412dfff1d69552d1f2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939702"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="cd9e1-103">getRelatedAppStates 函数</span><span class="sxs-lookup"><span data-stu-id="cd9e1-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="cd9e1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd9e1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd9e1-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd9e1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd9e1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd9e1-107">Prerequisites</span></span>
<span data-ttu-id="cd9e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd9e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd9e1-110">Permission type</span></span>|<span data-ttu-id="cd9e1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd9e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd9e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd9e1-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cd9e1-113">&nbsp;&nbsp; **应用程序）**</span><span class="sxs-lookup"><span data-stu-id="cd9e1-113">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="cd9e1-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd9e1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cd9e1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd9e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd9e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-116">Not supported.</span></span>|
|<span data-ttu-id="cd9e1-117">Application</span><span class="sxs-lookup"><span data-stu-id="cd9e1-117">Application</span></span>||
| <span data-ttu-id="cd9e1-118">&nbsp;&nbsp; **应用程序）**</span><span class="sxs-lookup"><span data-stu-id="cd9e1-118">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="cd9e1-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd9e1-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd9e1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd9e1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="cd9e1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd9e1-121">Request headers</span></span>
|<span data-ttu-id="cd9e1-122">标头</span><span class="sxs-lookup"><span data-stu-id="cd9e1-122">Header</span></span>|<span data-ttu-id="cd9e1-123">值</span><span class="sxs-lookup"><span data-stu-id="cd9e1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd9e1-124">授权</span><span class="sxs-lookup"><span data-stu-id="cd9e1-124">Authorization</span></span>|<span data-ttu-id="cd9e1-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd9e1-126">接受</span><span class="sxs-lookup"><span data-stu-id="cd9e1-126">Accept</span></span>|<span data-ttu-id="cd9e1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9e1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd9e1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd9e1-128">Request body</span></span>
<span data-ttu-id="cd9e1-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cd9e1-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cd9e1-131">属性</span><span class="sxs-lookup"><span data-stu-id="cd9e1-131">Property</span></span>|<span data-ttu-id="cd9e1-132">类型</span><span class="sxs-lookup"><span data-stu-id="cd9e1-132">Type</span></span>|<span data-ttu-id="cd9e1-133">说明</span><span class="sxs-lookup"><span data-stu-id="cd9e1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9e1-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cd9e1-134">userPrincipalName</span></span>|<span data-ttu-id="cd9e1-135">字符串</span><span class="sxs-lookup"><span data-stu-id="cd9e1-135">String</span></span>|<span data-ttu-id="cd9e1-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd9e1-136">Not yet documented</span></span>|
|<span data-ttu-id="cd9e1-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="cd9e1-137">deviceId</span></span>|<span data-ttu-id="cd9e1-138">String</span><span class="sxs-lookup"><span data-stu-id="cd9e1-138">String</span></span>|<span data-ttu-id="cd9e1-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cd9e1-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd9e1-140">响应</span><span class="sxs-lookup"><span data-stu-id="cd9e1-140">Response</span></span>
<span data-ttu-id="cd9e1-141">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)集合。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-141">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9e1-142">示例</span><span class="sxs-lookup"><span data-stu-id="cd9e1-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd9e1-143">请求</span><span class="sxs-lookup"><span data-stu-id="cd9e1-143">Request</span></span>
<span data-ttu-id="cd9e1-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-144">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cd9e1-145">响应</span><span class="sxs-lookup"><span data-stu-id="cd9e1-145">Response</span></span>
<span data-ttu-id="cd9e1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd9e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








