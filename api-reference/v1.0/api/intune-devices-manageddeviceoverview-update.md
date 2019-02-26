---
title: 更新 managedDeviceOverview
description: 更新 managedDeviceOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e4b7acf2b03ee37bf9171bfe83164c25e993f5f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260576"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="fd63a-103">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fd63a-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="fd63a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd63a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd63a-105">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd63a-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd63a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd63a-106">Prerequisites</span></span>
<span data-ttu-id="fd63a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fd63a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd63a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd63a-109">Permission type</span></span>|<span data-ttu-id="fd63a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd63a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd63a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd63a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd63a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd63a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fd63a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd63a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd63a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd63a-114">Not supported.</span></span>|
|<span data-ttu-id="fd63a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd63a-115">Application</span></span>|<span data-ttu-id="fd63a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd63a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd63a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd63a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="fd63a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd63a-118">Request headers</span></span>
|<span data-ttu-id="fd63a-119">标头</span><span class="sxs-lookup"><span data-stu-id="fd63a-119">Header</span></span>|<span data-ttu-id="fd63a-120">值</span><span class="sxs-lookup"><span data-stu-id="fd63a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd63a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd63a-121">Authorization</span></span>|<span data-ttu-id="fd63a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd63a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd63a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fd63a-123">Accept</span></span>|<span data-ttu-id="fd63a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd63a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd63a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd63a-125">Request body</span></span>
<span data-ttu-id="fd63a-126">在请求正文中，提供 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd63a-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="fd63a-127">下表显示创建 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fd63a-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="fd63a-128">属性</span><span class="sxs-lookup"><span data-stu-id="fd63a-128">Property</span></span>|<span data-ttu-id="fd63a-129">类型</span><span class="sxs-lookup"><span data-stu-id="fd63a-129">Type</span></span>|<span data-ttu-id="fd63a-130">说明</span><span class="sxs-lookup"><span data-stu-id="fd63a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd63a-131">id</span><span class="sxs-lookup"><span data-stu-id="fd63a-131">id</span></span>|<span data-ttu-id="fd63a-132">String</span><span class="sxs-lookup"><span data-stu-id="fd63a-132">String</span></span>|<span data-ttu-id="fd63a-133">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="fd63a-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="fd63a-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fd63a-134">enrolledDeviceCount</span></span>|<span data-ttu-id="fd63a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="fd63a-135">Int32</span></span>|<span data-ttu-id="fd63a-136">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="fd63a-136">Total enrolled device count.</span></span> <span data-ttu-id="fd63a-137">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="fd63a-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="fd63a-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="fd63a-138">mdmEnrolledCount</span></span>|<span data-ttu-id="fd63a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fd63a-139">Int32</span></span>|<span data-ttu-id="fd63a-140">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="fd63a-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="fd63a-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fd63a-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="fd63a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fd63a-142">Int32</span></span>|<span data-ttu-id="fd63a-143">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="fd63a-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="fd63a-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="fd63a-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="fd63a-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="fd63a-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="fd63a-146">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="fd63a-146">Device operating system summary.</span></span>|
|<span data-ttu-id="fd63a-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fd63a-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="fd63a-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fd63a-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="fd63a-149">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="fd63a-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="fd63a-150">响应</span><span class="sxs-lookup"><span data-stu-id="fd63a-150">Response</span></span>
<span data-ttu-id="fd63a-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd63a-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd63a-152">示例</span><span class="sxs-lookup"><span data-stu-id="fd63a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd63a-153">请求</span><span class="sxs-lookup"><span data-stu-id="fd63a-153">Request</span></span>
<span data-ttu-id="fd63a-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd63a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 685

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
  }
}
```

### <a name="response"></a><span data-ttu-id="fd63a-155">响应</span><span class="sxs-lookup"><span data-stu-id="fd63a-155">Response</span></span>
<span data-ttu-id="fd63a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd63a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

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
  }
}
```



