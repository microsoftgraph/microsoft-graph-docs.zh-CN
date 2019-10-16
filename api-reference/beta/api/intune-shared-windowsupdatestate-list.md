---
title: 列出 windowsUpdateStates
description: 列出 windowsUpdateState 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5c9a516165cdb82e8f26c2d40c1160c181dfe41
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536824"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="4a77d-103">列出 windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="4a77d-103">List windowsUpdateStates</span></span>

> <span data-ttu-id="4a77d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a77d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a77d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a77d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a77d-106">列出[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a77d-106">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a77d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a77d-107">Prerequisites</span></span>
<span data-ttu-id="4a77d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a77d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a77d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a77d-110">Permission type</span></span>|<span data-ttu-id="4a77d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a77d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a77d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a77d-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4a77d-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4a77d-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4a77d-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a77d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4a77d-115">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="4a77d-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4a77d-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a77d-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a77d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a77d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a77d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a77d-118">Not supported.</span></span>|
|<span data-ttu-id="4a77d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a77d-119">Application</span></span>||
| <span data-ttu-id="4a77d-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4a77d-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4a77d-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a77d-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4a77d-122">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="4a77d-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4a77d-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a77d-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a77d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a77d-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="4a77d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a77d-125">Request headers</span></span>
|<span data-ttu-id="4a77d-126">标头</span><span class="sxs-lookup"><span data-stu-id="4a77d-126">Header</span></span>|<span data-ttu-id="4a77d-127">值</span><span class="sxs-lookup"><span data-stu-id="4a77d-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a77d-128">授权</span><span class="sxs-lookup"><span data-stu-id="4a77d-128">Authorization</span></span>|<span data-ttu-id="4a77d-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a77d-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a77d-130">接受</span><span class="sxs-lookup"><span data-stu-id="4a77d-130">Accept</span></span>|<span data-ttu-id="4a77d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4a77d-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a77d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a77d-132">Request body</span></span>
<span data-ttu-id="4a77d-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a77d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a77d-134">响应</span><span class="sxs-lookup"><span data-stu-id="4a77d-134">Response</span></span>
<span data-ttu-id="4a77d-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a77d-135">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a77d-136">示例</span><span class="sxs-lookup"><span data-stu-id="4a77d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a77d-137">请求</span><span class="sxs-lookup"><span data-stu-id="4a77d-137">Request</span></span>
<span data-ttu-id="4a77d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a77d-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="4a77d-139">响应</span><span class="sxs-lookup"><span data-stu-id="4a77d-139">Response</span></span>
<span data-ttu-id="4a77d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a77d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateState",
      "id": "3d92af00-af00-3d92-00af-923d00af923d",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "status": "pendingInstallation",
      "qualityUpdateVersion": "Quality Update Version value",
      "featureUpdateVersion": "Feature Update Version value",
      "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  ]
}
```






