---
title: 更新 managedDeviceOverview
description: 更新 managedDeviceOverview 对象的属性。
ms.openlocfilehash: 31a061a5c75e312901d642071255716272dfe564
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044980"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="f2269-103">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f2269-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="f2269-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f2269-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2269-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2269-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2269-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2269-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2269-107">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2269-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2269-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2269-108">Prerequisites</span></span>
<span data-ttu-id="f2269-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f2269-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2269-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2269-111">Permission type</span></span>|<span data-ttu-id="f2269-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2269-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2269-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2269-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2269-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2269-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f2269-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2269-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2269-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2269-116">Not supported.</span></span>|
|<span data-ttu-id="f2269-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2269-117">Application</span></span>|<span data-ttu-id="f2269-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2269-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2269-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2269-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="f2269-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2269-120">Request headers</span></span>
|<span data-ttu-id="f2269-121">标头</span><span class="sxs-lookup"><span data-stu-id="f2269-121">Header</span></span>|<span data-ttu-id="f2269-122">值</span><span class="sxs-lookup"><span data-stu-id="f2269-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2269-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2269-123">Authorization</span></span>|<span data-ttu-id="f2269-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2269-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2269-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2269-125">Accept</span></span>|<span data-ttu-id="f2269-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2269-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2269-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2269-127">Request body</span></span>
<span data-ttu-id="f2269-128">在请求正文中，提供 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2269-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="f2269-129">下表显示创建 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2269-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="f2269-130">属性</span><span class="sxs-lookup"><span data-stu-id="f2269-130">Property</span></span>|<span data-ttu-id="f2269-131">类型</span><span class="sxs-lookup"><span data-stu-id="f2269-131">Type</span></span>|<span data-ttu-id="f2269-132">说明</span><span class="sxs-lookup"><span data-stu-id="f2269-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2269-133">id</span><span class="sxs-lookup"><span data-stu-id="f2269-133">id</span></span>|<span data-ttu-id="f2269-134">String</span><span class="sxs-lookup"><span data-stu-id="f2269-134">String</span></span>|<span data-ttu-id="f2269-135">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f2269-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f2269-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2269-136">enrolledDeviceCount</span></span>|<span data-ttu-id="f2269-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f2269-137">Int32</span></span>|<span data-ttu-id="f2269-138">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="f2269-138">Total enrolled device count.</span></span> <span data-ttu-id="f2269-139">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="f2269-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f2269-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f2269-140">mdmEnrolledCount</span></span>|<span data-ttu-id="f2269-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f2269-141">Int32</span></span>|<span data-ttu-id="f2269-142">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="f2269-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f2269-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2269-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f2269-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f2269-144">Int32</span></span>|<span data-ttu-id="f2269-145">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="f2269-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f2269-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f2269-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f2269-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f2269-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f2269-148">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="f2269-148">Device operating system summary.</span></span>|
|<span data-ttu-id="f2269-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f2269-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f2269-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f2269-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f2269-151">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="f2269-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="f2269-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f2269-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="f2269-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f2269-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="f2269-154">模型和托管帐户中的设备的制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="f2269-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="f2269-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2269-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f2269-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2269-156">DateTimeOffset</span></span>|<span data-ttu-id="f2269-157">上次修改的日期时间的设备概述 （英文）</span><span class="sxs-lookup"><span data-stu-id="f2269-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="f2269-158">响应</span><span class="sxs-lookup"><span data-stu-id="f2269-158">Response</span></span>
<span data-ttu-id="f2269-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2269-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2269-160">示例</span><span class="sxs-lookup"><span data-stu-id="f2269-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2269-161">请求</span><span class="sxs-lookup"><span data-stu-id="f2269-161">Request</span></span>
<span data-ttu-id="f2269-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2269-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 947

{
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

### <a name="response"></a><span data-ttu-id="f2269-163">响应</span><span class="sxs-lookup"><span data-stu-id="f2269-163">Response</span></span>
<span data-ttu-id="f2269-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2269-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





