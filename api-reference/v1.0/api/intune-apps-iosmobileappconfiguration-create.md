---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa162d832c0994cc4410732f3c69016a5252d138
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757386"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="28c05-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="28c05-103">Create iosMobileAppConfiguration</span></span>

<span data-ttu-id="28c05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28c05-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28c05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c05-106">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28c05-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28c05-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="28c05-107">Prerequisites</span></span>
<span data-ttu-id="28c05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28c05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c05-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28c05-110">Permission type</span></span>|<span data-ttu-id="28c05-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28c05-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28c05-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28c05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28c05-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c05-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28c05-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28c05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28c05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28c05-115">Not supported.</span></span>|
|<span data-ttu-id="28c05-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28c05-116">Application</span></span>|<span data-ttu-id="28c05-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c05-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28c05-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28c05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="28c05-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28c05-119">Request headers</span></span>
|<span data-ttu-id="28c05-120">标头</span><span class="sxs-lookup"><span data-stu-id="28c05-120">Header</span></span>|<span data-ttu-id="28c05-121">值</span><span class="sxs-lookup"><span data-stu-id="28c05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28c05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28c05-122">Authorization</span></span>|<span data-ttu-id="28c05-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28c05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28c05-124">接受</span><span class="sxs-lookup"><span data-stu-id="28c05-124">Accept</span></span>|<span data-ttu-id="28c05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28c05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28c05-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28c05-126">Request body</span></span>
<span data-ttu-id="28c05-127">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28c05-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="28c05-128">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28c05-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="28c05-129">属性</span><span class="sxs-lookup"><span data-stu-id="28c05-129">Property</span></span>|<span data-ttu-id="28c05-130">类型</span><span class="sxs-lookup"><span data-stu-id="28c05-130">Type</span></span>|<span data-ttu-id="28c05-131">说明</span><span class="sxs-lookup"><span data-stu-id="28c05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c05-132">id</span><span class="sxs-lookup"><span data-stu-id="28c05-132">id</span></span>|<span data-ttu-id="28c05-133">String</span><span class="sxs-lookup"><span data-stu-id="28c05-133">String</span></span>|<span data-ttu-id="28c05-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28c05-134">Key of the entity.</span></span> <span data-ttu-id="28c05-135">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="28c05-136">targetedMobileApps</span></span>|<span data-ttu-id="28c05-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="28c05-137">String collection</span></span>|<span data-ttu-id="28c05-138">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="28c05-138">the associated app.</span></span> <span data-ttu-id="28c05-139">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28c05-140">createdDateTime</span></span>|<span data-ttu-id="28c05-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28c05-141">DateTimeOffset</span></span>|<span data-ttu-id="28c05-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="28c05-142">DateTime the object was created.</span></span> <span data-ttu-id="28c05-143">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-144">description</span><span class="sxs-lookup"><span data-stu-id="28c05-144">description</span></span>|<span data-ttu-id="28c05-145">String</span><span class="sxs-lookup"><span data-stu-id="28c05-145">String</span></span>|<span data-ttu-id="28c05-146">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="28c05-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28c05-147">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28c05-148">lastModifiedDateTime</span></span>|<span data-ttu-id="28c05-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28c05-149">DateTimeOffset</span></span>|<span data-ttu-id="28c05-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="28c05-150">DateTime the object was last modified.</span></span> <span data-ttu-id="28c05-151">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-152">displayName</span><span class="sxs-lookup"><span data-stu-id="28c05-152">displayName</span></span>|<span data-ttu-id="28c05-153">String</span><span class="sxs-lookup"><span data-stu-id="28c05-153">String</span></span>|<span data-ttu-id="28c05-154">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="28c05-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28c05-155">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-156">version</span><span class="sxs-lookup"><span data-stu-id="28c05-156">version</span></span>|<span data-ttu-id="28c05-157">Int32</span><span class="sxs-lookup"><span data-stu-id="28c05-157">Int32</span></span>|<span data-ttu-id="28c05-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="28c05-158">Version of the device configuration.</span></span> <span data-ttu-id="28c05-159">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28c05-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="28c05-160">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="28c05-160">encodedSettingXml</span></span>|<span data-ttu-id="28c05-161">Binary</span><span class="sxs-lookup"><span data-stu-id="28c05-161">Binary</span></span>|<span data-ttu-id="28c05-162">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="28c05-162">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="28c05-163">settings</span><span class="sxs-lookup"><span data-stu-id="28c05-163">settings</span></span>|<span data-ttu-id="28c05-164">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28c05-164">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="28c05-165">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="28c05-165">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="28c05-166">响应</span><span class="sxs-lookup"><span data-stu-id="28c05-166">Response</span></span>
<span data-ttu-id="28c05-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28c05-167">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28c05-168">示例</span><span class="sxs-lookup"><span data-stu-id="28c05-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="28c05-169">请求</span><span class="sxs-lookup"><span data-stu-id="28c05-169">Request</span></span>
<span data-ttu-id="28c05-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28c05-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="28c05-171">响应</span><span class="sxs-lookup"><span data-stu-id="28c05-171">Response</span></span>
<span data-ttu-id="28c05-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28c05-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




