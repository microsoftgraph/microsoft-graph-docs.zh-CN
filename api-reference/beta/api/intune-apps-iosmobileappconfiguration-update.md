---
title: Update iosMobileAppConfiguration
description: 更新 iosMobileAppConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aeb7ab2fc660b22c229342ddb78a7caa5e12dc70
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409900"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="ab3f9-103">Update iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab3f9-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="ab3f9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab3f9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab3f9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab3f9-107">更新 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-107">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab3f9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab3f9-108">Prerequisites</span></span>
<span data-ttu-id="ab3f9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ab3f9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab3f9-111">Permission type</span></span>|<span data-ttu-id="ab3f9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab3f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab3f9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab3f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab3f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3f9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab3f9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab3f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab3f9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-116">Not supported.</span></span>|
|<span data-ttu-id="ab3f9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab3f9-117">Application</span></span>|<span data-ttu-id="ab3f9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab3f9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab3f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab3f9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab3f9-120">Request headers</span></span>
|<span data-ttu-id="ab3f9-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab3f9-121">Header</span></span>|<span data-ttu-id="ab3f9-122">值</span><span class="sxs-lookup"><span data-stu-id="ab3f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab3f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab3f9-123">Authorization</span></span>|<span data-ttu-id="ab3f9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab3f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab3f9-125">Accept</span></span>|<span data-ttu-id="ab3f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab3f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab3f9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab3f9-127">Request body</span></span>
<span data-ttu-id="ab3f9-128">在请求正文中，提供 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-128">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="ab3f9-129">下表显示创建 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-129">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="ab3f9-130">属性</span><span class="sxs-lookup"><span data-stu-id="ab3f9-130">Property</span></span>|<span data-ttu-id="ab3f9-131">类型</span><span class="sxs-lookup"><span data-stu-id="ab3f9-131">Type</span></span>|<span data-ttu-id="ab3f9-132">说明</span><span class="sxs-lookup"><span data-stu-id="ab3f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab3f9-133">id</span><span class="sxs-lookup"><span data-stu-id="ab3f9-133">id</span></span>|<span data-ttu-id="ab3f9-134">String</span><span class="sxs-lookup"><span data-stu-id="ab3f9-134">String</span></span>|<span data-ttu-id="ab3f9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-135">Key of the entity.</span></span> <span data-ttu-id="ab3f9-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ab3f9-137">targetedMobileApps</span></span>|<span data-ttu-id="ab3f9-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="ab3f9-138">String collection</span></span>|<span data-ttu-id="ab3f9-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-139">the associated app.</span></span> <span data-ttu-id="ab3f9-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab3f9-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab3f9-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="ab3f9-142">String collection</span></span>|<span data-ttu-id="ab3f9-143">此应用程序配置实体范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="ab3f9-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3f9-145">createdDateTime</span></span>|<span data-ttu-id="ab3f9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab3f9-146">DateTimeOffset</span></span>|<span data-ttu-id="ab3f9-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-147">DateTime the object was created.</span></span> <span data-ttu-id="ab3f9-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-149">description</span><span class="sxs-lookup"><span data-stu-id="ab3f9-149">description</span></span>|<span data-ttu-id="ab3f9-150">String</span><span class="sxs-lookup"><span data-stu-id="ab3f9-150">String</span></span>|<span data-ttu-id="ab3f9-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab3f9-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3f9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ab3f9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab3f9-154">DateTimeOffset</span></span>|<span data-ttu-id="ab3f9-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-155">DateTime the object was last modified.</span></span> <span data-ttu-id="ab3f9-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-157">displayName</span><span class="sxs-lookup"><span data-stu-id="ab3f9-157">displayName</span></span>|<span data-ttu-id="ab3f9-158">String</span><span class="sxs-lookup"><span data-stu-id="ab3f9-158">String</span></span>|<span data-ttu-id="ab3f9-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab3f9-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-161">version</span><span class="sxs-lookup"><span data-stu-id="ab3f9-161">version</span></span>|<span data-ttu-id="ab3f9-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ab3f9-162">Int32</span></span>|<span data-ttu-id="ab3f9-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-163">Version of the device configuration.</span></span> <span data-ttu-id="ab3f9-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab3f9-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ab3f9-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="ab3f9-165">encodedSettingXml</span></span>|<span data-ttu-id="ab3f9-166">Binary</span><span class="sxs-lookup"><span data-stu-id="ab3f9-166">Binary</span></span>|<span data-ttu-id="ab3f9-167">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="ab3f9-168">settings</span><span class="sxs-lookup"><span data-stu-id="ab3f9-168">settings</span></span>|<span data-ttu-id="ab3f9-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab3f9-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="ab3f9-170">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="ab3f9-171">响应</span><span class="sxs-lookup"><span data-stu-id="ab3f9-171">Response</span></span>
<span data-ttu-id="ab3f9-172">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-172">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab3f9-173">示例</span><span class="sxs-lookup"><span data-stu-id="ab3f9-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab3f9-174">请求</span><span class="sxs-lookup"><span data-stu-id="ab3f9-174">Request</span></span>
<span data-ttu-id="ab3f9-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ab3f9-176">响应</span><span class="sxs-lookup"><span data-stu-id="ab3f9-176">Response</span></span>
<span data-ttu-id="ab3f9-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab3f9-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




