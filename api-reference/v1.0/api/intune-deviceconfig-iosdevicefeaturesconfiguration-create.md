---
title: 创建 iosDeviceFeaturesConfiguration
description: 创建新的 iosDeviceFeaturesConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2be3450704898896e9fe1018da5dbd1212c442d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578118"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="6ce87-103">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ce87-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6ce87-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ce87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce87-105">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ce87-105">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ce87-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ce87-106">Prerequisites</span></span>
<span data-ttu-id="6ce87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ce87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce87-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ce87-109">Permission type</span></span>|<span data-ttu-id="6ce87-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6ce87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce87-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ce87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce87-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce87-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce87-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ce87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce87-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ce87-114">Not supported.</span></span>|
|<span data-ttu-id="6ce87-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ce87-115">Application</span></span>|<span data-ttu-id="6ce87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ce87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce87-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ce87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6ce87-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ce87-118">Request headers</span></span>
|<span data-ttu-id="6ce87-119">标头</span><span class="sxs-lookup"><span data-stu-id="6ce87-119">Header</span></span>|<span data-ttu-id="6ce87-120">值</span><span class="sxs-lookup"><span data-stu-id="6ce87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ce87-121">Authorization</span></span>|<span data-ttu-id="6ce87-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ce87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce87-123">接受</span><span class="sxs-lookup"><span data-stu-id="6ce87-123">Accept</span></span>|<span data-ttu-id="6ce87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce87-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ce87-125">Request body</span></span>
<span data-ttu-id="6ce87-126">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ce87-126">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="6ce87-127">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6ce87-127">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="6ce87-128">属性</span><span class="sxs-lookup"><span data-stu-id="6ce87-128">Property</span></span>|<span data-ttu-id="6ce87-129">类型</span><span class="sxs-lookup"><span data-stu-id="6ce87-129">Type</span></span>|<span data-ttu-id="6ce87-130">说明</span><span class="sxs-lookup"><span data-stu-id="6ce87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce87-131">id</span><span class="sxs-lookup"><span data-stu-id="6ce87-131">id</span></span>|<span data-ttu-id="6ce87-132">字符串</span><span class="sxs-lookup"><span data-stu-id="6ce87-132">String</span></span>|<span data-ttu-id="6ce87-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6ce87-133">Key of the entity.</span></span> <span data-ttu-id="6ce87-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ce87-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ce87-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce87-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6ce87-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce87-136">DateTimeOffset</span></span>|<span data-ttu-id="6ce87-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6ce87-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6ce87-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ce87-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ce87-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce87-139">createdDateTime</span></span>|<span data-ttu-id="6ce87-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce87-140">DateTimeOffset</span></span>|<span data-ttu-id="6ce87-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6ce87-141">DateTime the object was created.</span></span> <span data-ttu-id="6ce87-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ce87-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ce87-143">说明</span><span class="sxs-lookup"><span data-stu-id="6ce87-143">description</span></span>|<span data-ttu-id="6ce87-144">String</span><span class="sxs-lookup"><span data-stu-id="6ce87-144">String</span></span>|<span data-ttu-id="6ce87-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6ce87-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ce87-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ce87-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ce87-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6ce87-147">displayName</span></span>|<span data-ttu-id="6ce87-148">字符串</span><span class="sxs-lookup"><span data-stu-id="6ce87-148">String</span></span>|<span data-ttu-id="6ce87-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6ce87-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ce87-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ce87-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ce87-151">version</span><span class="sxs-lookup"><span data-stu-id="6ce87-151">version</span></span>|<span data-ttu-id="6ce87-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6ce87-152">Int32</span></span>|<span data-ttu-id="6ce87-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6ce87-153">Version of the device configuration.</span></span> <span data-ttu-id="6ce87-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ce87-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ce87-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="6ce87-155">assetTagTemplate</span></span>|<span data-ttu-id="6ce87-156">String</span><span class="sxs-lookup"><span data-stu-id="6ce87-156">String</span></span>|<span data-ttu-id="6ce87-157">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="6ce87-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="6ce87-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="6ce87-158">lockScreenFootnote</span></span>|<span data-ttu-id="6ce87-159">String</span><span class="sxs-lookup"><span data-stu-id="6ce87-159">String</span></span>|<span data-ttu-id="6ce87-160">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="6ce87-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="6ce87-161">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="6ce87-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="6ce87-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="6ce87-162">homeScreenDockIcons</span></span>|<span data-ttu-id="6ce87-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ce87-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="6ce87-164">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="6ce87-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="6ce87-165">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6ce87-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ce87-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="6ce87-166">homeScreenPages</span></span>|<span data-ttu-id="6ce87-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ce87-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="6ce87-168">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="6ce87-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="6ce87-169">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6ce87-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ce87-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="6ce87-170">notificationSettings</span></span>|<span data-ttu-id="6ce87-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ce87-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="6ce87-172">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="6ce87-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="6ce87-173">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6ce87-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6ce87-174">响应</span><span class="sxs-lookup"><span data-stu-id="6ce87-174">Response</span></span>
<span data-ttu-id="6ce87-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ce87-175">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce87-176">示例</span><span class="sxs-lookup"><span data-stu-id="6ce87-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ce87-177">请求</span><span class="sxs-lookup"><span data-stu-id="6ce87-177">Request</span></span>
<span data-ttu-id="6ce87-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ce87-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ce87-179">响应</span><span class="sxs-lookup"><span data-stu-id="6ce87-179">Response</span></span>
<span data-ttu-id="6ce87-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ce87-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



