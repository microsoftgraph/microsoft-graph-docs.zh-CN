---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97a81e0c1b32c5145a457c235b515eb57867b8b1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936972"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="70b62-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="70b62-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="70b62-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70b62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70b62-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70b62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70b62-106">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70b62-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70b62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="70b62-107">Prerequisites</span></span>
<span data-ttu-id="70b62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70b62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="70b62-110">Permission type</span></span>|<span data-ttu-id="70b62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70b62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70b62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70b62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70b62-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70b62-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70b62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70b62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70b62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70b62-115">Not supported.</span></span>|
|<span data-ttu-id="70b62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="70b62-116">Application</span></span>|<span data-ttu-id="70b62-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="70b62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70b62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70b62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="70b62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="70b62-119">Request headers</span></span>
|<span data-ttu-id="70b62-120">标头</span><span class="sxs-lookup"><span data-stu-id="70b62-120">Header</span></span>|<span data-ttu-id="70b62-121">值</span><span class="sxs-lookup"><span data-stu-id="70b62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70b62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70b62-122">Authorization</span></span>|<span data-ttu-id="70b62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70b62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70b62-124">接受</span><span class="sxs-lookup"><span data-stu-id="70b62-124">Accept</span></span>|<span data-ttu-id="70b62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70b62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70b62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70b62-126">Request body</span></span>
<span data-ttu-id="70b62-127">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70b62-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="70b62-128">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="70b62-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="70b62-129">属性</span><span class="sxs-lookup"><span data-stu-id="70b62-129">Property</span></span>|<span data-ttu-id="70b62-130">类型</span><span class="sxs-lookup"><span data-stu-id="70b62-130">Type</span></span>|<span data-ttu-id="70b62-131">说明</span><span class="sxs-lookup"><span data-stu-id="70b62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70b62-132">id</span><span class="sxs-lookup"><span data-stu-id="70b62-132">id</span></span>|<span data-ttu-id="70b62-133">字符串</span><span class="sxs-lookup"><span data-stu-id="70b62-133">String</span></span>|<span data-ttu-id="70b62-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="70b62-134">Key of the entity.</span></span> <span data-ttu-id="70b62-135">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="70b62-136">targetedMobileApps</span></span>|<span data-ttu-id="70b62-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="70b62-137">String collection</span></span>|<span data-ttu-id="70b62-138">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="70b62-138">the associated app.</span></span> <span data-ttu-id="70b62-139">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70b62-140">roleScopeTagIds</span></span>|<span data-ttu-id="70b62-141">String collection</span><span class="sxs-lookup"><span data-stu-id="70b62-141">String collection</span></span>|<span data-ttu-id="70b62-142">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="70b62-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="70b62-143">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70b62-144">createdDateTime</span></span>|<span data-ttu-id="70b62-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70b62-145">DateTimeOffset</span></span>|<span data-ttu-id="70b62-146">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="70b62-146">DateTime the object was created.</span></span> <span data-ttu-id="70b62-147">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-148">说明</span><span class="sxs-lookup"><span data-stu-id="70b62-148">description</span></span>|<span data-ttu-id="70b62-149">String</span><span class="sxs-lookup"><span data-stu-id="70b62-149">String</span></span>|<span data-ttu-id="70b62-150">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="70b62-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70b62-151">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70b62-152">lastModifiedDateTime</span></span>|<span data-ttu-id="70b62-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70b62-153">DateTimeOffset</span></span>|<span data-ttu-id="70b62-154">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="70b62-154">DateTime the object was last modified.</span></span> <span data-ttu-id="70b62-155">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-156">displayName</span><span class="sxs-lookup"><span data-stu-id="70b62-156">displayName</span></span>|<span data-ttu-id="70b62-157">String</span><span class="sxs-lookup"><span data-stu-id="70b62-157">String</span></span>|<span data-ttu-id="70b62-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="70b62-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70b62-159">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-160">version</span><span class="sxs-lookup"><span data-stu-id="70b62-160">version</span></span>|<span data-ttu-id="70b62-161">Int32</span><span class="sxs-lookup"><span data-stu-id="70b62-161">Int32</span></span>|<span data-ttu-id="70b62-162">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="70b62-162">Version of the device configuration.</span></span> <span data-ttu-id="70b62-163">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70b62-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="70b62-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="70b62-164">encodedSettingXml</span></span>|<span data-ttu-id="70b62-165">Binary</span><span class="sxs-lookup"><span data-stu-id="70b62-165">Binary</span></span>|<span data-ttu-id="70b62-166">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="70b62-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="70b62-167">settings</span><span class="sxs-lookup"><span data-stu-id="70b62-167">settings</span></span>|<span data-ttu-id="70b62-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70b62-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="70b62-169">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="70b62-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="70b62-170">响应</span><span class="sxs-lookup"><span data-stu-id="70b62-170">Response</span></span>
<span data-ttu-id="70b62-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70b62-171">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70b62-172">示例</span><span class="sxs-lookup"><span data-stu-id="70b62-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="70b62-173">请求</span><span class="sxs-lookup"><span data-stu-id="70b62-173">Request</span></span>
<span data-ttu-id="70b62-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70b62-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 596

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="70b62-175">响应</span><span class="sxs-lookup"><span data-stu-id="70b62-175">Response</span></span>
<span data-ttu-id="70b62-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70b62-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 768

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```




