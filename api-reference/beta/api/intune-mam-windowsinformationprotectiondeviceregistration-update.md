---
title: 更新 windowsInformationProtectionDeviceRegistration
description: 更新 windowsInformationProtectionDeviceRegistration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 382cd6016b71c29ea9187d534800a4d7575b92b2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191440"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="c1217-103">更新 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="c1217-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="c1217-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1217-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1217-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1217-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1217-106">更新[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1217-106">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1217-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1217-107">Prerequisites</span></span>
<span data-ttu-id="c1217-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1217-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1217-110">Permission type</span></span>|<span data-ttu-id="c1217-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1217-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1217-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1217-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1217-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1217-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1217-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1217-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1217-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1217-115">Not supported.</span></span>|
|<span data-ttu-id="c1217-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1217-116">Application</span></span>|<span data-ttu-id="c1217-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1217-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1217-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1217-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1217-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1217-119">Request headers</span></span>
|<span data-ttu-id="c1217-120">标头</span><span class="sxs-lookup"><span data-stu-id="c1217-120">Header</span></span>|<span data-ttu-id="c1217-121">值</span><span class="sxs-lookup"><span data-stu-id="c1217-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1217-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1217-122">Authorization</span></span>|<span data-ttu-id="c1217-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1217-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1217-124">接受</span><span class="sxs-lookup"><span data-stu-id="c1217-124">Accept</span></span>|<span data-ttu-id="c1217-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1217-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1217-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1217-126">Request body</span></span>
<span data-ttu-id="c1217-127">在请求正文中，提供[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1217-127">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="c1217-128">下表显示创建[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1217-128">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="c1217-129">属性</span><span class="sxs-lookup"><span data-stu-id="c1217-129">Property</span></span>|<span data-ttu-id="c1217-130">类型</span><span class="sxs-lookup"><span data-stu-id="c1217-130">Type</span></span>|<span data-ttu-id="c1217-131">说明</span><span class="sxs-lookup"><span data-stu-id="c1217-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1217-132">id</span><span class="sxs-lookup"><span data-stu-id="c1217-132">id</span></span>|<span data-ttu-id="c1217-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c1217-133">String</span></span>|<span data-ttu-id="c1217-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c1217-134">Key of the entity.</span></span>|
|<span data-ttu-id="c1217-135">userId</span><span class="sxs-lookup"><span data-stu-id="c1217-135">userId</span></span>|<span data-ttu-id="c1217-136">String</span><span class="sxs-lookup"><span data-stu-id="c1217-136">String</span></span>|<span data-ttu-id="c1217-137">与此设备注册记录相关联的 UserId。</span><span class="sxs-lookup"><span data-stu-id="c1217-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="c1217-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c1217-138">deviceRegistrationId</span></span>|<span data-ttu-id="c1217-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c1217-139">String</span></span>|<span data-ttu-id="c1217-140">此设备注册记录的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="c1217-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="c1217-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="c1217-141">deviceName</span></span>|<span data-ttu-id="c1217-142">String</span><span class="sxs-lookup"><span data-stu-id="c1217-142">String</span></span>|<span data-ttu-id="c1217-143">设备名称。</span><span class="sxs-lookup"><span data-stu-id="c1217-143">Device name.</span></span>|
|<span data-ttu-id="c1217-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="c1217-144">deviceType</span></span>|<span data-ttu-id="c1217-145">String</span><span class="sxs-lookup"><span data-stu-id="c1217-145">String</span></span>|<span data-ttu-id="c1217-146">设备类型，例如，Windows 便携式计算机 VS Windows phone。</span><span class="sxs-lookup"><span data-stu-id="c1217-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="c1217-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="c1217-147">deviceMacAddress</span></span>|<span data-ttu-id="c1217-148">String</span><span class="sxs-lookup"><span data-stu-id="c1217-148">String</span></span>|<span data-ttu-id="c1217-149">设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="c1217-149">Device Mac address.</span></span>|
|<span data-ttu-id="c1217-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="c1217-150">lastCheckInDateTime</span></span>|<span data-ttu-id="c1217-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1217-151">DateTimeOffset</span></span>|<span data-ttu-id="c1217-152">设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="c1217-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="c1217-153">响应</span><span class="sxs-lookup"><span data-stu-id="c1217-153">Response</span></span>
<span data-ttu-id="c1217-154">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1217-154">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1217-155">示例</span><span class="sxs-lookup"><span data-stu-id="c1217-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1217-156">请求</span><span class="sxs-lookup"><span data-stu-id="c1217-156">Request</span></span>
<span data-ttu-id="c1217-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1217-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
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

### <a name="response"></a><span data-ttu-id="c1217-158">响应</span><span class="sxs-lookup"><span data-stu-id="c1217-158">Response</span></span>
<span data-ttu-id="c1217-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1217-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




