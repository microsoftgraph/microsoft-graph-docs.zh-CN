---
title: 获取 managedDeviceOverview
description: 读取 managedDeviceOverview 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35b91b36bfaf190a69c8f4d78d717e5c71cb312a
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122705"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="ae10f-103">获取 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ae10f-103">Get managedDeviceOverview</span></span>

<span data-ttu-id="ae10f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae10f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae10f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae10f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae10f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae10f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae10f-107">读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae10f-107">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae10f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ae10f-108">Prerequisites</span></span>
<span data-ttu-id="ae10f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ae10f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ae10f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae10f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae10f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae10f-111">Permission type</span></span>|<span data-ttu-id="ae10f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ae10f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae10f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae10f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae10f-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae10f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ae10f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae10f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae10f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae10f-116">Not supported.</span></span>|
|<span data-ttu-id="ae10f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae10f-117">Application</span></span>|<span data-ttu-id="ae10f-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae10f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae10f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae10f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae10f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae10f-120">Optional query parameters</span></span>
<span data-ttu-id="ae10f-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae10f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae10f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae10f-122">Request headers</span></span>
|<span data-ttu-id="ae10f-123">标头</span><span class="sxs-lookup"><span data-stu-id="ae10f-123">Header</span></span>|<span data-ttu-id="ae10f-124">值</span><span class="sxs-lookup"><span data-stu-id="ae10f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae10f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae10f-125">Authorization</span></span>|<span data-ttu-id="ae10f-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ae10f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae10f-127">接受</span><span class="sxs-lookup"><span data-stu-id="ae10f-127">Accept</span></span>|<span data-ttu-id="ae10f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ae10f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae10f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae10f-129">Request body</span></span>
<span data-ttu-id="ae10f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae10f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae10f-131">响应</span><span class="sxs-lookup"><span data-stu-id="ae10f-131">Response</span></span>
<span data-ttu-id="ae10f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae10f-132">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae10f-133">示例</span><span class="sxs-lookup"><span data-stu-id="ae10f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae10f-134">请求</span><span class="sxs-lookup"><span data-stu-id="ae10f-134">Request</span></span>
<span data-ttu-id="ae10f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae10f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="ae10f-136">响应</span><span class="sxs-lookup"><span data-stu-id="ae10f-136">Response</span></span>
<span data-ttu-id="ae10f-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ae10f-137">Here is an example of the response.</span></span> <span data-ttu-id="ae10f-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ae10f-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ae10f-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ae10f-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1366

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
      "unknownCount": 12,
      "androidDedicatedCount": 5,
      "androidDeviceAdminCount": 7,
      "androidFullyManagedCount": 8,
      "androidWorkProfileCount": 7,
      "androidCorporateWorkProfileCount": 0,
      "configMgrDeviceCount": 4
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    },
    "managedDeviceModelsAndManufacturers": {
      "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
      "deviceModels": [
        "Device Models value"
      ],
      "deviceManufacturers": [
        "Device Manufacturers value"
      ]
    },
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```



