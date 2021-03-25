---
title: 创建 windowsInformationProtectionDeviceRegistration
description: 创建新的 windowsInformationProtectionDeviceRegistration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a752cb3262d4ca8899660e0de50b637315680ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158883"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="94e39-103">创建 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="94e39-103">Create windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="94e39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94e39-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94e39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94e39-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94e39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94e39-107">创建新的 [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94e39-107">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94e39-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="94e39-108">Prerequisites</span></span>
<span data-ttu-id="94e39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94e39-111">Permission type</span></span>|<span data-ttu-id="94e39-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94e39-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94e39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94e39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94e39-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e39-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94e39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94e39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94e39-116">Not supported.</span></span>|
|<span data-ttu-id="94e39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94e39-117">Application</span></span>|<span data-ttu-id="94e39-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e39-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94e39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94e39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="94e39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94e39-120">Request headers</span></span>
|<span data-ttu-id="94e39-121">标头</span><span class="sxs-lookup"><span data-stu-id="94e39-121">Header</span></span>|<span data-ttu-id="94e39-122">值</span><span class="sxs-lookup"><span data-stu-id="94e39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94e39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e39-123">Authorization</span></span>|<span data-ttu-id="94e39-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94e39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94e39-125">接受</span><span class="sxs-lookup"><span data-stu-id="94e39-125">Accept</span></span>|<span data-ttu-id="94e39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94e39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94e39-127">Request body</span></span>
<span data-ttu-id="94e39-128">在请求正文中，提供 windowsInformationProtectionDeviceRegistration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94e39-128">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="94e39-129">下表显示创建 windowsInformationProtectionDeviceRegistration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="94e39-129">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="94e39-130">属性</span><span class="sxs-lookup"><span data-stu-id="94e39-130">Property</span></span>|<span data-ttu-id="94e39-131">类型</span><span class="sxs-lookup"><span data-stu-id="94e39-131">Type</span></span>|<span data-ttu-id="94e39-132">说明</span><span class="sxs-lookup"><span data-stu-id="94e39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94e39-133">id</span><span class="sxs-lookup"><span data-stu-id="94e39-133">id</span></span>|<span data-ttu-id="94e39-134">String</span><span class="sxs-lookup"><span data-stu-id="94e39-134">String</span></span>|<span data-ttu-id="94e39-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94e39-135">Key of the entity.</span></span>|
|<span data-ttu-id="94e39-136">userId</span><span class="sxs-lookup"><span data-stu-id="94e39-136">userId</span></span>|<span data-ttu-id="94e39-137">String</span><span class="sxs-lookup"><span data-stu-id="94e39-137">String</span></span>|<span data-ttu-id="94e39-138">与此设备注册记录关联的 UserId。</span><span class="sxs-lookup"><span data-stu-id="94e39-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="94e39-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="94e39-139">deviceRegistrationId</span></span>|<span data-ttu-id="94e39-140">字符串</span><span class="sxs-lookup"><span data-stu-id="94e39-140">String</span></span>|<span data-ttu-id="94e39-141">此设备注册记录的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="94e39-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="94e39-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="94e39-142">deviceName</span></span>|<span data-ttu-id="94e39-143">String</span><span class="sxs-lookup"><span data-stu-id="94e39-143">String</span></span>|<span data-ttu-id="94e39-144">设备名称。</span><span class="sxs-lookup"><span data-stu-id="94e39-144">Device name.</span></span>|
|<span data-ttu-id="94e39-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="94e39-145">deviceType</span></span>|<span data-ttu-id="94e39-146">String</span><span class="sxs-lookup"><span data-stu-id="94e39-146">String</span></span>|<span data-ttu-id="94e39-147">设备类型，例如，Windows 笔记本电脑 VS Windows 手机。</span><span class="sxs-lookup"><span data-stu-id="94e39-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="94e39-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="94e39-148">deviceMacAddress</span></span>|<span data-ttu-id="94e39-149">String</span><span class="sxs-lookup"><span data-stu-id="94e39-149">String</span></span>|<span data-ttu-id="94e39-150">设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="94e39-150">Device Mac address.</span></span>|
|<span data-ttu-id="94e39-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="94e39-151">lastCheckInDateTime</span></span>|<span data-ttu-id="94e39-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94e39-152">DateTimeOffset</span></span>|<span data-ttu-id="94e39-153">设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="94e39-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="94e39-154">响应</span><span class="sxs-lookup"><span data-stu-id="94e39-154">Response</span></span>
<span data-ttu-id="94e39-155">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94e39-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e39-156">示例</span><span class="sxs-lookup"><span data-stu-id="94e39-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="94e39-157">请求</span><span class="sxs-lookup"><span data-stu-id="94e39-157">Request</span></span>
<span data-ttu-id="94e39-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94e39-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94e39-159">响应</span><span class="sxs-lookup"><span data-stu-id="94e39-159">Response</span></span>
<span data-ttu-id="94e39-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94e39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




