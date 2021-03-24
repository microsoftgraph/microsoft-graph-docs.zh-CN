---
title: 更新 deviceComanagementAuthorityConfiguration
description: 更新 deviceComanagementAuthorityConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ab03be505736eb358e784d68ce97fd924526a9a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135087"
---
# <a name="update-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="a7c2e-103">更新 deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7c2e-103">Update deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="a7c2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7c2e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7c2e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c2e-107">更新 [deviceComanagementAuthorityConfiguration 对象](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-107">Update the properties of a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7c2e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7c2e-108">Prerequisites</span></span>
<span data-ttu-id="a7c2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c2e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7c2e-111">Permission type</span></span>|<span data-ttu-id="a7c2e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7c2e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7c2e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7c2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7c2e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7c2e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7c2e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7c2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7c2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-116">Not supported.</span></span>|
|<span data-ttu-id="a7c2e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7c2e-117">Application</span></span>|<span data-ttu-id="a7c2e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7c2e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7c2e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7c2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7c2e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7c2e-120">Request headers</span></span>
|<span data-ttu-id="a7c2e-121">标头</span><span class="sxs-lookup"><span data-stu-id="a7c2e-121">Header</span></span>|<span data-ttu-id="a7c2e-122">值</span><span class="sxs-lookup"><span data-stu-id="a7c2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7c2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7c2e-123">Authorization</span></span>|<span data-ttu-id="a7c2e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7c2e-125">接受</span><span class="sxs-lookup"><span data-stu-id="a7c2e-125">Accept</span></span>|<span data-ttu-id="a7c2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7c2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c2e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7c2e-127">Request body</span></span>
<span data-ttu-id="a7c2e-128">在请求正文中，提供 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-128">In the request body, supply a JSON representation for the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

<span data-ttu-id="a7c2e-129">下表显示创建 [deviceComanagementAuthorityConfiguration 时所需的属性](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-129">The following table shows the properties that are required when you create the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span></span>

|<span data-ttu-id="a7c2e-130">属性</span><span class="sxs-lookup"><span data-stu-id="a7c2e-130">Property</span></span>|<span data-ttu-id="a7c2e-131">类型</span><span class="sxs-lookup"><span data-stu-id="a7c2e-131">Type</span></span>|<span data-ttu-id="a7c2e-132">说明</span><span class="sxs-lookup"><span data-stu-id="a7c2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c2e-133">id</span><span class="sxs-lookup"><span data-stu-id="a7c2e-133">id</span></span>|<span data-ttu-id="a7c2e-134">String</span><span class="sxs-lookup"><span data-stu-id="a7c2e-134">String</span></span>|<span data-ttu-id="a7c2e-135">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a7c2e-136">displayName</span></span>|<span data-ttu-id="a7c2e-137">String</span><span class="sxs-lookup"><span data-stu-id="a7c2e-137">String</span></span>|<span data-ttu-id="a7c2e-138">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-139">说明</span><span class="sxs-lookup"><span data-stu-id="a7c2e-139">description</span></span>|<span data-ttu-id="a7c2e-140">String</span><span class="sxs-lookup"><span data-stu-id="a7c2e-140">String</span></span>|<span data-ttu-id="a7c2e-141">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-142">priority</span><span class="sxs-lookup"><span data-stu-id="a7c2e-142">priority</span></span>|<span data-ttu-id="a7c2e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c2e-143">Int32</span></span>|<span data-ttu-id="a7c2e-144">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a7c2e-145">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="a7c2e-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c2e-147">createdDateTime</span></span>|<span data-ttu-id="a7c2e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c2e-148">DateTimeOffset</span></span>|<span data-ttu-id="a7c2e-149">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c2e-150">lastModifiedDateTime</span></span>|<span data-ttu-id="a7c2e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c2e-151">DateTimeOffset</span></span>|<span data-ttu-id="a7c2e-152">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-153">version</span><span class="sxs-lookup"><span data-stu-id="a7c2e-153">version</span></span>|<span data-ttu-id="a7c2e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c2e-154">Int32</span></span>|<span data-ttu-id="a7c2e-155">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7c2e-156">roleScopeTagIds</span></span>|<span data-ttu-id="a7c2e-157">String collection</span><span class="sxs-lookup"><span data-stu-id="a7c2e-157">String collection</span></span>|<span data-ttu-id="a7c2e-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="a7c2e-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7c2e-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a7c2e-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="a7c2e-160">managedDeviceAuthority</span></span>|<span data-ttu-id="a7c2e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a7c2e-161">Int32</span></span>|<span data-ttu-id="a7c2e-162">CoManagement Authority 配置 ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="a7c2e-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="a7c2e-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="a7c2e-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="a7c2e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7c2e-164">Boolean</span></span>|<span data-ttu-id="a7c2e-165">CoManagement Authority 配置 InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="a7c2e-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="a7c2e-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="a7c2e-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="a7c2e-167">String</span><span class="sxs-lookup"><span data-stu-id="a7c2e-167">String</span></span>|<span data-ttu-id="a7c2e-168">CoManagement Authority 配置配置ManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="a7c2e-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="a7c2e-169">响应</span><span class="sxs-lookup"><span data-stu-id="a7c2e-169">Response</span></span>
<span data-ttu-id="a7c2e-170">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-170">If successful, this method returns a `200 OK` response code and an updated [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7c2e-171">示例</span><span class="sxs-lookup"><span data-stu-id="a7c2e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7c2e-172">请求</span><span class="sxs-lookup"><span data-stu-id="a7c2e-172">Request</span></span>
<span data-ttu-id="a7c2e-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7c2e-174">响应</span><span class="sxs-lookup"><span data-stu-id="a7c2e-174">Response</span></span>
<span data-ttu-id="a7c2e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7c2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




