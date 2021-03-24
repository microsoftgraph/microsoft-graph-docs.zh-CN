---
title: 更新 deviceEnrollmentLimitConfiguration
description: 更新 deviceEnrollmentLimitConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ba360475199d47bda3b2c65ee6c7991bbb8fb91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135017"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d4e0c-103">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4e0c-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="d4e0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4e0c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e0c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e0c-107">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e0c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4e0c-108">Prerequisites</span></span>
<span data-ttu-id="d4e0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e0c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4e0c-111">Permission type</span></span>|<span data-ttu-id="d4e0c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4e0c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e0c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4e0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e0c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e0c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e0c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4e0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e0c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-116">Not supported.</span></span>|
|<span data-ttu-id="d4e0c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4e0c-117">Application</span></span>|<span data-ttu-id="d4e0c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e0c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e0c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4e0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4e0c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4e0c-120">Request headers</span></span>
|<span data-ttu-id="d4e0c-121">标头</span><span class="sxs-lookup"><span data-stu-id="d4e0c-121">Header</span></span>|<span data-ttu-id="d4e0c-122">值</span><span class="sxs-lookup"><span data-stu-id="d4e0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e0c-123">Authorization</span></span>|<span data-ttu-id="d4e0c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e0c-125">接受</span><span class="sxs-lookup"><span data-stu-id="d4e0c-125">Accept</span></span>|<span data-ttu-id="d4e0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e0c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4e0c-127">Request body</span></span>
<span data-ttu-id="d4e0c-128">在请求正文中，提供 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="d4e0c-129">下表显示创建 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="d4e0c-130">属性</span><span class="sxs-lookup"><span data-stu-id="d4e0c-130">Property</span></span>|<span data-ttu-id="d4e0c-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4e0c-131">Type</span></span>|<span data-ttu-id="d4e0c-132">说明</span><span class="sxs-lookup"><span data-stu-id="d4e0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e0c-133">id</span><span class="sxs-lookup"><span data-stu-id="d4e0c-133">id</span></span>|<span data-ttu-id="d4e0c-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e0c-134">String</span></span>|<span data-ttu-id="d4e0c-135">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d4e0c-136">displayName</span></span>|<span data-ttu-id="d4e0c-137">String</span><span class="sxs-lookup"><span data-stu-id="d4e0c-137">String</span></span>|<span data-ttu-id="d4e0c-138">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-139">说明</span><span class="sxs-lookup"><span data-stu-id="d4e0c-139">description</span></span>|<span data-ttu-id="d4e0c-140">String</span><span class="sxs-lookup"><span data-stu-id="d4e0c-140">String</span></span>|<span data-ttu-id="d4e0c-141">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-142">priority</span><span class="sxs-lookup"><span data-stu-id="d4e0c-142">priority</span></span>|<span data-ttu-id="d4e0c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e0c-143">Int32</span></span>|<span data-ttu-id="d4e0c-144">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d4e0c-145">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="d4e0c-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e0c-147">createdDateTime</span></span>|<span data-ttu-id="d4e0c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e0c-148">DateTimeOffset</span></span>|<span data-ttu-id="d4e0c-149">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e0c-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d4e0c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e0c-151">DateTimeOffset</span></span>|<span data-ttu-id="d4e0c-152">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-153">version</span><span class="sxs-lookup"><span data-stu-id="d4e0c-153">version</span></span>|<span data-ttu-id="d4e0c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e0c-154">Int32</span></span>|<span data-ttu-id="d4e0c-155">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4e0c-156">roleScopeTagIds</span></span>|<span data-ttu-id="d4e0c-157">String collection</span><span class="sxs-lookup"><span data-stu-id="d4e0c-157">String collection</span></span>|<span data-ttu-id="d4e0c-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="d4e0c-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d4e0c-160">limit</span><span class="sxs-lookup"><span data-stu-id="d4e0c-160">limit</span></span>|<span data-ttu-id="d4e0c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e0c-161">Int32</span></span>|<span data-ttu-id="d4e0c-162">用户可以注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="d4e0c-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="d4e0c-163">响应</span><span class="sxs-lookup"><span data-stu-id="d4e0c-163">Response</span></span>
<span data-ttu-id="d4e0c-164">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-164">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e0c-165">示例</span><span class="sxs-lookup"><span data-stu-id="d4e0c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e0c-166">请求</span><span class="sxs-lookup"><span data-stu-id="d4e0c-166">Request</span></span>
<span data-ttu-id="d4e0c-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="d4e0c-168">响应</span><span class="sxs-lookup"><span data-stu-id="d4e0c-168">Response</span></span>
<span data-ttu-id="d4e0c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




