---
title: Update iosMobileAppConfiguration
description: 更新 iosMobileAppConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2119d146e4fa2cd64bc3aa39368d749993471811
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977707"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="06c65-103">Update iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="06c65-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="06c65-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06c65-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c65-105">更新 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06c65-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06c65-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="06c65-106">Prerequisites</span></span>
<span data-ttu-id="06c65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06c65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c65-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06c65-109">Permission type</span></span>|<span data-ttu-id="06c65-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06c65-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06c65-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06c65-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06c65-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c65-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06c65-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06c65-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06c65-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06c65-114">Not supported.</span></span>|
|<span data-ttu-id="06c65-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06c65-115">Application</span></span>|<span data-ttu-id="06c65-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06c65-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c65-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06c65-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06c65-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="06c65-118">Request headers</span></span>
|<span data-ttu-id="06c65-119">标头</span><span class="sxs-lookup"><span data-stu-id="06c65-119">Header</span></span>|<span data-ttu-id="06c65-120">值</span><span class="sxs-lookup"><span data-stu-id="06c65-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06c65-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c65-121">Authorization</span></span>|<span data-ttu-id="06c65-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06c65-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06c65-123">接受</span><span class="sxs-lookup"><span data-stu-id="06c65-123">Accept</span></span>|<span data-ttu-id="06c65-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06c65-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06c65-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="06c65-125">Request body</span></span>
<span data-ttu-id="06c65-126">在请求正文中，提供 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06c65-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="06c65-127">下表显示创建 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06c65-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="06c65-128">属性</span><span class="sxs-lookup"><span data-stu-id="06c65-128">Property</span></span>|<span data-ttu-id="06c65-129">类型</span><span class="sxs-lookup"><span data-stu-id="06c65-129">Type</span></span>|<span data-ttu-id="06c65-130">说明</span><span class="sxs-lookup"><span data-stu-id="06c65-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c65-131">id</span><span class="sxs-lookup"><span data-stu-id="06c65-131">id</span></span>|<span data-ttu-id="06c65-132">String</span><span class="sxs-lookup"><span data-stu-id="06c65-132">String</span></span>|<span data-ttu-id="06c65-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06c65-133">Key of the entity.</span></span> <span data-ttu-id="06c65-134">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="06c65-135">targetedMobileApps</span></span>|<span data-ttu-id="06c65-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="06c65-136">String collection</span></span>|<span data-ttu-id="06c65-137">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="06c65-137">the associated app.</span></span> <span data-ttu-id="06c65-138">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06c65-139">createdDateTime</span></span>|<span data-ttu-id="06c65-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c65-140">DateTimeOffset</span></span>|<span data-ttu-id="06c65-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06c65-141">DateTime the object was created.</span></span> <span data-ttu-id="06c65-142">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-143">description</span><span class="sxs-lookup"><span data-stu-id="06c65-143">description</span></span>|<span data-ttu-id="06c65-144">String</span><span class="sxs-lookup"><span data-stu-id="06c65-144">String</span></span>|<span data-ttu-id="06c65-145">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="06c65-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06c65-146">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06c65-147">lastModifiedDateTime</span></span>|<span data-ttu-id="06c65-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c65-148">DateTimeOffset</span></span>|<span data-ttu-id="06c65-149">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06c65-149">DateTime the object was last modified.</span></span> <span data-ttu-id="06c65-150">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-151">displayName</span><span class="sxs-lookup"><span data-stu-id="06c65-151">displayName</span></span>|<span data-ttu-id="06c65-152">String</span><span class="sxs-lookup"><span data-stu-id="06c65-152">String</span></span>|<span data-ttu-id="06c65-153">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="06c65-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06c65-154">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-155">version</span><span class="sxs-lookup"><span data-stu-id="06c65-155">version</span></span>|<span data-ttu-id="06c65-156">Int32</span><span class="sxs-lookup"><span data-stu-id="06c65-156">Int32</span></span>|<span data-ttu-id="06c65-157">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="06c65-157">Version of the device configuration.</span></span> <span data-ttu-id="06c65-158">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06c65-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="06c65-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="06c65-159">encodedSettingXml</span></span>|<span data-ttu-id="06c65-160">Binary</span><span class="sxs-lookup"><span data-stu-id="06c65-160">Binary</span></span>|<span data-ttu-id="06c65-161">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="06c65-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="06c65-162">settings</span><span class="sxs-lookup"><span data-stu-id="06c65-162">settings</span></span>|<span data-ttu-id="06c65-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06c65-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="06c65-164">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="06c65-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="06c65-165">响应</span><span class="sxs-lookup"><span data-stu-id="06c65-165">Response</span></span>
<span data-ttu-id="06c65-166">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06c65-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c65-167">示例</span><span class="sxs-lookup"><span data-stu-id="06c65-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="06c65-168">请求</span><span class="sxs-lookup"><span data-stu-id="06c65-168">Request</span></span>
<span data-ttu-id="06c65-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06c65-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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

### <a name="response"></a><span data-ttu-id="06c65-170">响应</span><span class="sxs-lookup"><span data-stu-id="06c65-170">Response</span></span>
<span data-ttu-id="06c65-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06c65-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
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



