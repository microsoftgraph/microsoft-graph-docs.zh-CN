---
title: 更新 deviceComanagementAuthorityConfiguration
description: 更新 deviceComanagementAuthorityConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a9e6ed4177c866d7945841cc4ca66404faea895
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301551"
---
# <a name="update-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="e4e95-103">更新 deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4e95-103">Update deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="e4e95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4e95-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4e95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4e95-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4e95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4e95-107">更新 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4e95-107">Update the properties of a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4e95-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4e95-108">Prerequisites</span></span>
<span data-ttu-id="e4e95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4e95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e95-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4e95-111">Permission type</span></span>|<span data-ttu-id="e4e95-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4e95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e95-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e95-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e95-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e4e95-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e95-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4e95-116">Not supported.</span></span>|
|<span data-ttu-id="e4e95-117">Application</span><span class="sxs-lookup"><span data-stu-id="e4e95-117">Application</span></span>|<span data-ttu-id="e4e95-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e95-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e95-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4e95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e4e95-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4e95-120">Request headers</span></span>
|<span data-ttu-id="e4e95-121">标头</span><span class="sxs-lookup"><span data-stu-id="e4e95-121">Header</span></span>|<span data-ttu-id="e4e95-122">值</span><span class="sxs-lookup"><span data-stu-id="e4e95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4e95-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e95-123">Authorization</span></span>|<span data-ttu-id="e4e95-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4e95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4e95-125">接受</span><span class="sxs-lookup"><span data-stu-id="e4e95-125">Accept</span></span>|<span data-ttu-id="e4e95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e95-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4e95-127">Request body</span></span>
<span data-ttu-id="e4e95-128">在请求正文中，提供 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4e95-128">In the request body, supply a JSON representation for the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

<span data-ttu-id="e4e95-129">下表显示创建 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4e95-129">The following table shows the properties that are required when you create the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span></span>

|<span data-ttu-id="e4e95-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4e95-130">Property</span></span>|<span data-ttu-id="e4e95-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4e95-131">Type</span></span>|<span data-ttu-id="e4e95-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4e95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4e95-133">id</span><span class="sxs-lookup"><span data-stu-id="e4e95-133">id</span></span>|<span data-ttu-id="e4e95-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e4e95-134">String</span></span>|<span data-ttu-id="e4e95-135">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e4e95-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e4e95-136">displayName</span></span>|<span data-ttu-id="e4e95-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e4e95-137">String</span></span>|<span data-ttu-id="e4e95-138">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="e4e95-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-139">description</span><span class="sxs-lookup"><span data-stu-id="e4e95-139">description</span></span>|<span data-ttu-id="e4e95-140">字符串</span><span class="sxs-lookup"><span data-stu-id="e4e95-140">String</span></span>|<span data-ttu-id="e4e95-141">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="e4e95-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-142">priority</span><span class="sxs-lookup"><span data-stu-id="e4e95-142">priority</span></span>|<span data-ttu-id="e4e95-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e95-143">Int32</span></span>|<span data-ttu-id="e4e95-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="e4e95-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="e4e95-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="e4e95-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="e4e95-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4e95-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e95-147">createdDateTime</span></span>|<span data-ttu-id="e4e95-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e95-148">DateTimeOffset</span></span>|<span data-ttu-id="e4e95-149">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="e4e95-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e95-150">lastModifiedDateTime</span></span>|<span data-ttu-id="e4e95-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e95-151">DateTimeOffset</span></span>|<span data-ttu-id="e4e95-152">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="e4e95-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-153">version</span><span class="sxs-lookup"><span data-stu-id="e4e95-153">version</span></span>|<span data-ttu-id="e4e95-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e95-154">Int32</span></span>|<span data-ttu-id="e4e95-155">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="e4e95-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4e95-156">roleScopeTagIds</span></span>|<span data-ttu-id="e4e95-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="e4e95-157">String collection</span></span>|<span data-ttu-id="e4e95-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="e4e95-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="e4e95-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4e95-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e4e95-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="e4e95-160">managedDeviceAuthority</span></span>|<span data-ttu-id="e4e95-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e95-161">Int32</span></span>|<span data-ttu-id="e4e95-162">CoManagement 颁发机构配置 ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="e4e95-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="e4e95-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="e4e95-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="e4e95-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4e95-164">Boolean</span></span>|<span data-ttu-id="e4e95-165">CoManagement 颁发机构配置 InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="e4e95-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="e4e95-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="e4e95-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="e4e95-167">字符串</span><span class="sxs-lookup"><span data-stu-id="e4e95-167">String</span></span>|<span data-ttu-id="e4e95-168">CoManagement 颁发机构配置 ConfigurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="e4e95-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="e4e95-169">响应</span><span class="sxs-lookup"><span data-stu-id="e4e95-169">Response</span></span>
<span data-ttu-id="e4e95-170">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4e95-170">If successful, this method returns a `200 OK` response code and an updated [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e95-171">示例</span><span class="sxs-lookup"><span data-stu-id="e4e95-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e95-172">请求</span><span class="sxs-lookup"><span data-stu-id="e4e95-172">Request</span></span>
<span data-ttu-id="e4e95-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4e95-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```

### <a name="response"></a><span data-ttu-id="e4e95-174">响应</span><span class="sxs-lookup"><span data-stu-id="e4e95-174">Response</span></span>
<span data-ttu-id="e4e95-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4e95-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 617

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "0ba0057f-057f-0ba0-7f05-a00b7f05a00b",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```




