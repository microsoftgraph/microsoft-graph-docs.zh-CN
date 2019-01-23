---
title: 创建 windowsInformationProtectionDeviceRegistration
description: 创建新的 windowsInformationProtectionDeviceRegistration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea5e3bac32e0511b54e08cb37063084f359e554a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428858"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="316e4-103">创建 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="316e4-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="316e4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="316e4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="316e4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="316e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="316e4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="316e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="316e4-107">创建新的[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="316e4-107">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="316e4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="316e4-108">Prerequisites</span></span>
<span data-ttu-id="316e4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="316e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="316e4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="316e4-111">Permission type</span></span>|<span data-ttu-id="316e4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="316e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="316e4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="316e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="316e4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="316e4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="316e4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="316e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="316e4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="316e4-116">Not supported.</span></span>|
|<span data-ttu-id="316e4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="316e4-117">Application</span></span>|<span data-ttu-id="316e4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="316e4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="316e4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="316e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="316e4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="316e4-120">Request headers</span></span>
|<span data-ttu-id="316e4-121">标头</span><span class="sxs-lookup"><span data-stu-id="316e4-121">Header</span></span>|<span data-ttu-id="316e4-122">值</span><span class="sxs-lookup"><span data-stu-id="316e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="316e4-123">授权</span><span class="sxs-lookup"><span data-stu-id="316e4-123">Authorization</span></span>|<span data-ttu-id="316e4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="316e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="316e4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="316e4-125">Accept</span></span>|<span data-ttu-id="316e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="316e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="316e4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="316e4-127">Request body</span></span>
<span data-ttu-id="316e4-128">在请求正文中，提供 windowsInformationProtectionDeviceRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="316e4-128">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="316e4-129">下表显示时创建 windowsInformationProtectionDeviceRegistration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="316e4-129">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="316e4-130">属性</span><span class="sxs-lookup"><span data-stu-id="316e4-130">Property</span></span>|<span data-ttu-id="316e4-131">类型</span><span class="sxs-lookup"><span data-stu-id="316e4-131">Type</span></span>|<span data-ttu-id="316e4-132">说明</span><span class="sxs-lookup"><span data-stu-id="316e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="316e4-133">id</span><span class="sxs-lookup"><span data-stu-id="316e4-133">id</span></span>|<span data-ttu-id="316e4-134">String</span><span class="sxs-lookup"><span data-stu-id="316e4-134">String</span></span>|<span data-ttu-id="316e4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="316e4-135">Key of the entity.</span></span>|
|<span data-ttu-id="316e4-136">userId</span><span class="sxs-lookup"><span data-stu-id="316e4-136">userId</span></span>|<span data-ttu-id="316e4-137">String</span><span class="sxs-lookup"><span data-stu-id="316e4-137">String</span></span>|<span data-ttu-id="316e4-138">此设备注册记录相关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="316e4-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="316e4-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="316e4-139">deviceRegistrationId</span></span>|<span data-ttu-id="316e4-140">字符串</span><span class="sxs-lookup"><span data-stu-id="316e4-140">String</span></span>|<span data-ttu-id="316e4-141">此设备注册记录的的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="316e4-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="316e4-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="316e4-142">deviceName</span></span>|<span data-ttu-id="316e4-143">String</span><span class="sxs-lookup"><span data-stu-id="316e4-143">String</span></span>|<span data-ttu-id="316e4-144">设备名称。</span><span class="sxs-lookup"><span data-stu-id="316e4-144">Device name.</span></span>|
|<span data-ttu-id="316e4-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="316e4-145">deviceType</span></span>|<span data-ttu-id="316e4-146">String</span><span class="sxs-lookup"><span data-stu-id="316e4-146">String</span></span>|<span data-ttu-id="316e4-147">设备类型，例如 Windows 便携式计算机 VS Windows phone。</span><span class="sxs-lookup"><span data-stu-id="316e4-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="316e4-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="316e4-148">deviceMacAddress</span></span>|<span data-ttu-id="316e4-149">String</span><span class="sxs-lookup"><span data-stu-id="316e4-149">String</span></span>|<span data-ttu-id="316e4-150">设备的 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="316e4-150">Device Mac address.</span></span>|
|<span data-ttu-id="316e4-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="316e4-151">lastCheckInDateTime</span></span>|<span data-ttu-id="316e4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="316e4-152">DateTimeOffset</span></span>|<span data-ttu-id="316e4-153">设备的最后一个签入时间。</span><span class="sxs-lookup"><span data-stu-id="316e4-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="316e4-154">响应</span><span class="sxs-lookup"><span data-stu-id="316e4-154">Response</span></span>
<span data-ttu-id="316e4-155">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="316e4-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="316e4-156">示例</span><span class="sxs-lookup"><span data-stu-id="316e4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="316e4-157">请求</span><span class="sxs-lookup"><span data-stu-id="316e4-157">Request</span></span>
<span data-ttu-id="316e4-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="316e4-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="316e4-159">响应</span><span class="sxs-lookup"><span data-stu-id="316e4-159">Response</span></span>
<span data-ttu-id="316e4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="316e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




