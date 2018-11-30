---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
ms.openlocfilehash: 089a3d499ac656421ed6b7e2f0fd3a3c9fcca079
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044185"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="fe8d8-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe8d8-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="fe8d8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe8d8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe8d8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe8d8-107">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe8d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe8d8-108">Prerequisites</span></span>
<span data-ttu-id="fe8d8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fe8d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe8d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe8d8-111">Permission type</span></span>|<span data-ttu-id="fe8d8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe8d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe8d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe8d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe8d8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8d8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe8d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe8d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe8d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-116">Not supported.</span></span>|
|<span data-ttu-id="fe8d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe8d8-117">Application</span></span>|<span data-ttu-id="fe8d8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe8d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe8d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fe8d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe8d8-120">Request headers</span></span>
|<span data-ttu-id="fe8d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="fe8d8-121">Header</span></span>|<span data-ttu-id="fe8d8-122">值</span><span class="sxs-lookup"><span data-stu-id="fe8d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe8d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe8d8-123">Authorization</span></span>|<span data-ttu-id="fe8d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe8d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe8d8-125">Accept</span></span>|<span data-ttu-id="fe8d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe8d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe8d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe8d8-127">Request body</span></span>
<span data-ttu-id="fe8d8-128">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="fe8d8-129">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="fe8d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe8d8-130">Property</span></span>|<span data-ttu-id="fe8d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe8d8-131">Type</span></span>|<span data-ttu-id="fe8d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe8d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe8d8-133">id</span><span class="sxs-lookup"><span data-stu-id="fe8d8-133">id</span></span>|<span data-ttu-id="fe8d8-134">String</span><span class="sxs-lookup"><span data-stu-id="fe8d8-134">String</span></span>|<span data-ttu-id="fe8d8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-135">Key of the entity.</span></span> <span data-ttu-id="fe8d8-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="fe8d8-137">targetedMobileApps</span></span>|<span data-ttu-id="fe8d8-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="fe8d8-138">String collection</span></span>|<span data-ttu-id="fe8d8-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-139">the associated app.</span></span> <span data-ttu-id="fe8d8-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe8d8-141">roleScopeTagIds</span></span>|<span data-ttu-id="fe8d8-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="fe8d8-142">String collection</span></span>|<span data-ttu-id="fe8d8-143">此应用程序配置实体范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="fe8d8-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe8d8-145">createdDateTime</span></span>|<span data-ttu-id="fe8d8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe8d8-146">DateTimeOffset</span></span>|<span data-ttu-id="fe8d8-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-147">DateTime the object was created.</span></span> <span data-ttu-id="fe8d8-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-149">description</span><span class="sxs-lookup"><span data-stu-id="fe8d8-149">description</span></span>|<span data-ttu-id="fe8d8-150">String</span><span class="sxs-lookup"><span data-stu-id="fe8d8-150">String</span></span>|<span data-ttu-id="fe8d8-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe8d8-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe8d8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fe8d8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe8d8-154">DateTimeOffset</span></span>|<span data-ttu-id="fe8d8-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-155">DateTime the object was last modified.</span></span> <span data-ttu-id="fe8d8-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-157">displayName</span><span class="sxs-lookup"><span data-stu-id="fe8d8-157">displayName</span></span>|<span data-ttu-id="fe8d8-158">String</span><span class="sxs-lookup"><span data-stu-id="fe8d8-158">String</span></span>|<span data-ttu-id="fe8d8-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe8d8-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-161">version</span><span class="sxs-lookup"><span data-stu-id="fe8d8-161">version</span></span>|<span data-ttu-id="fe8d8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="fe8d8-162">Int32</span></span>|<span data-ttu-id="fe8d8-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-163">Version of the device configuration.</span></span> <span data-ttu-id="fe8d8-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe8d8-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fe8d8-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="fe8d8-165">encodedSettingXml</span></span>|<span data-ttu-id="fe8d8-166">Binary</span><span class="sxs-lookup"><span data-stu-id="fe8d8-166">Binary</span></span>|<span data-ttu-id="fe8d8-167">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="fe8d8-168">settings</span><span class="sxs-lookup"><span data-stu-id="fe8d8-168">settings</span></span>|<span data-ttu-id="fe8d8-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe8d8-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="fe8d8-170">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="fe8d8-171">响应</span><span class="sxs-lookup"><span data-stu-id="fe8d8-171">Response</span></span>
<span data-ttu-id="fe8d8-172">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe8d8-173">示例</span><span class="sxs-lookup"><span data-stu-id="fe8d8-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe8d8-174">请求</span><span class="sxs-lookup"><span data-stu-id="fe8d8-174">Request</span></span>
<span data-ttu-id="fe8d8-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 660

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="fe8d8-176">响应</span><span class="sxs-lookup"><span data-stu-id="fe8d8-176">Response</span></span>
<span data-ttu-id="fe8d8-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe8d8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





