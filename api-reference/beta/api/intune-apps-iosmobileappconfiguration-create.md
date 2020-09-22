---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b21f5675bb2c3cbcd09e56036306e0358eefa11a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001111"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="862b3-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="862b3-103">Create iosMobileAppConfiguration</span></span>

<span data-ttu-id="862b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="862b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="862b3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="862b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="862b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="862b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="862b3-107">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="862b3-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="862b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="862b3-108">Prerequisites</span></span>
<span data-ttu-id="862b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="862b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="862b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="862b3-111">Permission type</span></span>|<span data-ttu-id="862b3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="862b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="862b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="862b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="862b3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="862b3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="862b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="862b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="862b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="862b3-116">Not supported.</span></span>|
|<span data-ttu-id="862b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="862b3-117">Application</span></span>|<span data-ttu-id="862b3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="862b3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="862b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="862b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="862b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="862b3-120">Request headers</span></span>
|<span data-ttu-id="862b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="862b3-121">Header</span></span>|<span data-ttu-id="862b3-122">值</span><span class="sxs-lookup"><span data-stu-id="862b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="862b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="862b3-123">Authorization</span></span>|<span data-ttu-id="862b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="862b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="862b3-125">接受</span><span class="sxs-lookup"><span data-stu-id="862b3-125">Accept</span></span>|<span data-ttu-id="862b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="862b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="862b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="862b3-127">Request body</span></span>
<span data-ttu-id="862b3-128">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="862b3-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="862b3-129">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="862b3-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="862b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="862b3-130">Property</span></span>|<span data-ttu-id="862b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="862b3-131">Type</span></span>|<span data-ttu-id="862b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="862b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="862b3-133">id</span><span class="sxs-lookup"><span data-stu-id="862b3-133">id</span></span>|<span data-ttu-id="862b3-134">String</span><span class="sxs-lookup"><span data-stu-id="862b3-134">String</span></span>|<span data-ttu-id="862b3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="862b3-135">Key of the entity.</span></span> <span data-ttu-id="862b3-136">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="862b3-137">targetedMobileApps</span></span>|<span data-ttu-id="862b3-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="862b3-138">String collection</span></span>|<span data-ttu-id="862b3-139">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="862b3-139">the associated app.</span></span> <span data-ttu-id="862b3-140">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="862b3-141">roleScopeTagIds</span></span>|<span data-ttu-id="862b3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="862b3-142">String collection</span></span>|<span data-ttu-id="862b3-143">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="862b3-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="862b3-144">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="862b3-145">createdDateTime</span></span>|<span data-ttu-id="862b3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862b3-146">DateTimeOffset</span></span>|<span data-ttu-id="862b3-147">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="862b3-147">DateTime the object was created.</span></span> <span data-ttu-id="862b3-148">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-149">description</span><span class="sxs-lookup"><span data-stu-id="862b3-149">description</span></span>|<span data-ttu-id="862b3-150">String</span><span class="sxs-lookup"><span data-stu-id="862b3-150">String</span></span>|<span data-ttu-id="862b3-151">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="862b3-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="862b3-152">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="862b3-153">lastModifiedDateTime</span></span>|<span data-ttu-id="862b3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="862b3-154">DateTimeOffset</span></span>|<span data-ttu-id="862b3-155">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="862b3-155">DateTime the object was last modified.</span></span> <span data-ttu-id="862b3-156">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-157">displayName</span><span class="sxs-lookup"><span data-stu-id="862b3-157">displayName</span></span>|<span data-ttu-id="862b3-158">String</span><span class="sxs-lookup"><span data-stu-id="862b3-158">String</span></span>|<span data-ttu-id="862b3-159">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="862b3-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="862b3-160">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-161">version</span><span class="sxs-lookup"><span data-stu-id="862b3-161">version</span></span>|<span data-ttu-id="862b3-162">Int32</span><span class="sxs-lookup"><span data-stu-id="862b3-162">Int32</span></span>|<span data-ttu-id="862b3-163">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="862b3-163">Version of the device configuration.</span></span> <span data-ttu-id="862b3-164">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="862b3-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="862b3-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="862b3-165">encodedSettingXml</span></span>|<span data-ttu-id="862b3-166">Binary</span><span class="sxs-lookup"><span data-stu-id="862b3-166">Binary</span></span>|<span data-ttu-id="862b3-167">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="862b3-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="862b3-168">settings</span><span class="sxs-lookup"><span data-stu-id="862b3-168">settings</span></span>|<span data-ttu-id="862b3-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="862b3-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="862b3-170">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="862b3-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="862b3-171">响应</span><span class="sxs-lookup"><span data-stu-id="862b3-171">Response</span></span>
<span data-ttu-id="862b3-172">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="862b3-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="862b3-173">示例</span><span class="sxs-lookup"><span data-stu-id="862b3-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="862b3-174">请求</span><span class="sxs-lookup"><span data-stu-id="862b3-174">Request</span></span>
<span data-ttu-id="862b3-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="862b3-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="862b3-176">响应</span><span class="sxs-lookup"><span data-stu-id="862b3-176">Response</span></span>
<span data-ttu-id="862b3-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="862b3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






