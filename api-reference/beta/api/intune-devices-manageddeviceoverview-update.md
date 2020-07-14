---
title: 更新 managedDeviceOverview
description: 更新 managedDeviceOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e0034c22be5b8a33d2fe46e1115c2bed5a08958
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122712"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="b006a-103">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b006a-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="b006a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b006a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b006a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b006a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b006a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b006a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b006a-107">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b006a-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b006a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b006a-108">Prerequisites</span></span>
<span data-ttu-id="b006a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b006a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b006a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b006a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b006a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b006a-111">Permission type</span></span>|<span data-ttu-id="b006a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b006a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b006a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b006a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b006a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b006a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b006a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b006a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b006a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b006a-116">Not supported.</span></span>|
|<span data-ttu-id="b006a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b006a-117">Application</span></span>|<span data-ttu-id="b006a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b006a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b006a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b006a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="b006a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b006a-120">Request headers</span></span>
|<span data-ttu-id="b006a-121">标头</span><span class="sxs-lookup"><span data-stu-id="b006a-121">Header</span></span>|<span data-ttu-id="b006a-122">值</span><span class="sxs-lookup"><span data-stu-id="b006a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b006a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b006a-123">Authorization</span></span>|<span data-ttu-id="b006a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b006a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b006a-125">接受</span><span class="sxs-lookup"><span data-stu-id="b006a-125">Accept</span></span>|<span data-ttu-id="b006a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b006a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b006a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b006a-127">Request body</span></span>
<span data-ttu-id="b006a-128">在请求正文中，提供 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b006a-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="b006a-129">下表显示创建 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b006a-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="b006a-130">属性</span><span class="sxs-lookup"><span data-stu-id="b006a-130">Property</span></span>|<span data-ttu-id="b006a-131">类型</span><span class="sxs-lookup"><span data-stu-id="b006a-131">Type</span></span>|<span data-ttu-id="b006a-132">说明</span><span class="sxs-lookup"><span data-stu-id="b006a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b006a-133">id</span><span class="sxs-lookup"><span data-stu-id="b006a-133">id</span></span>|<span data-ttu-id="b006a-134">String</span><span class="sxs-lookup"><span data-stu-id="b006a-134">String</span></span>|<span data-ttu-id="b006a-135">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b006a-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b006a-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b006a-136">enrolledDeviceCount</span></span>|<span data-ttu-id="b006a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b006a-137">Int32</span></span>|<span data-ttu-id="b006a-138">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="b006a-138">Total enrolled device count.</span></span> <span data-ttu-id="b006a-139">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="b006a-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b006a-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b006a-140">mdmEnrolledCount</span></span>|<span data-ttu-id="b006a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b006a-141">Int32</span></span>|<span data-ttu-id="b006a-142">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="b006a-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b006a-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b006a-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b006a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b006a-144">Int32</span></span>|<span data-ttu-id="b006a-145">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="b006a-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b006a-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b006a-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b006a-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b006a-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b006a-148">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="b006a-148">Device operating system summary.</span></span>|
|<span data-ttu-id="b006a-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b006a-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b006a-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b006a-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b006a-151">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="b006a-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="b006a-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b006a-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="b006a-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b006a-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="b006a-154">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="b006a-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="b006a-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b006a-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b006a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b006a-156">DateTimeOffset</span></span>|<span data-ttu-id="b006a-157">设备的上次修改日期时间概述</span><span class="sxs-lookup"><span data-stu-id="b006a-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="b006a-158">响应</span><span class="sxs-lookup"><span data-stu-id="b006a-158">Response</span></span>
<span data-ttu-id="b006a-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b006a-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b006a-160">示例</span><span class="sxs-lookup"><span data-stu-id="b006a-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="b006a-161">请求</span><span class="sxs-lookup"><span data-stu-id="b006a-161">Request</span></span>
<span data-ttu-id="b006a-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b006a-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 1158

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
  }
}
```

### <a name="response"></a><span data-ttu-id="b006a-163">响应</span><span class="sxs-lookup"><span data-stu-id="b006a-163">Response</span></span>
<span data-ttu-id="b006a-164">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b006a-164">Here is an example of the response.</span></span> <span data-ttu-id="b006a-165">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b006a-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b006a-166">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b006a-166">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1271

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
```



