---
title: 创建 windowsInformationProtectionDeviceRegistration
description: 创建新的 windowsInformationProtectionDeviceRegistration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd4ebf62b1f43018db2e4d905188e4505e6c9d1d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353531"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="66f62-103">创建 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="66f62-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="66f62-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66f62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66f62-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66f62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66f62-106">创建新的[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66f62-106">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66f62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="66f62-107">Prerequisites</span></span>
<span data-ttu-id="66f62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66f62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66f62-110">Permission type</span></span>|<span data-ttu-id="66f62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66f62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66f62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66f62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66f62-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66f62-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66f62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66f62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66f62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66f62-115">Not supported.</span></span>|
|<span data-ttu-id="66f62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66f62-116">Application</span></span>|<span data-ttu-id="66f62-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66f62-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66f62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66f62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="66f62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="66f62-119">Request headers</span></span>
|<span data-ttu-id="66f62-120">标头</span><span class="sxs-lookup"><span data-stu-id="66f62-120">Header</span></span>|<span data-ttu-id="66f62-121">值</span><span class="sxs-lookup"><span data-stu-id="66f62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66f62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66f62-122">Authorization</span></span>|<span data-ttu-id="66f62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66f62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66f62-124">接受</span><span class="sxs-lookup"><span data-stu-id="66f62-124">Accept</span></span>|<span data-ttu-id="66f62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66f62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66f62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66f62-126">Request body</span></span>
<span data-ttu-id="66f62-127">在请求正文中, 提供 windowsInformationProtectionDeviceRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66f62-127">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="66f62-128">下表显示创建 windowsInformationProtectionDeviceRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66f62-128">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="66f62-129">属性</span><span class="sxs-lookup"><span data-stu-id="66f62-129">Property</span></span>|<span data-ttu-id="66f62-130">类型</span><span class="sxs-lookup"><span data-stu-id="66f62-130">Type</span></span>|<span data-ttu-id="66f62-131">说明</span><span class="sxs-lookup"><span data-stu-id="66f62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66f62-132">id</span><span class="sxs-lookup"><span data-stu-id="66f62-132">id</span></span>|<span data-ttu-id="66f62-133">字符串</span><span class="sxs-lookup"><span data-stu-id="66f62-133">String</span></span>|<span data-ttu-id="66f62-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66f62-134">Key of the entity.</span></span>|
|<span data-ttu-id="66f62-135">userId</span><span class="sxs-lookup"><span data-stu-id="66f62-135">userId</span></span>|<span data-ttu-id="66f62-136">String</span><span class="sxs-lookup"><span data-stu-id="66f62-136">String</span></span>|<span data-ttu-id="66f62-137">与此设备注册记录相关联的 UserId。</span><span class="sxs-lookup"><span data-stu-id="66f62-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="66f62-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="66f62-138">deviceRegistrationId</span></span>|<span data-ttu-id="66f62-139">字符串</span><span class="sxs-lookup"><span data-stu-id="66f62-139">String</span></span>|<span data-ttu-id="66f62-140">此设备注册记录的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="66f62-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="66f62-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="66f62-141">deviceName</span></span>|<span data-ttu-id="66f62-142">String</span><span class="sxs-lookup"><span data-stu-id="66f62-142">String</span></span>|<span data-ttu-id="66f62-143">设备名称。</span><span class="sxs-lookup"><span data-stu-id="66f62-143">Device name.</span></span>|
|<span data-ttu-id="66f62-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="66f62-144">deviceType</span></span>|<span data-ttu-id="66f62-145">String</span><span class="sxs-lookup"><span data-stu-id="66f62-145">String</span></span>|<span data-ttu-id="66f62-146">设备类型, 例如, Windows 便携式计算机 VS Windows phone。</span><span class="sxs-lookup"><span data-stu-id="66f62-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="66f62-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="66f62-147">deviceMacAddress</span></span>|<span data-ttu-id="66f62-148">String</span><span class="sxs-lookup"><span data-stu-id="66f62-148">String</span></span>|<span data-ttu-id="66f62-149">设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="66f62-149">Device Mac address.</span></span>|
|<span data-ttu-id="66f62-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="66f62-150">lastCheckInDateTime</span></span>|<span data-ttu-id="66f62-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66f62-151">DateTimeOffset</span></span>|<span data-ttu-id="66f62-152">设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="66f62-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="66f62-153">响应</span><span class="sxs-lookup"><span data-stu-id="66f62-153">Response</span></span>
<span data-ttu-id="66f62-154">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66f62-154">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66f62-155">示例</span><span class="sxs-lookup"><span data-stu-id="66f62-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="66f62-156">请求</span><span class="sxs-lookup"><span data-stu-id="66f62-156">Request</span></span>
<span data-ttu-id="66f62-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66f62-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66f62-158">响应</span><span class="sxs-lookup"><span data-stu-id="66f62-158">Response</span></span>
<span data-ttu-id="66f62-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66f62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






