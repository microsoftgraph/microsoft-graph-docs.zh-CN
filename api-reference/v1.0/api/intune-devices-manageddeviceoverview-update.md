---
title: 更新 managedDeviceOverview
description: 更新 managedDeviceOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69ad6672c5a3bc8ac0bb605c95c207665523c5b4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752621"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="fa8fc-103">更新 managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa8fc-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="fa8fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa8fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa8fc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa8fc-106">更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa8fc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa8fc-107">Prerequisites</span></span>
<span data-ttu-id="fa8fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa8fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa8fc-110">Permission type</span></span>|<span data-ttu-id="fa8fc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa8fc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa8fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa8fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa8fc-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa8fc-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fa8fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa8fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa8fc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-115">Not supported.</span></span>|
|<span data-ttu-id="fa8fc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa8fc-116">Application</span></span>|<span data-ttu-id="fa8fc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa8fc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa8fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa8fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="fa8fc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa8fc-119">Request headers</span></span>
|<span data-ttu-id="fa8fc-120">标头</span><span class="sxs-lookup"><span data-stu-id="fa8fc-120">Header</span></span>|<span data-ttu-id="fa8fc-121">值</span><span class="sxs-lookup"><span data-stu-id="fa8fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa8fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa8fc-122">Authorization</span></span>|<span data-ttu-id="fa8fc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa8fc-124">接受</span><span class="sxs-lookup"><span data-stu-id="fa8fc-124">Accept</span></span>|<span data-ttu-id="fa8fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa8fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa8fc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa8fc-126">Request body</span></span>
<span data-ttu-id="fa8fc-127">在请求正文中，提供 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="fa8fc-128">下表显示创建 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="fa8fc-129">属性</span><span class="sxs-lookup"><span data-stu-id="fa8fc-129">Property</span></span>|<span data-ttu-id="fa8fc-130">类型</span><span class="sxs-lookup"><span data-stu-id="fa8fc-130">Type</span></span>|<span data-ttu-id="fa8fc-131">说明</span><span class="sxs-lookup"><span data-stu-id="fa8fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa8fc-132">id</span><span class="sxs-lookup"><span data-stu-id="fa8fc-132">id</span></span>|<span data-ttu-id="fa8fc-133">String</span><span class="sxs-lookup"><span data-stu-id="fa8fc-133">String</span></span>|<span data-ttu-id="fa8fc-134">摘要的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="fa8fc-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="fa8fc-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8fc-135">enrolledDeviceCount</span></span>|<span data-ttu-id="fa8fc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8fc-136">Int32</span></span>|<span data-ttu-id="fa8fc-137">总注册设备计数。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-137">Total enrolled device count.</span></span> <span data-ttu-id="fa8fc-138">不包括通过 Intune PC 代理管理的 PC 设备。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="fa8fc-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="fa8fc-139">mdmEnrolledCount</span></span>|<span data-ttu-id="fa8fc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8fc-140">Int32</span></span>|<span data-ttu-id="fa8fc-141">MDM 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="fa8fc-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="fa8fc-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa8fc-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="fa8fc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fa8fc-143">Int32</span></span>|<span data-ttu-id="fa8fc-144">MDM 和 EAS 中注册的设备数</span><span class="sxs-lookup"><span data-stu-id="fa8fc-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="fa8fc-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="fa8fc-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="fa8fc-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="fa8fc-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="fa8fc-147">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-147">Device operating system summary.</span></span>|
|<span data-ttu-id="fa8fc-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa8fc-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="fa8fc-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa8fc-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="fa8fc-150">Intune 中的 Exchange 访问状态的分配</span><span class="sxs-lookup"><span data-stu-id="fa8fc-150">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="fa8fc-151">响应</span><span class="sxs-lookup"><span data-stu-id="fa8fc-151">Response</span></span>
<span data-ttu-id="fa8fc-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa8fc-153">示例</span><span class="sxs-lookup"><span data-stu-id="fa8fc-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa8fc-154">请求</span><span class="sxs-lookup"><span data-stu-id="fa8fc-154">Request</span></span>
<span data-ttu-id="fa8fc-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa8fc-156">响应</span><span class="sxs-lookup"><span data-stu-id="fa8fc-156">Response</span></span>
<span data-ttu-id="fa8fc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa8fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




