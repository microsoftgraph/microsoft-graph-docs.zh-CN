---
title: 创建 iosDeviceFeaturesConfiguration
description: 创建新的 iosDeviceFeaturesConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6f6a5fe84c5ecd4f95168c027a344237a55961b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423193"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="a9dc5-103">创建 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9dc5-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a9dc5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9dc5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9dc5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9dc5-107">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9dc5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9dc5-108">Prerequisites</span></span>
<span data-ttu-id="a9dc5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9dc5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9dc5-111">Permission type</span></span>|<span data-ttu-id="a9dc5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9dc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9dc5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9dc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9dc5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9dc5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9dc5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9dc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9dc5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-116">Not supported.</span></span>|
|<span data-ttu-id="a9dc5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9dc5-117">Application</span></span>|<span data-ttu-id="a9dc5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9dc5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9dc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9dc5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9dc5-120">Request headers</span></span>
|<span data-ttu-id="a9dc5-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9dc5-121">Header</span></span>|<span data-ttu-id="a9dc5-122">值</span><span class="sxs-lookup"><span data-stu-id="a9dc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9dc5-123">授权</span><span class="sxs-lookup"><span data-stu-id="a9dc5-123">Authorization</span></span>|<span data-ttu-id="a9dc5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9dc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9dc5-125">Accept</span></span>|<span data-ttu-id="a9dc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9dc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9dc5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9dc5-127">Request body</span></span>
<span data-ttu-id="a9dc5-128">在请求正文中，提供 iosDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="a9dc5-129">下表显示创建 iosDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="a9dc5-130">属性</span><span class="sxs-lookup"><span data-stu-id="a9dc5-130">Property</span></span>|<span data-ttu-id="a9dc5-131">类型</span><span class="sxs-lookup"><span data-stu-id="a9dc5-131">Type</span></span>|<span data-ttu-id="a9dc5-132">说明</span><span class="sxs-lookup"><span data-stu-id="a9dc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9dc5-133">id</span><span class="sxs-lookup"><span data-stu-id="a9dc5-133">id</span></span>|<span data-ttu-id="a9dc5-134">String</span><span class="sxs-lookup"><span data-stu-id="a9dc5-134">String</span></span>|<span data-ttu-id="a9dc5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-135">Key of the entity.</span></span> <span data-ttu-id="a9dc5-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9dc5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a9dc5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9dc5-138">DateTimeOffset</span></span>|<span data-ttu-id="a9dc5-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a9dc5-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9dc5-141">roleScopeTagIds</span></span>|<span data-ttu-id="a9dc5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="a9dc5-142">String collection</span></span>|<span data-ttu-id="a9dc5-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9dc5-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a9dc5-145">supportsScopeTags</span></span>|<span data-ttu-id="a9dc5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9dc5-146">Boolean</span></span>|<span data-ttu-id="a9dc5-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9dc5-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9dc5-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9dc5-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-150">This property is read-only.</span></span> <span data-ttu-id="a9dc5-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9dc5-152">createdDateTime</span></span>|<span data-ttu-id="a9dc5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9dc5-153">DateTimeOffset</span></span>|<span data-ttu-id="a9dc5-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-154">DateTime the object was created.</span></span> <span data-ttu-id="a9dc5-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-156">description</span><span class="sxs-lookup"><span data-stu-id="a9dc5-156">description</span></span>|<span data-ttu-id="a9dc5-157">String</span><span class="sxs-lookup"><span data-stu-id="a9dc5-157">String</span></span>|<span data-ttu-id="a9dc5-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9dc5-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a9dc5-160">displayName</span></span>|<span data-ttu-id="a9dc5-161">String</span><span class="sxs-lookup"><span data-stu-id="a9dc5-161">String</span></span>|<span data-ttu-id="a9dc5-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9dc5-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-164">version</span><span class="sxs-lookup"><span data-stu-id="a9dc5-164">version</span></span>|<span data-ttu-id="a9dc5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a9dc5-165">Int32</span></span>|<span data-ttu-id="a9dc5-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-166">Version of the device configuration.</span></span> <span data-ttu-id="a9dc5-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9dc5-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="a9dc5-168">airPrintDestinations</span></span>|<span data-ttu-id="a9dc5-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="a9dc5-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="a9dc5-170">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="a9dc5-171">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a9dc5-172">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a9dc5-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="a9dc5-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="a9dc5-173">assetTagTemplate</span></span>|<span data-ttu-id="a9dc5-174">String</span><span class="sxs-lookup"><span data-stu-id="a9dc5-174">String</span></span>|<span data-ttu-id="a9dc5-175">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="a9dc5-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="a9dc5-176">contentFilterSettings</span></span>|[<span data-ttu-id="a9dc5-177">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="a9dc5-177">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="a9dc5-178">获取或设置 iOS Web 内容筛选器设置，仅监管模式</span><span class="sxs-lookup"><span data-stu-id="a9dc5-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="a9dc5-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="a9dc5-179">lockScreenFootnote</span></span>|<span data-ttu-id="a9dc5-180">String</span><span class="sxs-lookup"><span data-stu-id="a9dc5-180">String</span></span>|<span data-ttu-id="a9dc5-181">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="a9dc5-182">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="a9dc5-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="a9dc5-183">homeScreenDockIcons</span></span>|<span data-ttu-id="a9dc5-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9dc5-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a9dc5-185">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="a9dc5-186">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a9dc5-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="a9dc5-187">homeScreenPages</span></span>|<span data-ttu-id="a9dc5-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9dc5-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="a9dc5-189">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="a9dc5-190">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a9dc5-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="a9dc5-191">notificationSettings</span></span>|<span data-ttu-id="a9dc5-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9dc5-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="a9dc5-193">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="a9dc5-194">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a9dc5-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a9dc5-195">singleSignOnSettings</span></span>|[<span data-ttu-id="a9dc5-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a9dc5-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="a9dc5-197">启用应用程序上接收设备进行身份验证平稳 Kerberos 登录设置。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="a9dc5-198">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="a9dc5-198">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="a9dc5-199">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="a9dc5-199">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="a9dc5-200">墙纸显示位置说明符。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-200">A wallpaper display location specifier.</span></span> <span data-ttu-id="a9dc5-201">可取值为：`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens`。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-201">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="a9dc5-202">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="a9dc5-202">wallpaperImage</span></span>|[<span data-ttu-id="a9dc5-203">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9dc5-203">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a9dc5-204">墙纸图像必须是 PNG 或 JPEG 格式。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-204">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="a9dc5-205">它要求监管的设备 iOS 8 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-205">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="a9dc5-206">响应</span><span class="sxs-lookup"><span data-stu-id="a9dc5-206">Response</span></span>
<span data-ttu-id="a9dc5-207">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-207">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9dc5-208">示例</span><span class="sxs-lookup"><span data-stu-id="a9dc5-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9dc5-209">请求</span><span class="sxs-lookup"><span data-stu-id="a9dc5-209">Request</span></span>
<span data-ttu-id="a9dc5-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9dc5-211">响应</span><span class="sxs-lookup"><span data-stu-id="a9dc5-211">Response</span></span>
<span data-ttu-id="a9dc5-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9dc5-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




