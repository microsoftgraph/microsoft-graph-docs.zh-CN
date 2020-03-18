---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc6c8eb33177cb4c662dfa290979f059bf8b4932
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803040"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="84861-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="84861-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="84861-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84861-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84861-106">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84861-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84861-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="84861-107">Prerequisites</span></span>
<span data-ttu-id="84861-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84861-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84861-110">Permission type</span></span>|<span data-ttu-id="84861-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84861-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84861-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84861-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84861-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84861-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="84861-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84861-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84861-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84861-115">Not supported.</span></span>|
|<span data-ttu-id="84861-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84861-116">Application</span></span>|<span data-ttu-id="84861-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84861-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84861-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84861-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84861-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84861-119">Request headers</span></span>
|<span data-ttu-id="84861-120">标头</span><span class="sxs-lookup"><span data-stu-id="84861-120">Header</span></span>|<span data-ttu-id="84861-121">值</span><span class="sxs-lookup"><span data-stu-id="84861-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84861-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84861-122">Authorization</span></span>|<span data-ttu-id="84861-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84861-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84861-124">接受</span><span class="sxs-lookup"><span data-stu-id="84861-124">Accept</span></span>|<span data-ttu-id="84861-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84861-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84861-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="84861-126">Request body</span></span>
<span data-ttu-id="84861-127">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84861-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="84861-128">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84861-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="84861-129">属性</span><span class="sxs-lookup"><span data-stu-id="84861-129">Property</span></span>|<span data-ttu-id="84861-130">类型</span><span class="sxs-lookup"><span data-stu-id="84861-130">Type</span></span>|<span data-ttu-id="84861-131">说明</span><span class="sxs-lookup"><span data-stu-id="84861-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84861-132">id</span><span class="sxs-lookup"><span data-stu-id="84861-132">id</span></span>|<span data-ttu-id="84861-133">字符串</span><span class="sxs-lookup"><span data-stu-id="84861-133">String</span></span>|<span data-ttu-id="84861-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="84861-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-135">displayName</span><span class="sxs-lookup"><span data-stu-id="84861-135">displayName</span></span>|<span data-ttu-id="84861-136">String</span><span class="sxs-lookup"><span data-stu-id="84861-136">String</span></span>|<span data-ttu-id="84861-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="84861-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-138">说明</span><span class="sxs-lookup"><span data-stu-id="84861-138">description</span></span>|<span data-ttu-id="84861-139">String</span><span class="sxs-lookup"><span data-stu-id="84861-139">String</span></span>|<span data-ttu-id="84861-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="84861-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-141">priority</span><span class="sxs-lookup"><span data-stu-id="84861-141">priority</span></span>|<span data-ttu-id="84861-142">Int32</span><span class="sxs-lookup"><span data-stu-id="84861-142">Int32</span></span>|<span data-ttu-id="84861-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="84861-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="84861-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="84861-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="84861-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84861-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84861-146">createdDateTime</span></span>|<span data-ttu-id="84861-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84861-147">DateTimeOffset</span></span>|<span data-ttu-id="84861-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="84861-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84861-149">lastModifiedDateTime</span></span>|<span data-ttu-id="84861-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84861-150">DateTimeOffset</span></span>|<span data-ttu-id="84861-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="84861-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-152">version</span><span class="sxs-lookup"><span data-stu-id="84861-152">version</span></span>|<span data-ttu-id="84861-153">Int32</span><span class="sxs-lookup"><span data-stu-id="84861-153">Int32</span></span>|<span data-ttu-id="84861-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="84861-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="84861-155">limit</span><span class="sxs-lookup"><span data-stu-id="84861-155">limit</span></span>|<span data-ttu-id="84861-156">Int32</span><span class="sxs-lookup"><span data-stu-id="84861-156">Int32</span></span>|<span data-ttu-id="84861-157">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="84861-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="84861-158">响应</span><span class="sxs-lookup"><span data-stu-id="84861-158">Response</span></span>
<span data-ttu-id="84861-159">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84861-159">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84861-160">示例</span><span class="sxs-lookup"><span data-stu-id="84861-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="84861-161">请求</span><span class="sxs-lookup"><span data-stu-id="84861-161">Request</span></span>
<span data-ttu-id="84861-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84861-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="84861-163">响应</span><span class="sxs-lookup"><span data-stu-id="84861-163">Response</span></span>
<span data-ttu-id="84861-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84861-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




