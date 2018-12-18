---
title: 创建 iosDeviceFeaturesConfiguration
description: 创建新的 iosDeviceFeaturesConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 9467e42e16d88e0d1bfa02ea0996a8930d5d6cdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307418"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="f662e-103">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="f662e-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="f662e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f662e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f662e-105">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f662e-105">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f662e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f662e-106">Prerequisites</span></span>
<span data-ttu-id="f662e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f662e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f662e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f662e-109">Permission type</span></span>|<span data-ttu-id="f662e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f662e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f662e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f662e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f662e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f662e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f662e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f662e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f662e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f662e-114">Not supported.</span></span>|
|<span data-ttu-id="f662e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f662e-115">Application</span></span>|<span data-ttu-id="f662e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f662e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f662e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f662e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f662e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f662e-118">Request headers</span></span>
|<span data-ttu-id="f662e-119">标头</span><span class="sxs-lookup"><span data-stu-id="f662e-119">Header</span></span>|<span data-ttu-id="f662e-120">值</span><span class="sxs-lookup"><span data-stu-id="f662e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f662e-121">授权</span><span class="sxs-lookup"><span data-stu-id="f662e-121">Authorization</span></span>|<span data-ttu-id="f662e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f662e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f662e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f662e-123">Accept</span></span>|<span data-ttu-id="f662e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f662e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f662e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f662e-125">Request body</span></span>
<span data-ttu-id="f662e-126">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f662e-126">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="f662e-127">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f662e-127">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="f662e-128">属性</span><span class="sxs-lookup"><span data-stu-id="f662e-128">Property</span></span>|<span data-ttu-id="f662e-129">类型</span><span class="sxs-lookup"><span data-stu-id="f662e-129">Type</span></span>|<span data-ttu-id="f662e-130">说明</span><span class="sxs-lookup"><span data-stu-id="f662e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f662e-131">id</span><span class="sxs-lookup"><span data-stu-id="f662e-131">id</span></span>|<span data-ttu-id="f662e-132">String</span><span class="sxs-lookup"><span data-stu-id="f662e-132">String</span></span>|<span data-ttu-id="f662e-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f662e-133">Key of the entity.</span></span> <span data-ttu-id="f662e-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f662e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f662e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f662e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f662e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f662e-136">DateTimeOffset</span></span>|<span data-ttu-id="f662e-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f662e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="f662e-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f662e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f662e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f662e-139">createdDateTime</span></span>|<span data-ttu-id="f662e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f662e-140">DateTimeOffset</span></span>|<span data-ttu-id="f662e-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f662e-141">DateTime the object was created.</span></span> <span data-ttu-id="f662e-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f662e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f662e-143">description</span><span class="sxs-lookup"><span data-stu-id="f662e-143">description</span></span>|<span data-ttu-id="f662e-144">String</span><span class="sxs-lookup"><span data-stu-id="f662e-144">String</span></span>|<span data-ttu-id="f662e-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f662e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f662e-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f662e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f662e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f662e-147">displayName</span></span>|<span data-ttu-id="f662e-148">String</span><span class="sxs-lookup"><span data-stu-id="f662e-148">String</span></span>|<span data-ttu-id="f662e-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f662e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f662e-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f662e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f662e-151">version</span><span class="sxs-lookup"><span data-stu-id="f662e-151">version</span></span>|<span data-ttu-id="f662e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f662e-152">Int32</span></span>|<span data-ttu-id="f662e-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f662e-153">Version of the device configuration.</span></span> <span data-ttu-id="f662e-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f662e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f662e-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="f662e-155">assetTagTemplate</span></span>|<span data-ttu-id="f662e-156">String</span><span class="sxs-lookup"><span data-stu-id="f662e-156">String</span></span>|<span data-ttu-id="f662e-157">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="f662e-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="f662e-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="f662e-158">lockScreenFootnote</span></span>|<span data-ttu-id="f662e-159">String</span><span class="sxs-lookup"><span data-stu-id="f662e-159">String</span></span>|<span data-ttu-id="f662e-160">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="f662e-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="f662e-161">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="f662e-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="f662e-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="f662e-162">homeScreenDockIcons</span></span>|<span data-ttu-id="f662e-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f662e-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="f662e-164">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="f662e-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="f662e-165">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f662e-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f662e-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="f662e-166">homeScreenPages</span></span>|<span data-ttu-id="f662e-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f662e-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="f662e-168">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="f662e-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="f662e-169">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f662e-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f662e-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="f662e-170">notificationSettings</span></span>|<span data-ttu-id="f662e-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f662e-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="f662e-172">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f662e-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="f662e-173">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f662e-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f662e-174">响应</span><span class="sxs-lookup"><span data-stu-id="f662e-174">Response</span></span>
<span data-ttu-id="f662e-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f662e-175">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f662e-176">示例</span><span class="sxs-lookup"><span data-stu-id="f662e-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="f662e-177">请求</span><span class="sxs-lookup"><span data-stu-id="f662e-177">Request</span></span>
<span data-ttu-id="f662e-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f662e-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f662e-179">响应</span><span class="sxs-lookup"><span data-stu-id="f662e-179">Response</span></span>
<span data-ttu-id="f662e-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f662e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



