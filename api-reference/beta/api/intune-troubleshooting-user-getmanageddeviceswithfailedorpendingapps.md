---
title: getManagedDevicesWithFailedOrPendingApps 函数
description: 检索具有失败或挂起的应用程序的设备的列表
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 47b0f41dfd0430a4b6674a126c7d8cedc58ef400
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160897"
---
# <a name="getmanageddeviceswithfailedorpendingapps-function"></a><span data-ttu-id="3d794-103">getManagedDevicesWithFailedOrPendingApps 函数</span><span class="sxs-lookup"><span data-stu-id="3d794-103">getManagedDevicesWithFailedOrPendingApps function</span></span>

> <span data-ttu-id="3d794-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d794-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d794-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d794-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d794-106">检索具有失败或挂起的应用程序的设备的列表</span><span class="sxs-lookup"><span data-stu-id="3d794-106">Retrieves the list of devices with failed or pending apps</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d794-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d794-107">Prerequisites</span></span>
<span data-ttu-id="3d794-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d794-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d794-110">Permission type</span></span>|<span data-ttu-id="3d794-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d794-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d794-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d794-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d794-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d794-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3d794-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d794-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d794-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d794-115">Not supported.</span></span>|
|<span data-ttu-id="3d794-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d794-116">Application</span></span>|<span data-ttu-id="3d794-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d794-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d794-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d794-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

## <a name="request-headers"></a><span data-ttu-id="3d794-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d794-119">Request headers</span></span>
|<span data-ttu-id="3d794-120">标头</span><span class="sxs-lookup"><span data-stu-id="3d794-120">Header</span></span>|<span data-ttu-id="3d794-121">值</span><span class="sxs-lookup"><span data-stu-id="3d794-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d794-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d794-122">Authorization</span></span>|<span data-ttu-id="3d794-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d794-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d794-124">接受</span><span class="sxs-lookup"><span data-stu-id="3d794-124">Accept</span></span>|<span data-ttu-id="3d794-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d794-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d794-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d794-126">Request body</span></span>
<span data-ttu-id="3d794-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d794-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d794-128">响应</span><span class="sxs-lookup"><span data-stu-id="3d794-128">Response</span></span>
<span data-ttu-id="3d794-129">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md)集合。</span><span class="sxs-lookup"><span data-stu-id="3d794-129">If successful, this function returns a `200 OK` response code and a [managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d794-130">示例</span><span class="sxs-lookup"><span data-stu-id="3d794-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d794-131">请求</span><span class="sxs-lookup"><span data-stu-id="3d794-131">Request</span></span>
<span data-ttu-id="3d794-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d794-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

### <a name="response"></a><span data-ttu-id="3d794-133">响应</span><span class="sxs-lookup"><span data-stu-id="3d794-133">Response</span></span>
<span data-ttu-id="3d794-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d794-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 187

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState",
      "summarizedAppState": "success",
      "deviceId": "Device Id value"
    }
  ]
}
```





