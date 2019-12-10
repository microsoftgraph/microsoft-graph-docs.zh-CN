---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e6fbac50a529a165483858dfd7c0059da6876f9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39925835"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="61b31-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="61b31-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="61b31-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="61b31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61b31-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61b31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b31-106">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61b31-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61b31-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="61b31-107">Prerequisites</span></span>
<span data-ttu-id="61b31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61b31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61b31-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61b31-110">Permission type</span></span>|<span data-ttu-id="61b31-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="61b31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61b31-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61b31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61b31-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61b31-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61b31-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61b31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61b31-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61b31-115">Not supported.</span></span>|
|<span data-ttu-id="61b31-116">Application</span><span class="sxs-lookup"><span data-stu-id="61b31-116">Application</span></span>|<span data-ttu-id="61b31-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61b31-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61b31-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61b31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="61b31-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="61b31-119">Request headers</span></span>
|<span data-ttu-id="61b31-120">标头</span><span class="sxs-lookup"><span data-stu-id="61b31-120">Header</span></span>|<span data-ttu-id="61b31-121">值</span><span class="sxs-lookup"><span data-stu-id="61b31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61b31-122">授权</span><span class="sxs-lookup"><span data-stu-id="61b31-122">Authorization</span></span>|<span data-ttu-id="61b31-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="61b31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61b31-124">接受</span><span class="sxs-lookup"><span data-stu-id="61b31-124">Accept</span></span>|<span data-ttu-id="61b31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61b31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61b31-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="61b31-126">Request body</span></span>
<span data-ttu-id="61b31-127">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61b31-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="61b31-128">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="61b31-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="61b31-129">属性</span><span class="sxs-lookup"><span data-stu-id="61b31-129">Property</span></span>|<span data-ttu-id="61b31-130">类型</span><span class="sxs-lookup"><span data-stu-id="61b31-130">Type</span></span>|<span data-ttu-id="61b31-131">说明</span><span class="sxs-lookup"><span data-stu-id="61b31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b31-132">id</span><span class="sxs-lookup"><span data-stu-id="61b31-132">id</span></span>|<span data-ttu-id="61b31-133">字符串</span><span class="sxs-lookup"><span data-stu-id="61b31-133">String</span></span>|<span data-ttu-id="61b31-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="61b31-134">Key of the entity.</span></span> <span data-ttu-id="61b31-135">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="61b31-136">targetedMobileApps</span></span>|<span data-ttu-id="61b31-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="61b31-137">String collection</span></span>|<span data-ttu-id="61b31-138">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="61b31-138">the associated app.</span></span> <span data-ttu-id="61b31-139">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61b31-140">roleScopeTagIds</span></span>|<span data-ttu-id="61b31-141">String collection</span><span class="sxs-lookup"><span data-stu-id="61b31-141">String collection</span></span>|<span data-ttu-id="61b31-142">此应用配置实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="61b31-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="61b31-143">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61b31-144">createdDateTime</span></span>|<span data-ttu-id="61b31-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61b31-145">DateTimeOffset</span></span>|<span data-ttu-id="61b31-146">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="61b31-146">DateTime the object was created.</span></span> <span data-ttu-id="61b31-147">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-148">说明</span><span class="sxs-lookup"><span data-stu-id="61b31-148">description</span></span>|<span data-ttu-id="61b31-149">String</span><span class="sxs-lookup"><span data-stu-id="61b31-149">String</span></span>|<span data-ttu-id="61b31-150">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="61b31-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="61b31-151">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61b31-152">lastModifiedDateTime</span></span>|<span data-ttu-id="61b31-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61b31-153">DateTimeOffset</span></span>|<span data-ttu-id="61b31-154">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="61b31-154">DateTime the object was last modified.</span></span> <span data-ttu-id="61b31-155">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-156">displayName</span><span class="sxs-lookup"><span data-stu-id="61b31-156">displayName</span></span>|<span data-ttu-id="61b31-157">String</span><span class="sxs-lookup"><span data-stu-id="61b31-157">String</span></span>|<span data-ttu-id="61b31-158">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="61b31-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="61b31-159">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-160">version</span><span class="sxs-lookup"><span data-stu-id="61b31-160">version</span></span>|<span data-ttu-id="61b31-161">Int32</span><span class="sxs-lookup"><span data-stu-id="61b31-161">Int32</span></span>|<span data-ttu-id="61b31-162">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="61b31-162">Version of the device configuration.</span></span> <span data-ttu-id="61b31-163">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61b31-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="61b31-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="61b31-164">encodedSettingXml</span></span>|<span data-ttu-id="61b31-165">Binary</span><span class="sxs-lookup"><span data-stu-id="61b31-165">Binary</span></span>|<span data-ttu-id="61b31-166">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="61b31-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="61b31-167">settings</span><span class="sxs-lookup"><span data-stu-id="61b31-167">settings</span></span>|<span data-ttu-id="61b31-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61b31-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="61b31-169">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="61b31-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="61b31-170">响应</span><span class="sxs-lookup"><span data-stu-id="61b31-170">Response</span></span>
<span data-ttu-id="61b31-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61b31-171">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61b31-172">示例</span><span class="sxs-lookup"><span data-stu-id="61b31-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="61b31-173">请求</span><span class="sxs-lookup"><span data-stu-id="61b31-173">Request</span></span>
<span data-ttu-id="61b31-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61b31-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61b31-175">响应</span><span class="sxs-lookup"><span data-stu-id="61b31-175">Response</span></span>
<span data-ttu-id="61b31-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61b31-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





