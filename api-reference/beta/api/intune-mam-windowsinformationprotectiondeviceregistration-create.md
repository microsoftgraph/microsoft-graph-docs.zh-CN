---
title: 创建 windowsInformationProtectionDeviceRegistration
description: 创建新的 windowsInformationProtectionDeviceRegistration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b2e6131a1d4393026ebf88a7ed089ebba2390b2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158840"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="3fb1c-103">创建 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="3fb1c-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="3fb1c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fb1c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fb1c-106">创建新的[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-106">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fb1c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3fb1c-107">Prerequisites</span></span>
<span data-ttu-id="3fb1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fb1c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fb1c-110">Permission type</span></span>|<span data-ttu-id="3fb1c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3fb1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb1c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fb1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb1c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fb1c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3fb1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fb1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb1c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-115">Not supported.</span></span>|
|<span data-ttu-id="3fb1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fb1c-116">Application</span></span>|<span data-ttu-id="3fb1c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb1c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fb1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="3fb1c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fb1c-119">Request headers</span></span>
|<span data-ttu-id="3fb1c-120">标头</span><span class="sxs-lookup"><span data-stu-id="3fb1c-120">Header</span></span>|<span data-ttu-id="3fb1c-121">值</span><span class="sxs-lookup"><span data-stu-id="3fb1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fb1c-122">Authorization</span></span>|<span data-ttu-id="3fb1c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3fb1c-124">Accept</span></span>|<span data-ttu-id="3fb1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb1c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fb1c-126">Request body</span></span>
<span data-ttu-id="3fb1c-127">在请求正文中, 提供 windowsInformationProtectionDeviceRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-127">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="3fb1c-128">下表显示创建 windowsInformationProtectionDeviceRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-128">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="3fb1c-129">属性</span><span class="sxs-lookup"><span data-stu-id="3fb1c-129">Property</span></span>|<span data-ttu-id="3fb1c-130">类型</span><span class="sxs-lookup"><span data-stu-id="3fb1c-130">Type</span></span>|<span data-ttu-id="3fb1c-131">说明</span><span class="sxs-lookup"><span data-stu-id="3fb1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb1c-132">id</span><span class="sxs-lookup"><span data-stu-id="3fb1c-132">id</span></span>|<span data-ttu-id="3fb1c-133">String</span><span class="sxs-lookup"><span data-stu-id="3fb1c-133">String</span></span>|<span data-ttu-id="3fb1c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-134">Key of the entity.</span></span>|
|<span data-ttu-id="3fb1c-135">userId</span><span class="sxs-lookup"><span data-stu-id="3fb1c-135">userId</span></span>|<span data-ttu-id="3fb1c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3fb1c-136">String</span></span>|<span data-ttu-id="3fb1c-137">与此设备注册记录相关联的 UserId。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="3fb1c-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="3fb1c-138">deviceRegistrationId</span></span>|<span data-ttu-id="3fb1c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="3fb1c-139">String</span></span>|<span data-ttu-id="3fb1c-140">此设备注册记录的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="3fb1c-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="3fb1c-141">deviceName</span></span>|<span data-ttu-id="3fb1c-142">String</span><span class="sxs-lookup"><span data-stu-id="3fb1c-142">String</span></span>|<span data-ttu-id="3fb1c-143">设备名称。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-143">Device name.</span></span>|
|<span data-ttu-id="3fb1c-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="3fb1c-144">deviceType</span></span>|<span data-ttu-id="3fb1c-145">String</span><span class="sxs-lookup"><span data-stu-id="3fb1c-145">String</span></span>|<span data-ttu-id="3fb1c-146">设备类型, 例如, windows 便携式计算机 VS windows phone。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="3fb1c-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="3fb1c-147">deviceMacAddress</span></span>|<span data-ttu-id="3fb1c-148">字符串</span><span class="sxs-lookup"><span data-stu-id="3fb1c-148">String</span></span>|<span data-ttu-id="3fb1c-149">设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-149">Device Mac address.</span></span>|
|<span data-ttu-id="3fb1c-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="3fb1c-150">lastCheckInDateTime</span></span>|<span data-ttu-id="3fb1c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fb1c-151">DateTimeOffset</span></span>|<span data-ttu-id="3fb1c-152">设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="3fb1c-153">响应</span><span class="sxs-lookup"><span data-stu-id="3fb1c-153">Response</span></span>
<span data-ttu-id="3fb1c-154">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-154">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb1c-155">示例</span><span class="sxs-lookup"><span data-stu-id="3fb1c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fb1c-156">请求</span><span class="sxs-lookup"><span data-stu-id="3fb1c-156">Request</span></span>
<span data-ttu-id="3fb1c-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3fb1c-158">响应</span><span class="sxs-lookup"><span data-stu-id="3fb1c-158">Response</span></span>
<span data-ttu-id="3fb1c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3fb1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




