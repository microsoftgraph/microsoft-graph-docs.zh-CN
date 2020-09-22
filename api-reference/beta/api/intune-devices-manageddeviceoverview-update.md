---
title: 更新 managedDeviceOverview
description: 更新 managedDeviceOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 160da271112fb6dc3efaaa510fb8e2a4873b9289
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072415"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="817de-103">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="817de-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="817de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="817de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="817de-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="817de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="817de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="817de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="817de-107">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="817de-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="817de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="817de-108">Prerequisites</span></span>
<span data-ttu-id="817de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="817de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="817de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="817de-111">Permission type</span></span>|<span data-ttu-id="817de-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="817de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="817de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="817de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="817de-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="817de-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="817de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="817de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="817de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="817de-116">Not supported.</span></span>|
|<span data-ttu-id="817de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="817de-117">Application</span></span>|<span data-ttu-id="817de-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="817de-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="817de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="817de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="817de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="817de-120">Request headers</span></span>
|<span data-ttu-id="817de-121">标头</span><span class="sxs-lookup"><span data-stu-id="817de-121">Header</span></span>|<span data-ttu-id="817de-122">值</span><span class="sxs-lookup"><span data-stu-id="817de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="817de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="817de-123">Authorization</span></span>|<span data-ttu-id="817de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="817de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="817de-125">接受</span><span class="sxs-lookup"><span data-stu-id="817de-125">Accept</span></span>|<span data-ttu-id="817de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="817de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="817de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="817de-127">Request body</span></span>
<span data-ttu-id="817de-128">在请求正文中，提供 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="817de-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="817de-129">下表显示创建 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="817de-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="817de-130">属性</span><span class="sxs-lookup"><span data-stu-id="817de-130">Property</span></span>|<span data-ttu-id="817de-131">类型</span><span class="sxs-lookup"><span data-stu-id="817de-131">Type</span></span>|<span data-ttu-id="817de-132">说明</span><span class="sxs-lookup"><span data-stu-id="817de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="817de-133">id</span><span class="sxs-lookup"><span data-stu-id="817de-133">id</span></span>|<span data-ttu-id="817de-134">String</span><span class="sxs-lookup"><span data-stu-id="817de-134">String</span></span>|<span data-ttu-id="817de-135">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="817de-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="817de-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817de-136">enrolledDeviceCount</span></span>|<span data-ttu-id="817de-137">Int32</span><span class="sxs-lookup"><span data-stu-id="817de-137">Int32</span></span>|<span data-ttu-id="817de-138">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="817de-138">Total enrolled device count.</span></span> <span data-ttu-id="817de-139">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="817de-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="817de-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="817de-140">mdmEnrolledCount</span></span>|<span data-ttu-id="817de-141">Int32</span><span class="sxs-lookup"><span data-stu-id="817de-141">Int32</span></span>|<span data-ttu-id="817de-142">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="817de-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="817de-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817de-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="817de-144">Int32</span><span class="sxs-lookup"><span data-stu-id="817de-144">Int32</span></span>|<span data-ttu-id="817de-145">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="817de-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="817de-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="817de-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="817de-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="817de-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="817de-148">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="817de-148">Device operating system summary.</span></span>|
|<span data-ttu-id="817de-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="817de-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="817de-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="817de-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="817de-151">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="817de-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="817de-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="817de-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="817de-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="817de-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="817de-154">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="817de-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="817de-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="817de-155">lastModifiedDateTime</span></span>|<span data-ttu-id="817de-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="817de-156">DateTimeOffset</span></span>|<span data-ttu-id="817de-157">设备的上次修改日期时间概述</span><span class="sxs-lookup"><span data-stu-id="817de-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="817de-158">响应</span><span class="sxs-lookup"><span data-stu-id="817de-158">Response</span></span>
<span data-ttu-id="817de-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="817de-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="817de-160">示例</span><span class="sxs-lookup"><span data-stu-id="817de-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="817de-161">请求</span><span class="sxs-lookup"><span data-stu-id="817de-161">Request</span></span>
<span data-ttu-id="817de-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="817de-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 1187

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
    "configMgrDeviceCount": 4,
    "aospUserlessCount": 1
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

### <a name="response"></a><span data-ttu-id="817de-163">响应</span><span class="sxs-lookup"><span data-stu-id="817de-163">Response</span></span>
<span data-ttu-id="817de-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="817de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1300

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
    "configMgrDeviceCount": 4,
    "aospUserlessCount": 1
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






