---
title: 创建 iosMobileAppConfiguration
description: 创建新的 iosMobileAppConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d5ada7a620a131e17a3403ad8c30b52ca4ab5c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577320"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="c7e2b-103">创建 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7e2b-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="c7e2b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e2b-105">创建新的 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7e2b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7e2b-106">Prerequisites</span></span>
<span data-ttu-id="c7e2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e2b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7e2b-109">Permission type</span></span>|<span data-ttu-id="c7e2b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7e2b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7e2b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7e2b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7e2b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e2b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7e2b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7e2b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7e2b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-114">Not supported.</span></span>|
|<span data-ttu-id="c7e2b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7e2b-115">Application</span></span>|<span data-ttu-id="c7e2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7e2b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7e2b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7e2b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7e2b-118">Request headers</span></span>
|<span data-ttu-id="c7e2b-119">标头</span><span class="sxs-lookup"><span data-stu-id="c7e2b-119">Header</span></span>|<span data-ttu-id="c7e2b-120">值</span><span class="sxs-lookup"><span data-stu-id="c7e2b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7e2b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7e2b-121">Authorization</span></span>|<span data-ttu-id="c7e2b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7e2b-123">接受</span><span class="sxs-lookup"><span data-stu-id="c7e2b-123">Accept</span></span>|<span data-ttu-id="c7e2b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e2b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e2b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7e2b-125">Request body</span></span>
<span data-ttu-id="c7e2b-126">在请求正文中，提供 iosMobileAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="c7e2b-127">下表显示创建 iosMobileAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="c7e2b-128">属性</span><span class="sxs-lookup"><span data-stu-id="c7e2b-128">Property</span></span>|<span data-ttu-id="c7e2b-129">类型</span><span class="sxs-lookup"><span data-stu-id="c7e2b-129">Type</span></span>|<span data-ttu-id="c7e2b-130">说明</span><span class="sxs-lookup"><span data-stu-id="c7e2b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e2b-131">id</span><span class="sxs-lookup"><span data-stu-id="c7e2b-131">id</span></span>|<span data-ttu-id="c7e2b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c7e2b-132">String</span></span>|<span data-ttu-id="c7e2b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-133">Key of the entity.</span></span> <span data-ttu-id="c7e2b-134">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c7e2b-135">targetedMobileApps</span></span>|<span data-ttu-id="c7e2b-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="c7e2b-136">String collection</span></span>|<span data-ttu-id="c7e2b-137">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-137">the associated app.</span></span> <span data-ttu-id="c7e2b-138">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7e2b-139">createdDateTime</span></span>|<span data-ttu-id="c7e2b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7e2b-140">DateTimeOffset</span></span>|<span data-ttu-id="c7e2b-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-141">DateTime the object was created.</span></span> <span data-ttu-id="c7e2b-142">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-143">说明</span><span class="sxs-lookup"><span data-stu-id="c7e2b-143">description</span></span>|<span data-ttu-id="c7e2b-144">String</span><span class="sxs-lookup"><span data-stu-id="c7e2b-144">String</span></span>|<span data-ttu-id="c7e2b-145">管理员提供的设备配置说明。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7e2b-146">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7e2b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="c7e2b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7e2b-148">DateTimeOffset</span></span>|<span data-ttu-id="c7e2b-149">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-149">DateTime the object was last modified.</span></span> <span data-ttu-id="c7e2b-150">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-151">displayName</span><span class="sxs-lookup"><span data-stu-id="c7e2b-151">displayName</span></span>|<span data-ttu-id="c7e2b-152">String</span><span class="sxs-lookup"><span data-stu-id="c7e2b-152">String</span></span>|<span data-ttu-id="c7e2b-153">管理员提供的设备配置名称。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7e2b-154">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-155">version</span><span class="sxs-lookup"><span data-stu-id="c7e2b-155">version</span></span>|<span data-ttu-id="c7e2b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c7e2b-156">Int32</span></span>|<span data-ttu-id="c7e2b-157">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-157">Version of the device configuration.</span></span> <span data-ttu-id="c7e2b-158">继承自 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7e2b-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c7e2b-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="c7e2b-159">encodedSettingXml</span></span>|<span data-ttu-id="c7e2b-160">Binary</span><span class="sxs-lookup"><span data-stu-id="c7e2b-160">Binary</span></span>|<span data-ttu-id="c7e2b-161">mdm 应用配置 Base64 二进制。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="c7e2b-162">settings</span><span class="sxs-lookup"><span data-stu-id="c7e2b-162">settings</span></span>|<span data-ttu-id="c7e2b-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7e2b-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="c7e2b-164">应用配置设置项。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="c7e2b-165">响应</span><span class="sxs-lookup"><span data-stu-id="c7e2b-165">Response</span></span>
<span data-ttu-id="c7e2b-166">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e2b-167">示例</span><span class="sxs-lookup"><span data-stu-id="c7e2b-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7e2b-168">请求</span><span class="sxs-lookup"><span data-stu-id="c7e2b-168">Request</span></span>
<span data-ttu-id="c7e2b-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7e2b-170">响应</span><span class="sxs-lookup"><span data-stu-id="c7e2b-170">Response</span></span>
<span data-ttu-id="c7e2b-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7e2b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



