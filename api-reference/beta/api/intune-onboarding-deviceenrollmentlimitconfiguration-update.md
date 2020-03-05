---
title: 更新 deviceEnrollmentLimitConfiguration
description: 更新 deviceEnrollmentLimitConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34854bb09daf1b6e36f54315e6741a6b3ce85177
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462360"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="5814f-103">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="5814f-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="5814f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5814f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5814f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5814f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5814f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5814f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5814f-107">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5814f-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5814f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5814f-108">Prerequisites</span></span>
<span data-ttu-id="5814f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5814f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5814f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5814f-111">Permission type</span></span>|<span data-ttu-id="5814f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5814f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5814f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5814f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5814f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5814f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5814f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5814f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5814f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5814f-116">Not supported.</span></span>|
|<span data-ttu-id="5814f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5814f-117">Application</span></span>|<span data-ttu-id="5814f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5814f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5814f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5814f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5814f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5814f-120">Request headers</span></span>
|<span data-ttu-id="5814f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5814f-121">Header</span></span>|<span data-ttu-id="5814f-122">值</span><span class="sxs-lookup"><span data-stu-id="5814f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5814f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5814f-123">Authorization</span></span>|<span data-ttu-id="5814f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5814f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5814f-125">接受</span><span class="sxs-lookup"><span data-stu-id="5814f-125">Accept</span></span>|<span data-ttu-id="5814f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5814f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5814f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5814f-127">Request body</span></span>
<span data-ttu-id="5814f-128">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5814f-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="5814f-129">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5814f-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="5814f-130">属性</span><span class="sxs-lookup"><span data-stu-id="5814f-130">Property</span></span>|<span data-ttu-id="5814f-131">类型</span><span class="sxs-lookup"><span data-stu-id="5814f-131">Type</span></span>|<span data-ttu-id="5814f-132">说明</span><span class="sxs-lookup"><span data-stu-id="5814f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5814f-133">id</span><span class="sxs-lookup"><span data-stu-id="5814f-133">id</span></span>|<span data-ttu-id="5814f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5814f-134">String</span></span>|<span data-ttu-id="5814f-135">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5814f-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5814f-136">displayName</span></span>|<span data-ttu-id="5814f-137">String</span><span class="sxs-lookup"><span data-stu-id="5814f-137">String</span></span>|<span data-ttu-id="5814f-138">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="5814f-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-139">说明</span><span class="sxs-lookup"><span data-stu-id="5814f-139">description</span></span>|<span data-ttu-id="5814f-140">String</span><span class="sxs-lookup"><span data-stu-id="5814f-140">String</span></span>|<span data-ttu-id="5814f-141">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="5814f-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-142">priority</span><span class="sxs-lookup"><span data-stu-id="5814f-142">priority</span></span>|<span data-ttu-id="5814f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5814f-143">Int32</span></span>|<span data-ttu-id="5814f-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="5814f-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="5814f-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="5814f-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="5814f-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5814f-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5814f-147">createdDateTime</span></span>|<span data-ttu-id="5814f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5814f-148">DateTimeOffset</span></span>|<span data-ttu-id="5814f-149">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="5814f-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5814f-150">lastModifiedDateTime</span></span>|<span data-ttu-id="5814f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5814f-151">DateTimeOffset</span></span>|<span data-ttu-id="5814f-152">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="5814f-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-153">version</span><span class="sxs-lookup"><span data-stu-id="5814f-153">version</span></span>|<span data-ttu-id="5814f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5814f-154">Int32</span></span>|<span data-ttu-id="5814f-155">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="5814f-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5814f-156">limit</span><span class="sxs-lookup"><span data-stu-id="5814f-156">limit</span></span>|<span data-ttu-id="5814f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5814f-157">Int32</span></span>|<span data-ttu-id="5814f-158">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="5814f-158">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="5814f-159">响应</span><span class="sxs-lookup"><span data-stu-id="5814f-159">Response</span></span>
<span data-ttu-id="5814f-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5814f-160">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5814f-161">示例</span><span class="sxs-lookup"><span data-stu-id="5814f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="5814f-162">请求</span><span class="sxs-lookup"><span data-stu-id="5814f-162">Request</span></span>
<span data-ttu-id="5814f-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5814f-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="5814f-164">响应</span><span class="sxs-lookup"><span data-stu-id="5814f-164">Response</span></span>
<span data-ttu-id="5814f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5814f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```





