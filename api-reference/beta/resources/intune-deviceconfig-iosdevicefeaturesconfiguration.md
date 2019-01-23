---
title: iosDeviceFeaturesConfiguration 资源类型
description: iOS 设备功能配置的配置文件。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6d0438ac804203bcb1da2b46ba319470b2e90eac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397909"
---
# <a name="iosdevicefeaturesconfiguration-resource-type"></a><span data-ttu-id="5270a-103">iosDeviceFeaturesConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5270a-103">iosDeviceFeaturesConfiguration resource type</span></span>

> <span data-ttu-id="5270a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5270a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5270a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5270a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5270a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5270a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5270a-107">iOS 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="5270a-107">iOS Device Features Configuration Profile.</span></span>


<span data-ttu-id="5270a-108">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-108">Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5270a-109">方法</span><span class="sxs-lookup"><span data-stu-id="5270a-109">Methods</span></span>
|<span data-ttu-id="5270a-110">方法</span><span class="sxs-lookup"><span data-stu-id="5270a-110">Method</span></span>|<span data-ttu-id="5270a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5270a-111">Return Type</span></span>|<span data-ttu-id="5270a-112">说明</span><span class="sxs-lookup"><span data-stu-id="5270a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5270a-113">List iosDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="5270a-113">List iosDeviceFeaturesConfigurations</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-list.md)|<span data-ttu-id="5270a-114">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-114">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) collection</span></span>|<span data-ttu-id="5270a-115">列出 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5270a-115">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="5270a-116">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-116">Get iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-get.md)|[<span data-ttu-id="5270a-117">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-117">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="5270a-118">读取 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5270a-118">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="5270a-119">Create iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-119">Create iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-create.md)|[<span data-ttu-id="5270a-120">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-120">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="5270a-121">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5270a-121">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="5270a-122">Delete iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-122">Delete iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-delete.md)|<span data-ttu-id="5270a-123">无</span><span class="sxs-lookup"><span data-stu-id="5270a-123">None</span></span>|<span data-ttu-id="5270a-124">删除 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="5270a-124">Deletes a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>|
|[<span data-ttu-id="5270a-125">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-125">Update iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-update.md)|[<span data-ttu-id="5270a-126">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5270a-126">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="5270a-127">更新 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5270a-127">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5270a-128">属性</span><span class="sxs-lookup"><span data-stu-id="5270a-128">Properties</span></span>
|<span data-ttu-id="5270a-129">属性</span><span class="sxs-lookup"><span data-stu-id="5270a-129">Property</span></span>|<span data-ttu-id="5270a-130">类型</span><span class="sxs-lookup"><span data-stu-id="5270a-130">Type</span></span>|<span data-ttu-id="5270a-131">说明</span><span class="sxs-lookup"><span data-stu-id="5270a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5270a-132">id</span><span class="sxs-lookup"><span data-stu-id="5270a-132">id</span></span>|<span data-ttu-id="5270a-133">String</span><span class="sxs-lookup"><span data-stu-id="5270a-133">String</span></span>|<span data-ttu-id="5270a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5270a-134">Key of the entity.</span></span> <span data-ttu-id="5270a-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5270a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5270a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5270a-137">DateTimeOffset</span></span>|<span data-ttu-id="5270a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5270a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5270a-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5270a-140">roleScopeTagIds</span></span>|<span data-ttu-id="5270a-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-141">String collection</span></span>|<span data-ttu-id="5270a-142">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="5270a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5270a-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5270a-144">supportsScopeTags</span></span>|<span data-ttu-id="5270a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5270a-145">Boolean</span></span>|<span data-ttu-id="5270a-146">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="5270a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5270a-147">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="5270a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5270a-148">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="5270a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5270a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5270a-149">This property is read-only.</span></span> <span data-ttu-id="5270a-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5270a-151">createdDateTime</span></span>|<span data-ttu-id="5270a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5270a-152">DateTimeOffset</span></span>|<span data-ttu-id="5270a-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5270a-153">DateTime the object was created.</span></span> <span data-ttu-id="5270a-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-155">description</span><span class="sxs-lookup"><span data-stu-id="5270a-155">description</span></span>|<span data-ttu-id="5270a-156">String</span><span class="sxs-lookup"><span data-stu-id="5270a-156">String</span></span>|<span data-ttu-id="5270a-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5270a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5270a-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5270a-159">displayName</span></span>|<span data-ttu-id="5270a-160">String</span><span class="sxs-lookup"><span data-stu-id="5270a-160">String</span></span>|<span data-ttu-id="5270a-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5270a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5270a-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-163">version</span><span class="sxs-lookup"><span data-stu-id="5270a-163">version</span></span>|<span data-ttu-id="5270a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5270a-164">Int32</span></span>|<span data-ttu-id="5270a-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5270a-165">Version of the device configuration.</span></span> <span data-ttu-id="5270a-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="5270a-167">airPrintDestinations</span></span>|<span data-ttu-id="5270a-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="5270a-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="5270a-169">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="5270a-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="5270a-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5270a-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5270a-171">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="5270a-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="5270a-172">assetTagTemplate</span></span>|<span data-ttu-id="5270a-173">String</span><span class="sxs-lookup"><span data-stu-id="5270a-173">String</span></span>|<span data-ttu-id="5270a-174">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="5270a-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="5270a-175">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="5270a-175">contentFilterSettings</span></span>|[<span data-ttu-id="5270a-176">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="5270a-176">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="5270a-177">获取或设置 iOS Web 内容筛选器设置，仅监管模式</span><span class="sxs-lookup"><span data-stu-id="5270a-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="5270a-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="5270a-178">lockScreenFootnote</span></span>|<span data-ttu-id="5270a-179">String</span><span class="sxs-lookup"><span data-stu-id="5270a-179">String</span></span>|<span data-ttu-id="5270a-180">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="5270a-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="5270a-181">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="5270a-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="5270a-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="5270a-182">homeScreenDockIcons</span></span>|<span data-ttu-id="5270a-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="5270a-184">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="5270a-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="5270a-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5270a-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5270a-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="5270a-186">homeScreenPages</span></span>|<span data-ttu-id="5270a-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="5270a-188">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="5270a-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="5270a-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5270a-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5270a-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="5270a-190">notificationSettings</span></span>|<span data-ttu-id="5270a-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="5270a-192">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5270a-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="5270a-193">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5270a-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5270a-194">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="5270a-194">singleSignOnSettings</span></span>|[<span data-ttu-id="5270a-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="5270a-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="5270a-196">启用应用程序上接收设备进行身份验证平稳 Kerberos 登录设置。</span><span class="sxs-lookup"><span data-stu-id="5270a-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="5270a-197">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="5270a-197">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="5270a-198">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="5270a-198">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="5270a-199">墙纸显示位置说明符。</span><span class="sxs-lookup"><span data-stu-id="5270a-199">A wallpaper display location specifier.</span></span> <span data-ttu-id="5270a-200">可取值为：`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens`。</span><span class="sxs-lookup"><span data-stu-id="5270a-200">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="5270a-201">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="5270a-201">wallpaperImage</span></span>|[<span data-ttu-id="5270a-202">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5270a-202">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5270a-203">墙纸图像必须是 PNG 或 JPEG 格式。</span><span class="sxs-lookup"><span data-stu-id="5270a-203">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="5270a-204">它要求监管的设备 iOS 8 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="5270a-204">It requires a supervised device with iOS 8 or later version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5270a-205">关系</span><span class="sxs-lookup"><span data-stu-id="5270a-205">Relationships</span></span>
|<span data-ttu-id="5270a-206">关系</span><span class="sxs-lookup"><span data-stu-id="5270a-206">Relationship</span></span>|<span data-ttu-id="5270a-207">类型</span><span class="sxs-lookup"><span data-stu-id="5270a-207">Type</span></span>|<span data-ttu-id="5270a-208">说明</span><span class="sxs-lookup"><span data-stu-id="5270a-208">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5270a-209">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="5270a-209">groupAssignments</span></span>|<span data-ttu-id="5270a-210">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5270a-210">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="5270a-211">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="5270a-211">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="5270a-212">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-212">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-213">assignments</span><span class="sxs-lookup"><span data-stu-id="5270a-213">assignments</span></span>|<span data-ttu-id="5270a-214">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-214">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5270a-215">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="5270a-215">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="5270a-216">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-216">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-217">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5270a-217">deviceStatuses</span></span>|<span data-ttu-id="5270a-218">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-218">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="5270a-219">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="5270a-219">Device configuration installation status by device.</span></span> <span data-ttu-id="5270a-220">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-220">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-221">userStatuses</span><span class="sxs-lookup"><span data-stu-id="5270a-221">userStatuses</span></span>|<span data-ttu-id="5270a-222">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-222">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="5270a-223">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="5270a-223">Device configuration installation status by user.</span></span> <span data-ttu-id="5270a-224">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-224">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-225">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5270a-225">deviceStatusOverview</span></span>|[<span data-ttu-id="5270a-226">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5270a-226">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="5270a-227">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-227">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-228">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5270a-228">userStatusOverview</span></span>|[<span data-ttu-id="5270a-229">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="5270a-229">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="5270a-230">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-230">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-231">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="5270a-231">deviceSettingStateSummaries</span></span>|<span data-ttu-id="5270a-232">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5270a-232">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="5270a-233">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5270a-233">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5270a-234">identityCertificateForClientAuthentication</span><span class="sxs-lookup"><span data-stu-id="5270a-234">identityCertificateForClientAuthentication</span></span>|[<span data-ttu-id="5270a-235">iosCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="5270a-235">iosCertificateProfileBase</span></span>](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|<span data-ttu-id="5270a-236">在单一登录设置中使用的 Kerberos 票证续订的标识证书。</span><span class="sxs-lookup"><span data-stu-id="5270a-236">Identity Certificate for the renewal of Kerberos ticket used in single sign-on settings.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5270a-237">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5270a-237">JSON Representation</span></span>
<span data-ttu-id="5270a-238">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5270a-238">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDeviceFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "String",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "String",
        "bookmarkFolder": "String",
        "displayName": "String"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "String",
        "bookmarkFolder": "String",
        "displayName": "String"
      }
    ]
  },
  "lockScreenFootnote": "String",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "String",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "String",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "String",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "String",
                  "bundleID": "String"
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
      "bundleID": "String",
      "appName": "String",
      "publisher": "String",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "String",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "String",
        "publisher": "String",
        "appStoreUrl": "String",
        "appId": "String"
      }
    ],
    "allowedUrls": [
      "String"
    ],
    "displayName": "String",
    "kerberosPrincipalName": "String",
    "kerberosRealm": "String"
  },
  "wallpaperDisplayLocation": "String",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




