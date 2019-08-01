---
title: 获取 managedDeviceOverview
description: 读取 managedDeviceOverview 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27ed01c6b4a09b04c2688742008210b00451b203
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018559"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="a9956-103">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a9956-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="a9956-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9956-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9956-105">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9956-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9956-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9956-106">Prerequisites</span></span>
<span data-ttu-id="a9956-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9956-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9956-109">Permission type</span></span>|<span data-ttu-id="a9956-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9956-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9956-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9956-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9956-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9956-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a9956-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9956-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9956-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9956-114">Not supported.</span></span>|
|<span data-ttu-id="a9956-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9956-115">Application</span></span>|<span data-ttu-id="a9956-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9956-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9956-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9956-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9956-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a9956-118">Optional query parameters</span></span>
<span data-ttu-id="a9956-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a9956-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9956-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9956-120">Request headers</span></span>
|<span data-ttu-id="a9956-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9956-121">Header</span></span>|<span data-ttu-id="a9956-122">值</span><span class="sxs-lookup"><span data-stu-id="a9956-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9956-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9956-123">Authorization</span></span>|<span data-ttu-id="a9956-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9956-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9956-125">接受</span><span class="sxs-lookup"><span data-stu-id="a9956-125">Accept</span></span>|<span data-ttu-id="a9956-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9956-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9956-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9956-127">Request body</span></span>
<span data-ttu-id="a9956-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9956-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9956-129">响应</span><span class="sxs-lookup"><span data-stu-id="a9956-129">Response</span></span>
<span data-ttu-id="a9956-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9956-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9956-131">示例</span><span class="sxs-lookup"><span data-stu-id="a9956-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9956-132">请求</span><span class="sxs-lookup"><span data-stu-id="a9956-132">Request</span></span>
<span data-ttu-id="a9956-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9956-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="a9956-134">响应</span><span class="sxs-lookup"><span data-stu-id="a9956-134">Response</span></span>
<span data-ttu-id="a9956-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9956-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    }
  }
}
```



