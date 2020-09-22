---
title: 创建 deviceEnrollmentLimitConfiguration
description: 创建新的 deviceEnrollmentLimitConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb46b79637fa941edfb0d8b83dc7664c2e06213f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000222"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="90912-103">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="90912-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="90912-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90912-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90912-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90912-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90912-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90912-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90912-107">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90912-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90912-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="90912-108">Prerequisites</span></span>
<span data-ttu-id="90912-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90912-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="90912-111">Permission type</span></span>|<span data-ttu-id="90912-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90912-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90912-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90912-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90912-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90912-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90912-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90912-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90912-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90912-116">Not supported.</span></span>|
|<span data-ttu-id="90912-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="90912-117">Application</span></span>|<span data-ttu-id="90912-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90912-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90912-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90912-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90912-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="90912-120">Request headers</span></span>
|<span data-ttu-id="90912-121">标头</span><span class="sxs-lookup"><span data-stu-id="90912-121">Header</span></span>|<span data-ttu-id="90912-122">值</span><span class="sxs-lookup"><span data-stu-id="90912-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90912-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90912-123">Authorization</span></span>|<span data-ttu-id="90912-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90912-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90912-125">接受</span><span class="sxs-lookup"><span data-stu-id="90912-125">Accept</span></span>|<span data-ttu-id="90912-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90912-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90912-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="90912-127">Request body</span></span>
<span data-ttu-id="90912-128">在请求正文中，提供 deviceEnrollmentLimitConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90912-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="90912-129">下表显示创建 deviceEnrollmentLimitConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90912-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="90912-130">属性</span><span class="sxs-lookup"><span data-stu-id="90912-130">Property</span></span>|<span data-ttu-id="90912-131">类型</span><span class="sxs-lookup"><span data-stu-id="90912-131">Type</span></span>|<span data-ttu-id="90912-132">说明</span><span class="sxs-lookup"><span data-stu-id="90912-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90912-133">id</span><span class="sxs-lookup"><span data-stu-id="90912-133">id</span></span>|<span data-ttu-id="90912-134">String</span><span class="sxs-lookup"><span data-stu-id="90912-134">String</span></span>|<span data-ttu-id="90912-135">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="90912-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-136">displayName</span><span class="sxs-lookup"><span data-stu-id="90912-136">displayName</span></span>|<span data-ttu-id="90912-137">String</span><span class="sxs-lookup"><span data-stu-id="90912-137">String</span></span>|<span data-ttu-id="90912-138">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="90912-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-139">description</span><span class="sxs-lookup"><span data-stu-id="90912-139">description</span></span>|<span data-ttu-id="90912-140">String</span><span class="sxs-lookup"><span data-stu-id="90912-140">String</span></span>|<span data-ttu-id="90912-141">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="90912-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-142">priority</span><span class="sxs-lookup"><span data-stu-id="90912-142">priority</span></span>|<span data-ttu-id="90912-143">Int32</span><span class="sxs-lookup"><span data-stu-id="90912-143">Int32</span></span>|<span data-ttu-id="90912-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="90912-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="90912-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="90912-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="90912-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90912-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90912-147">createdDateTime</span></span>|<span data-ttu-id="90912-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90912-148">DateTimeOffset</span></span>|<span data-ttu-id="90912-149">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="90912-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90912-150">lastModifiedDateTime</span></span>|<span data-ttu-id="90912-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90912-151">DateTimeOffset</span></span>|<span data-ttu-id="90912-152">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="90912-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-153">version</span><span class="sxs-lookup"><span data-stu-id="90912-153">version</span></span>|<span data-ttu-id="90912-154">Int32</span><span class="sxs-lookup"><span data-stu-id="90912-154">Int32</span></span>|<span data-ttu-id="90912-155">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="90912-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90912-156">roleScopeTagIds</span></span>|<span data-ttu-id="90912-157">String collection</span><span class="sxs-lookup"><span data-stu-id="90912-157">String collection</span></span>|<span data-ttu-id="90912-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="90912-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="90912-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="90912-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="90912-160">limit</span><span class="sxs-lookup"><span data-stu-id="90912-160">limit</span></span>|<span data-ttu-id="90912-161">Int32</span><span class="sxs-lookup"><span data-stu-id="90912-161">Int32</span></span>|<span data-ttu-id="90912-162">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="90912-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="90912-163">响应</span><span class="sxs-lookup"><span data-stu-id="90912-163">Response</span></span>
<span data-ttu-id="90912-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90912-164">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90912-165">示例</span><span class="sxs-lookup"><span data-stu-id="90912-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="90912-166">请求</span><span class="sxs-lookup"><span data-stu-id="90912-166">Request</span></span>
<span data-ttu-id="90912-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90912-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="90912-168">响应</span><span class="sxs-lookup"><span data-stu-id="90912-168">Response</span></span>
<span data-ttu-id="90912-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90912-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```






