---
title: 创建 iosDeviceFeaturesConfiguration
description: 创建新的 iosDeviceFeaturesConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f032e8946729abf02bf832f1308d186d589f65a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747989"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="44eb9-103">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="44eb9-103">Create iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="44eb9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44eb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44eb9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44eb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44eb9-106">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44eb9-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44eb9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="44eb9-107">Prerequisites</span></span>
<span data-ttu-id="44eb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44eb9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="44eb9-110">Permission type</span></span>|<span data-ttu-id="44eb9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44eb9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44eb9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44eb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44eb9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44eb9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44eb9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44eb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44eb9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44eb9-115">Not supported.</span></span>|
|<span data-ttu-id="44eb9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="44eb9-116">Application</span></span>|<span data-ttu-id="44eb9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44eb9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44eb9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44eb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44eb9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="44eb9-119">Request headers</span></span>
|<span data-ttu-id="44eb9-120">标头</span><span class="sxs-lookup"><span data-stu-id="44eb9-120">Header</span></span>|<span data-ttu-id="44eb9-121">值</span><span class="sxs-lookup"><span data-stu-id="44eb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44eb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44eb9-122">Authorization</span></span>|<span data-ttu-id="44eb9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44eb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44eb9-124">接受</span><span class="sxs-lookup"><span data-stu-id="44eb9-124">Accept</span></span>|<span data-ttu-id="44eb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44eb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44eb9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="44eb9-126">Request body</span></span>
<span data-ttu-id="44eb9-127">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44eb9-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="44eb9-128">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44eb9-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="44eb9-129">属性</span><span class="sxs-lookup"><span data-stu-id="44eb9-129">Property</span></span>|<span data-ttu-id="44eb9-130">类型</span><span class="sxs-lookup"><span data-stu-id="44eb9-130">Type</span></span>|<span data-ttu-id="44eb9-131">说明</span><span class="sxs-lookup"><span data-stu-id="44eb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44eb9-132">id</span><span class="sxs-lookup"><span data-stu-id="44eb9-132">id</span></span>|<span data-ttu-id="44eb9-133">String</span><span class="sxs-lookup"><span data-stu-id="44eb9-133">String</span></span>|<span data-ttu-id="44eb9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="44eb9-134">Key of the entity.</span></span> <span data-ttu-id="44eb9-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44eb9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44eb9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44eb9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="44eb9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44eb9-137">DateTimeOffset</span></span>|<span data-ttu-id="44eb9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="44eb9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="44eb9-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44eb9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44eb9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44eb9-140">createdDateTime</span></span>|<span data-ttu-id="44eb9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44eb9-141">DateTimeOffset</span></span>|<span data-ttu-id="44eb9-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="44eb9-142">DateTime the object was created.</span></span> <span data-ttu-id="44eb9-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44eb9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44eb9-144">说明</span><span class="sxs-lookup"><span data-stu-id="44eb9-144">description</span></span>|<span data-ttu-id="44eb9-145">String</span><span class="sxs-lookup"><span data-stu-id="44eb9-145">String</span></span>|<span data-ttu-id="44eb9-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="44eb9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44eb9-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44eb9-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44eb9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="44eb9-148">displayName</span></span>|<span data-ttu-id="44eb9-149">String</span><span class="sxs-lookup"><span data-stu-id="44eb9-149">String</span></span>|<span data-ttu-id="44eb9-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="44eb9-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44eb9-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44eb9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44eb9-152">version</span><span class="sxs-lookup"><span data-stu-id="44eb9-152">version</span></span>|<span data-ttu-id="44eb9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="44eb9-153">Int32</span></span>|<span data-ttu-id="44eb9-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="44eb9-154">Version of the device configuration.</span></span> <span data-ttu-id="44eb9-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44eb9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44eb9-156">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="44eb9-156">assetTagTemplate</span></span>|<span data-ttu-id="44eb9-157">String</span><span class="sxs-lookup"><span data-stu-id="44eb9-157">String</span></span>|<span data-ttu-id="44eb9-158">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="44eb9-158">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="44eb9-159">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="44eb9-159">lockScreenFootnote</span></span>|<span data-ttu-id="44eb9-160">String</span><span class="sxs-lookup"><span data-stu-id="44eb9-160">String</span></span>|<span data-ttu-id="44eb9-161">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="44eb9-161">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="44eb9-162">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="44eb9-162">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="44eb9-163">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="44eb9-163">homeScreenDockIcons</span></span>|<span data-ttu-id="44eb9-164">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="44eb9-164">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="44eb9-165">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="44eb9-165">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="44eb9-166">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="44eb9-166">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="44eb9-167">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="44eb9-167">homeScreenPages</span></span>|<span data-ttu-id="44eb9-168">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="44eb9-168">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="44eb9-169">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="44eb9-169">A list of pages on the Home Screen.</span></span> <span data-ttu-id="44eb9-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="44eb9-170">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="44eb9-171">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="44eb9-171">notificationSettings</span></span>|<span data-ttu-id="44eb9-172">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="44eb9-172">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="44eb9-173">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="44eb9-173">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="44eb9-174">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="44eb9-174">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="44eb9-175">响应</span><span class="sxs-lookup"><span data-stu-id="44eb9-175">Response</span></span>
<span data-ttu-id="44eb9-176">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44eb9-176">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44eb9-177">示例</span><span class="sxs-lookup"><span data-stu-id="44eb9-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="44eb9-178">请求</span><span class="sxs-lookup"><span data-stu-id="44eb9-178">Request</span></span>
<span data-ttu-id="44eb9-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44eb9-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="44eb9-180">响应</span><span class="sxs-lookup"><span data-stu-id="44eb9-180">Response</span></span>
<span data-ttu-id="44eb9-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44eb9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```




