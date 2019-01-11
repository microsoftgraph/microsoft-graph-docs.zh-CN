---
title: 创建 iosDeviceFeaturesConfiguration
description: 创建新的 iosDeviceFeaturesConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d96751ea1c0558d23a6d63741b3e1d7d60580ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817204"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="e9e41-103">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9e41-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e9e41-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e9e41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9e41-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e9e41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9e41-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e9e41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9e41-107">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9e41-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9e41-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e9e41-108">Prerequisites</span></span>
<span data-ttu-id="e9e41-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e9e41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e41-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9e41-111">Permission type</span></span>|<span data-ttu-id="e9e41-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e9e41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9e41-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9e41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9e41-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9e41-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9e41-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9e41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9e41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9e41-116">Not supported.</span></span>|
|<span data-ttu-id="e9e41-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9e41-117">Application</span></span>|<span data-ttu-id="e9e41-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9e41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9e41-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9e41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e9e41-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9e41-120">Request headers</span></span>
|<span data-ttu-id="e9e41-121">标头</span><span class="sxs-lookup"><span data-stu-id="e9e41-121">Header</span></span>|<span data-ttu-id="e9e41-122">值</span><span class="sxs-lookup"><span data-stu-id="e9e41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9e41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9e41-123">Authorization</span></span>|<span data-ttu-id="e9e41-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e9e41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9e41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9e41-125">Accept</span></span>|<span data-ttu-id="e9e41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9e41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9e41-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9e41-127">Request body</span></span>
<span data-ttu-id="e9e41-128">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9e41-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="e9e41-129">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e9e41-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="e9e41-130">属性</span><span class="sxs-lookup"><span data-stu-id="e9e41-130">Property</span></span>|<span data-ttu-id="e9e41-131">类型</span><span class="sxs-lookup"><span data-stu-id="e9e41-131">Type</span></span>|<span data-ttu-id="e9e41-132">说明</span><span class="sxs-lookup"><span data-stu-id="e9e41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9e41-133">id</span><span class="sxs-lookup"><span data-stu-id="e9e41-133">id</span></span>|<span data-ttu-id="e9e41-134">String</span><span class="sxs-lookup"><span data-stu-id="e9e41-134">String</span></span>|<span data-ttu-id="e9e41-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e9e41-135">Key of the entity.</span></span> <span data-ttu-id="e9e41-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e41-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e9e41-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9e41-138">DateTimeOffset</span></span>|<span data-ttu-id="e9e41-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e9e41-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e9e41-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e9e41-141">roleScopeTagIds</span></span>|<span data-ttu-id="e9e41-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e9e41-142">String collection</span></span>|<span data-ttu-id="e9e41-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="e9e41-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e9e41-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e9e41-145">supportsScopeTags</span></span>|<span data-ttu-id="e9e41-146">布尔</span><span class="sxs-lookup"><span data-stu-id="e9e41-146">Boolean</span></span>|<span data-ttu-id="e9e41-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="e9e41-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e9e41-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="e9e41-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e9e41-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="e9e41-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e9e41-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e9e41-150">This property is read-only.</span></span> <span data-ttu-id="e9e41-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e41-152">createdDateTime</span></span>|<span data-ttu-id="e9e41-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9e41-153">DateTimeOffset</span></span>|<span data-ttu-id="e9e41-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e9e41-154">DateTime the object was created.</span></span> <span data-ttu-id="e9e41-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-156">description</span><span class="sxs-lookup"><span data-stu-id="e9e41-156">description</span></span>|<span data-ttu-id="e9e41-157">String</span><span class="sxs-lookup"><span data-stu-id="e9e41-157">String</span></span>|<span data-ttu-id="e9e41-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e9e41-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e9e41-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e9e41-160">displayName</span></span>|<span data-ttu-id="e9e41-161">String</span><span class="sxs-lookup"><span data-stu-id="e9e41-161">String</span></span>|<span data-ttu-id="e9e41-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e9e41-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e9e41-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-164">version</span><span class="sxs-lookup"><span data-stu-id="e9e41-164">version</span></span>|<span data-ttu-id="e9e41-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e9e41-165">Int32</span></span>|<span data-ttu-id="e9e41-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e9e41-166">Version of the device configuration.</span></span> <span data-ttu-id="e9e41-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9e41-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="e9e41-168">airPrintDestinations</span></span>|<span data-ttu-id="e9e41-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="e9e41-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="e9e41-170">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="e9e41-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="e9e41-171">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e9e41-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e9e41-172">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e9e41-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="e9e41-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="e9e41-173">assetTagTemplate</span></span>|<span data-ttu-id="e9e41-174">String</span><span class="sxs-lookup"><span data-stu-id="e9e41-174">String</span></span>|<span data-ttu-id="e9e41-175">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="e9e41-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="e9e41-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="e9e41-176">contentFilterSettings</span></span>|[<span data-ttu-id="e9e41-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="e9e41-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="e9e41-178">获取或设置 iOS Web 内容筛选器设置，仅监管模式</span><span class="sxs-lookup"><span data-stu-id="e9e41-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="e9e41-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="e9e41-179">lockScreenFootnote</span></span>|<span data-ttu-id="e9e41-180">String</span><span class="sxs-lookup"><span data-stu-id="e9e41-180">String</span></span>|<span data-ttu-id="e9e41-181">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="e9e41-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="e9e41-182">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="e9e41-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="e9e41-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="e9e41-183">homeScreenDockIcons</span></span>|<span data-ttu-id="e9e41-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9e41-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="e9e41-185">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="e9e41-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="e9e41-186">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e9e41-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e9e41-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="e9e41-187">homeScreenPages</span></span>|<span data-ttu-id="e9e41-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9e41-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="e9e41-189">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="e9e41-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="e9e41-190">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e9e41-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e9e41-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="e9e41-191">notificationSettings</span></span>|<span data-ttu-id="e9e41-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9e41-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="e9e41-193">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e9e41-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="e9e41-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e9e41-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e9e41-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="e9e41-195">singleSignOnSettings</span></span>|[<span data-ttu-id="e9e41-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="e9e41-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="e9e41-197">启用应用程序上接收设备进行身份验证平稳 Kerberos 登录设置。</span><span class="sxs-lookup"><span data-stu-id="e9e41-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|



## <a name="response"></a><span data-ttu-id="e9e41-198">响应</span><span class="sxs-lookup"><span data-stu-id="e9e41-198">Response</span></span>
<span data-ttu-id="e9e41-199">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9e41-199">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9e41-200">示例</span><span class="sxs-lookup"><span data-stu-id="e9e41-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9e41-201">请求</span><span class="sxs-lookup"><span data-stu-id="e9e41-201">Request</span></span>
<span data-ttu-id="e9e41-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9e41-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3543

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="e9e41-203">响应</span><span class="sxs-lookup"><span data-stu-id="e9e41-203">Response</span></span>
<span data-ttu-id="e9e41-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9e41-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3651

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
  }
}
```





