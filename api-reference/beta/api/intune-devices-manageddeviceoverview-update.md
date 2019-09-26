---
title: 更新 managedDeviceOverview
description: 更新 managedDeviceOverview 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a5048e5c01e22d9c0922f9620916c3bc4251b07
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188281"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="95ea3-103">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="95ea3-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="95ea3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95ea3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95ea3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95ea3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95ea3-106">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95ea3-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95ea3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95ea3-107">Prerequisites</span></span>
<span data-ttu-id="95ea3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95ea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95ea3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95ea3-110">Permission type</span></span>|<span data-ttu-id="95ea3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95ea3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95ea3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95ea3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95ea3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95ea3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="95ea3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95ea3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95ea3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95ea3-115">Not supported.</span></span>|
|<span data-ttu-id="95ea3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95ea3-116">Application</span></span>|<span data-ttu-id="95ea3-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95ea3-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95ea3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95ea3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="95ea3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95ea3-119">Request headers</span></span>
|<span data-ttu-id="95ea3-120">标头</span><span class="sxs-lookup"><span data-stu-id="95ea3-120">Header</span></span>|<span data-ttu-id="95ea3-121">值</span><span class="sxs-lookup"><span data-stu-id="95ea3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95ea3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95ea3-122">Authorization</span></span>|<span data-ttu-id="95ea3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95ea3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95ea3-124">接受</span><span class="sxs-lookup"><span data-stu-id="95ea3-124">Accept</span></span>|<span data-ttu-id="95ea3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95ea3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95ea3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95ea3-126">Request body</span></span>
<span data-ttu-id="95ea3-127">在请求正文中，提供 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95ea3-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="95ea3-128">下表显示创建 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95ea3-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="95ea3-129">属性</span><span class="sxs-lookup"><span data-stu-id="95ea3-129">Property</span></span>|<span data-ttu-id="95ea3-130">类型</span><span class="sxs-lookup"><span data-stu-id="95ea3-130">Type</span></span>|<span data-ttu-id="95ea3-131">说明</span><span class="sxs-lookup"><span data-stu-id="95ea3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95ea3-132">id</span><span class="sxs-lookup"><span data-stu-id="95ea3-132">id</span></span>|<span data-ttu-id="95ea3-133">String</span><span class="sxs-lookup"><span data-stu-id="95ea3-133">String</span></span>|<span data-ttu-id="95ea3-134">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="95ea3-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="95ea3-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="95ea3-135">enrolledDeviceCount</span></span>|<span data-ttu-id="95ea3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="95ea3-136">Int32</span></span>|<span data-ttu-id="95ea3-137">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="95ea3-137">Total enrolled device count.</span></span> <span data-ttu-id="95ea3-138">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="95ea3-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="95ea3-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="95ea3-139">mdmEnrolledCount</span></span>|<span data-ttu-id="95ea3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="95ea3-140">Int32</span></span>|<span data-ttu-id="95ea3-141">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="95ea3-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="95ea3-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="95ea3-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="95ea3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="95ea3-143">Int32</span></span>|<span data-ttu-id="95ea3-144">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="95ea3-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="95ea3-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="95ea3-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="95ea3-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="95ea3-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="95ea3-147">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="95ea3-147">Device operating system summary.</span></span>|
|<span data-ttu-id="95ea3-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="95ea3-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="95ea3-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="95ea3-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="95ea3-150">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="95ea3-150">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="95ea3-151">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="95ea3-151">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="95ea3-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="95ea3-152">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="95ea3-153">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="95ea3-153">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="95ea3-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95ea3-154">lastModifiedDateTime</span></span>|<span data-ttu-id="95ea3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95ea3-155">DateTimeOffset</span></span>|<span data-ttu-id="95ea3-156">设备的上次修改日期时间概述</span><span class="sxs-lookup"><span data-stu-id="95ea3-156">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="95ea3-157">响应</span><span class="sxs-lookup"><span data-stu-id="95ea3-157">Response</span></span>
<span data-ttu-id="95ea3-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95ea3-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95ea3-159">示例</span><span class="sxs-lookup"><span data-stu-id="95ea3-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="95ea3-160">请求</span><span class="sxs-lookup"><span data-stu-id="95ea3-160">Request</span></span>
<span data-ttu-id="95ea3-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95ea3-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 943

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="95ea3-162">响应</span><span class="sxs-lookup"><span data-stu-id="95ea3-162">Response</span></span>
<span data-ttu-id="95ea3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95ea3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1056

{
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
```




