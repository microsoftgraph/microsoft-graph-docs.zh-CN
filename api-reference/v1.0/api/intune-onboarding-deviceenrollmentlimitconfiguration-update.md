---
title: 更新 deviceEnrollmentLimitConfiguration
description: 更新 deviceEnrollmentLimitConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc479345fa9083976c937ec8bf71630e2205a0c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758029"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="aab4d-103">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="aab4d-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="aab4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aab4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aab4d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aab4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aab4d-106">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aab4d-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aab4d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aab4d-107">Prerequisites</span></span>
<span data-ttu-id="aab4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aab4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aab4d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aab4d-110">Permission type</span></span>|<span data-ttu-id="aab4d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aab4d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aab4d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aab4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aab4d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aab4d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aab4d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aab4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aab4d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab4d-115">Not supported.</span></span>|
|<span data-ttu-id="aab4d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aab4d-116">Application</span></span>|<span data-ttu-id="aab4d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aab4d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aab4d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aab4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aab4d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aab4d-119">Request headers</span></span>
|<span data-ttu-id="aab4d-120">标头</span><span class="sxs-lookup"><span data-stu-id="aab4d-120">Header</span></span>|<span data-ttu-id="aab4d-121">值</span><span class="sxs-lookup"><span data-stu-id="aab4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aab4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab4d-122">Authorization</span></span>|<span data-ttu-id="aab4d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aab4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aab4d-124">接受</span><span class="sxs-lookup"><span data-stu-id="aab4d-124">Accept</span></span>|<span data-ttu-id="aab4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aab4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab4d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aab4d-126">Request body</span></span>
<span data-ttu-id="aab4d-127">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aab4d-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="aab4d-128">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aab4d-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="aab4d-129">属性</span><span class="sxs-lookup"><span data-stu-id="aab4d-129">Property</span></span>|<span data-ttu-id="aab4d-130">类型</span><span class="sxs-lookup"><span data-stu-id="aab4d-130">Type</span></span>|<span data-ttu-id="aab4d-131">说明</span><span class="sxs-lookup"><span data-stu-id="aab4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aab4d-132">id</span><span class="sxs-lookup"><span data-stu-id="aab4d-132">id</span></span>|<span data-ttu-id="aab4d-133">String</span><span class="sxs-lookup"><span data-stu-id="aab4d-133">String</span></span>|<span data-ttu-id="aab4d-134">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aab4d-135">displayName</span></span>|<span data-ttu-id="aab4d-136">String</span><span class="sxs-lookup"><span data-stu-id="aab4d-136">String</span></span>|<span data-ttu-id="aab4d-137">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-138">description</span><span class="sxs-lookup"><span data-stu-id="aab4d-138">description</span></span>|<span data-ttu-id="aab4d-139">String</span><span class="sxs-lookup"><span data-stu-id="aab4d-139">String</span></span>|<span data-ttu-id="aab4d-140">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-141">priority</span><span class="sxs-lookup"><span data-stu-id="aab4d-141">priority</span></span>|<span data-ttu-id="aab4d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="aab4d-142">Int32</span></span>|<span data-ttu-id="aab4d-143">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="aab4d-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="aab4d-144">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="aab4d-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="aab4d-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aab4d-146">createdDateTime</span></span>|<span data-ttu-id="aab4d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aab4d-147">DateTimeOffset</span></span>|<span data-ttu-id="aab4d-148">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aab4d-149">lastModifiedDateTime</span></span>|<span data-ttu-id="aab4d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aab4d-150">DateTimeOffset</span></span>|<span data-ttu-id="aab4d-151">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-152">version</span><span class="sxs-lookup"><span data-stu-id="aab4d-152">version</span></span>|<span data-ttu-id="aab4d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="aab4d-153">Int32</span></span>|<span data-ttu-id="aab4d-154">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aab4d-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aab4d-155">limit</span><span class="sxs-lookup"><span data-stu-id="aab4d-155">limit</span></span>|<span data-ttu-id="aab4d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="aab4d-156">Int32</span></span>|<span data-ttu-id="aab4d-157">用户可以注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="aab4d-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="aab4d-158">响应</span><span class="sxs-lookup"><span data-stu-id="aab4d-158">Response</span></span>
<span data-ttu-id="aab4d-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aab4d-159">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab4d-160">示例</span><span class="sxs-lookup"><span data-stu-id="aab4d-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="aab4d-161">请求</span><span class="sxs-lookup"><span data-stu-id="aab4d-161">Request</span></span>
<span data-ttu-id="aab4d-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aab4d-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="aab4d-163">响应</span><span class="sxs-lookup"><span data-stu-id="aab4d-163">Response</span></span>
<span data-ttu-id="aab4d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aab4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




