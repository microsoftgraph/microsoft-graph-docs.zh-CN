---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1274dec42b698a40a892dbc0f7a583aad2bfaa22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915093"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="1c457-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c457-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="1c457-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c457-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c457-105">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c457-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c457-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c457-106">Prerequisites</span></span>
<span data-ttu-id="1c457-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1c457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c457-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c457-109">Permission type</span></span>|<span data-ttu-id="1c457-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1c457-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c457-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c457-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c457-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c457-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c457-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c457-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c457-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c457-114">Not supported.</span></span>|
|<span data-ttu-id="1c457-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c457-115">Application</span></span>|<span data-ttu-id="1c457-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c457-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c457-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c457-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c457-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c457-118">Request headers</span></span>
|<span data-ttu-id="1c457-119">标头</span><span class="sxs-lookup"><span data-stu-id="1c457-119">Header</span></span>|<span data-ttu-id="1c457-120">值</span><span class="sxs-lookup"><span data-stu-id="1c457-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c457-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c457-121">Authorization</span></span>|<span data-ttu-id="1c457-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c457-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c457-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1c457-123">Accept</span></span>|<span data-ttu-id="1c457-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c457-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c457-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c457-125">Request body</span></span>
<span data-ttu-id="1c457-126">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c457-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="1c457-127">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1c457-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="1c457-128">属性</span><span class="sxs-lookup"><span data-stu-id="1c457-128">Property</span></span>|<span data-ttu-id="1c457-129">类型</span><span class="sxs-lookup"><span data-stu-id="1c457-129">Type</span></span>|<span data-ttu-id="1c457-130">说明</span><span class="sxs-lookup"><span data-stu-id="1c457-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c457-131">id</span><span class="sxs-lookup"><span data-stu-id="1c457-131">id</span></span>|<span data-ttu-id="1c457-132">String</span><span class="sxs-lookup"><span data-stu-id="1c457-132">String</span></span>|<span data-ttu-id="1c457-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1c457-133">Key of the entity.</span></span> <span data-ttu-id="1c457-134">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1c457-135">targetedMobileApps</span></span>|<span data-ttu-id="1c457-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="1c457-136">String collection</span></span>|<span data-ttu-id="1c457-137">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="1c457-137">the associated app.</span></span> <span data-ttu-id="1c457-138">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c457-139">createdDateTime</span></span>|<span data-ttu-id="1c457-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c457-140">DateTimeOffset</span></span>|<span data-ttu-id="1c457-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c457-141">DateTime the object was created.</span></span> <span data-ttu-id="1c457-142">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-143">description</span><span class="sxs-lookup"><span data-stu-id="1c457-143">description</span></span>|<span data-ttu-id="1c457-144">String</span><span class="sxs-lookup"><span data-stu-id="1c457-144">String</span></span>|<span data-ttu-id="1c457-145">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="1c457-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c457-146">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c457-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1c457-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c457-148">DateTimeOffset</span></span>|<span data-ttu-id="1c457-149">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c457-149">DateTime the object was last modified.</span></span> <span data-ttu-id="1c457-150">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-151">displayName</span><span class="sxs-lookup"><span data-stu-id="1c457-151">displayName</span></span>|<span data-ttu-id="1c457-152">String</span><span class="sxs-lookup"><span data-stu-id="1c457-152">String</span></span>|<span data-ttu-id="1c457-153">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="1c457-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c457-154">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-155">version</span><span class="sxs-lookup"><span data-stu-id="1c457-155">version</span></span>|<span data-ttu-id="1c457-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1c457-156">Int32</span></span>|<span data-ttu-id="1c457-157">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1c457-157">Version of the device configuration.</span></span> <span data-ttu-id="1c457-158">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c457-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1c457-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="1c457-159">encodedSettingXml</span></span>|<span data-ttu-id="1c457-160">Binary</span><span class="sxs-lookup"><span data-stu-id="1c457-160">Binary</span></span>|<span data-ttu-id="1c457-161">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="1c457-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="1c457-162">settings</span><span class="sxs-lookup"><span data-stu-id="1c457-162">settings</span></span>|<span data-ttu-id="1c457-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c457-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="1c457-164">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="1c457-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="1c457-165">响应</span><span class="sxs-lookup"><span data-stu-id="1c457-165">Response</span></span>
<span data-ttu-id="1c457-166">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c457-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c457-167">示例</span><span class="sxs-lookup"><span data-stu-id="1c457-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c457-168">请求</span><span class="sxs-lookup"><span data-stu-id="1c457-168">Request</span></span>
<span data-ttu-id="1c457-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c457-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c457-170">响应</span><span class="sxs-lookup"><span data-stu-id="1c457-170">Response</span></span>
<span data-ttu-id="1c457-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c457-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



