---
title: 创建 iosDeviceFeaturesConfiguration
description: 创建新的 iosDeviceFeaturesConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f10bc7b7027b534a24f4a8f52ddbdd0499579f28
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785753"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="8ed38-103">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ed38-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8ed38-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ed38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ed38-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ed38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ed38-106">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ed38-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ed38-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ed38-107">Prerequisites</span></span>
<span data-ttu-id="8ed38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ed38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed38-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ed38-110">Permission type</span></span>|<span data-ttu-id="8ed38-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8ed38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ed38-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ed38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ed38-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed38-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ed38-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ed38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ed38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ed38-115">Not supported.</span></span>|
|<span data-ttu-id="8ed38-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ed38-116">Application</span></span>|<span data-ttu-id="8ed38-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ed38-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ed38-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ed38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ed38-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ed38-119">Request headers</span></span>
|<span data-ttu-id="8ed38-120">标头</span><span class="sxs-lookup"><span data-stu-id="8ed38-120">Header</span></span>|<span data-ttu-id="8ed38-121">值</span><span class="sxs-lookup"><span data-stu-id="8ed38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ed38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ed38-122">Authorization</span></span>|<span data-ttu-id="8ed38-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ed38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ed38-124">接受</span><span class="sxs-lookup"><span data-stu-id="8ed38-124">Accept</span></span>|<span data-ttu-id="8ed38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ed38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ed38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ed38-126">Request body</span></span>
<span data-ttu-id="8ed38-127">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ed38-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="8ed38-128">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ed38-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="8ed38-129">属性</span><span class="sxs-lookup"><span data-stu-id="8ed38-129">Property</span></span>|<span data-ttu-id="8ed38-130">类型</span><span class="sxs-lookup"><span data-stu-id="8ed38-130">Type</span></span>|<span data-ttu-id="8ed38-131">说明</span><span class="sxs-lookup"><span data-stu-id="8ed38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ed38-132">id</span><span class="sxs-lookup"><span data-stu-id="8ed38-132">id</span></span>|<span data-ttu-id="8ed38-133">String</span><span class="sxs-lookup"><span data-stu-id="8ed38-133">String</span></span>|<span data-ttu-id="8ed38-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8ed38-134">Key of the entity.</span></span> <span data-ttu-id="8ed38-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed38-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8ed38-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ed38-137">DateTimeOffset</span></span>|<span data-ttu-id="8ed38-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ed38-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8ed38-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ed38-140">roleScopeTagIds</span></span>|<span data-ttu-id="8ed38-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="8ed38-141">String collection</span></span>|<span data-ttu-id="8ed38-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8ed38-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ed38-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ed38-144">supportsScopeTags</span></span>|<span data-ttu-id="8ed38-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="8ed38-145">Boolean</span></span>|<span data-ttu-id="8ed38-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8ed38-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ed38-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8ed38-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ed38-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8ed38-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ed38-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8ed38-149">This property is read-only.</span></span> <span data-ttu-id="8ed38-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed38-151">createdDateTime</span></span>|<span data-ttu-id="8ed38-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ed38-152">DateTimeOffset</span></span>|<span data-ttu-id="8ed38-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ed38-153">DateTime the object was created.</span></span> <span data-ttu-id="8ed38-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-155">description</span><span class="sxs-lookup"><span data-stu-id="8ed38-155">description</span></span>|<span data-ttu-id="8ed38-156">String</span><span class="sxs-lookup"><span data-stu-id="8ed38-156">String</span></span>|<span data-ttu-id="8ed38-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8ed38-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ed38-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8ed38-159">displayName</span></span>|<span data-ttu-id="8ed38-160">String</span><span class="sxs-lookup"><span data-stu-id="8ed38-160">String</span></span>|<span data-ttu-id="8ed38-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8ed38-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ed38-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-163">version</span><span class="sxs-lookup"><span data-stu-id="8ed38-163">version</span></span>|<span data-ttu-id="8ed38-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8ed38-164">Int32</span></span>|<span data-ttu-id="8ed38-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8ed38-165">Version of the device configuration.</span></span> <span data-ttu-id="8ed38-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ed38-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="8ed38-167">airPrintDestinations</span></span>|<span data-ttu-id="8ed38-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="8ed38-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="8ed38-169">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="8ed38-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="8ed38-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8ed38-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8ed38-171">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="8ed38-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="8ed38-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="8ed38-172">assetTagTemplate</span></span>|<span data-ttu-id="8ed38-173">String</span><span class="sxs-lookup"><span data-stu-id="8ed38-173">String</span></span>|<span data-ttu-id="8ed38-174">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="8ed38-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="8ed38-175">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="8ed38-175">contentFilterSettings</span></span>|[<span data-ttu-id="8ed38-176">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="8ed38-176">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="8ed38-177">获取或设置 iOS Web 内容筛选器设置 (仅限受监督模式)</span><span class="sxs-lookup"><span data-stu-id="8ed38-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="8ed38-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="8ed38-178">lockScreenFootnote</span></span>|<span data-ttu-id="8ed38-179">String</span><span class="sxs-lookup"><span data-stu-id="8ed38-179">String</span></span>|<span data-ttu-id="8ed38-180">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="8ed38-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="8ed38-181">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="8ed38-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="8ed38-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="8ed38-182">homeScreenDockIcons</span></span>|<span data-ttu-id="8ed38-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed38-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="8ed38-184">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="8ed38-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="8ed38-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8ed38-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ed38-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="8ed38-186">homeScreenPages</span></span>|<span data-ttu-id="8ed38-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed38-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="8ed38-188">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="8ed38-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="8ed38-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8ed38-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ed38-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="8ed38-190">notificationSettings</span></span>|<span data-ttu-id="8ed38-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed38-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="8ed38-192">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="8ed38-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="8ed38-193">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8ed38-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ed38-194">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="8ed38-194">singleSignOnSettings</span></span>|[<span data-ttu-id="8ed38-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="8ed38-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="8ed38-196">Kerberos 登录设置, 使接收设备上的应用能够顺利进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="8ed38-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="8ed38-197">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="8ed38-197">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="8ed38-198">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="8ed38-198">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="8ed38-199">壁纸显示位置说明符。</span><span class="sxs-lookup"><span data-stu-id="8ed38-199">A wallpaper display location specifier.</span></span> <span data-ttu-id="8ed38-200">可取值为：`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens`。</span><span class="sxs-lookup"><span data-stu-id="8ed38-200">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="8ed38-201">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="8ed38-201">wallpaperImage</span></span>|[<span data-ttu-id="8ed38-202">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8ed38-202">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8ed38-203">墙纸图像必须是 PNG 或 JPEG 格式。</span><span class="sxs-lookup"><span data-stu-id="8ed38-203">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="8ed38-204">它需要具有 iOS 8 或更高版本的受监督的设备。</span><span class="sxs-lookup"><span data-stu-id="8ed38-204">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="8ed38-205">响应</span><span class="sxs-lookup"><span data-stu-id="8ed38-205">Response</span></span>
<span data-ttu-id="8ed38-206">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ed38-206">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed38-207">示例</span><span class="sxs-lookup"><span data-stu-id="8ed38-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ed38-208">请求</span><span class="sxs-lookup"><span data-stu-id="8ed38-208">Request</span></span>
<span data-ttu-id="8ed38-209">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ed38-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3656

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
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
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="8ed38-210">响应</span><span class="sxs-lookup"><span data-stu-id="8ed38-210">Response</span></span>
<span data-ttu-id="8ed38-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ed38-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3828

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
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
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





