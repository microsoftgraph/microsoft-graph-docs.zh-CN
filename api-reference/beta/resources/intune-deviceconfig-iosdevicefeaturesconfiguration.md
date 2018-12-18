---
title: iosDeviceFeaturesConfiguration 资源类型
description: iOS 设备功能配置的配置文件。
author: tfitzmac
ms.openlocfilehash: 114221bdb6390b80f7dd9b86edc7dac30d2bee46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349264"
---
# <a name="iosdevicefeaturesconfiguration-resource-type"></a><span data-ttu-id="0d31e-103">iosDeviceFeaturesConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-103">iosDeviceFeaturesConfiguration resource type</span></span>

> <span data-ttu-id="0d31e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0d31e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d31e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0d31e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d31e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0d31e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d31e-107">iOS 设备功能配置的配置文件。</span><span class="sxs-lookup"><span data-stu-id="0d31e-107">iOS Device Features Configuration Profile.</span></span>

<span data-ttu-id="0d31e-108">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-108">Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0d31e-109">方法</span><span class="sxs-lookup"><span data-stu-id="0d31e-109">Methods</span></span>
|<span data-ttu-id="0d31e-110">方法</span><span class="sxs-lookup"><span data-stu-id="0d31e-110">Method</span></span>|<span data-ttu-id="0d31e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-111">Return Type</span></span>|<span data-ttu-id="0d31e-112">说明</span><span class="sxs-lookup"><span data-stu-id="0d31e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0d31e-113">List iosDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="0d31e-113">List iosDeviceFeaturesConfigurations</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-list.md)|<span data-ttu-id="0d31e-114">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-114">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) collection</span></span>|<span data-ttu-id="0d31e-115">列出 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d31e-115">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0d31e-116">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-116">Get iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-get.md)|[<span data-ttu-id="0d31e-117">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-117">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="0d31e-118">读取 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d31e-118">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0d31e-119">Create iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-119">Create iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-create.md)|[<span data-ttu-id="0d31e-120">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-120">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="0d31e-121">创建新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d31e-121">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0d31e-122">Delete iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-122">Delete iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-delete.md)|<span data-ttu-id="0d31e-123">无</span><span class="sxs-lookup"><span data-stu-id="0d31e-123">None</span></span>|<span data-ttu-id="0d31e-124">删除 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0d31e-124">Deletes a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>|
|[<span data-ttu-id="0d31e-125">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-125">Update iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-update.md)|[<span data-ttu-id="0d31e-126">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d31e-126">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="0d31e-127">更新 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-127">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d31e-128">属性</span><span class="sxs-lookup"><span data-stu-id="0d31e-128">Properties</span></span>
|<span data-ttu-id="0d31e-129">属性</span><span class="sxs-lookup"><span data-stu-id="0d31e-129">Property</span></span>|<span data-ttu-id="0d31e-130">类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-130">Type</span></span>|<span data-ttu-id="0d31e-131">说明</span><span class="sxs-lookup"><span data-stu-id="0d31e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d31e-132">id</span><span class="sxs-lookup"><span data-stu-id="0d31e-132">id</span></span>|<span data-ttu-id="0d31e-133">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-133">String</span></span>|<span data-ttu-id="0d31e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0d31e-134">Key of the entity.</span></span> <span data-ttu-id="0d31e-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d31e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0d31e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d31e-137">DateTimeOffset</span></span>|<span data-ttu-id="0d31e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0d31e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0d31e-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d31e-140">roleScopeTagIds</span></span>|<span data-ttu-id="0d31e-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-141">String collection</span></span>|<span data-ttu-id="0d31e-142">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0d31e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0d31e-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0d31e-144">supportsScopeTags</span></span>|<span data-ttu-id="0d31e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d31e-145">Boolean</span></span>|<span data-ttu-id="0d31e-146">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0d31e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0d31e-147">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0d31e-148">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0d31e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0d31e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0d31e-149">This property is read-only.</span></span> <span data-ttu-id="0d31e-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d31e-151">createdDateTime</span></span>|<span data-ttu-id="0d31e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d31e-152">DateTimeOffset</span></span>|<span data-ttu-id="0d31e-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0d31e-153">DateTime the object was created.</span></span> <span data-ttu-id="0d31e-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-155">description</span><span class="sxs-lookup"><span data-stu-id="0d31e-155">description</span></span>|<span data-ttu-id="0d31e-156">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-156">String</span></span>|<span data-ttu-id="0d31e-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0d31e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d31e-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0d31e-159">displayName</span></span>|<span data-ttu-id="0d31e-160">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-160">String</span></span>|<span data-ttu-id="0d31e-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0d31e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d31e-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-163">version</span><span class="sxs-lookup"><span data-stu-id="0d31e-163">version</span></span>|<span data-ttu-id="0d31e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0d31e-164">Int32</span></span>|<span data-ttu-id="0d31e-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0d31e-165">Version of the device configuration.</span></span> <span data-ttu-id="0d31e-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="0d31e-167">airPrintDestinations</span></span>|<span data-ttu-id="0d31e-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="0d31e-169">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="0d31e-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="0d31e-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0d31e-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0d31e-171">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="0d31e-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="0d31e-172">assetTagTemplate</span></span>|<span data-ttu-id="0d31e-173">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-173">String</span></span>|<span data-ttu-id="0d31e-174">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="0d31e-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="0d31e-175">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="0d31e-175">contentFilterSettings</span></span>|[<span data-ttu-id="0d31e-176">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="0d31e-176">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="0d31e-177">获取或设置 iOS Web 内容筛选器设置，仅监管模式</span><span class="sxs-lookup"><span data-stu-id="0d31e-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="0d31e-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="0d31e-178">lockScreenFootnote</span></span>|<span data-ttu-id="0d31e-179">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-179">String</span></span>|<span data-ttu-id="0d31e-180">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="0d31e-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="0d31e-181">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="0d31e-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="0d31e-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="0d31e-182">homeScreenDockIcons</span></span>|<span data-ttu-id="0d31e-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="0d31e-184">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="0d31e-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="0d31e-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0d31e-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0d31e-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="0d31e-186">homeScreenPages</span></span>|<span data-ttu-id="0d31e-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="0d31e-188">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="0d31e-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="0d31e-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0d31e-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0d31e-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="0d31e-190">notificationSettings</span></span>|<span data-ttu-id="0d31e-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="0d31e-192">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0d31e-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="0d31e-193">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0d31e-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0d31e-194">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="0d31e-194">singleSignOnSettings</span></span>|[<span data-ttu-id="0d31e-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="0d31e-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="0d31e-196">启用应用程序上接收设备进行身份验证平稳 Kerberos 登录设置。</span><span class="sxs-lookup"><span data-stu-id="0d31e-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d31e-197">Relationships</span><span class="sxs-lookup"><span data-stu-id="0d31e-197">Relationships</span></span>
|<span data-ttu-id="0d31e-198">关系</span><span class="sxs-lookup"><span data-stu-id="0d31e-198">Relationship</span></span>|<span data-ttu-id="0d31e-199">类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-199">Type</span></span>|<span data-ttu-id="0d31e-200">说明</span><span class="sxs-lookup"><span data-stu-id="0d31e-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d31e-201">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0d31e-201">groupAssignments</span></span>|<span data-ttu-id="0d31e-202">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-202">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0d31e-203">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0d31e-203">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="0d31e-204">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-204">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-205">assignments</span><span class="sxs-lookup"><span data-stu-id="0d31e-205">assignments</span></span>|<span data-ttu-id="0d31e-206">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-206">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0d31e-207">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0d31e-207">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0d31e-208">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-208">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-209">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0d31e-209">deviceStatuses</span></span>|<span data-ttu-id="0d31e-210">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-210">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0d31e-211">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0d31e-211">Device configuration installation status by device.</span></span> <span data-ttu-id="0d31e-212">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-212">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-213">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0d31e-213">userStatuses</span></span>|<span data-ttu-id="0d31e-214">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-214">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0d31e-215">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0d31e-215">Device configuration installation status by user.</span></span> <span data-ttu-id="0d31e-216">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-216">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-217">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0d31e-217">deviceStatusOverview</span></span>|[<span data-ttu-id="0d31e-218">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0d31e-218">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0d31e-219">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-219">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-220">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0d31e-220">userStatusOverview</span></span>|[<span data-ttu-id="0d31e-221">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0d31e-221">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0d31e-222">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-222">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-223">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0d31e-223">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0d31e-224">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-224">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0d31e-225">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d31e-225">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d31e-226">identityCertificateForClientAuthentication</span><span class="sxs-lookup"><span data-stu-id="0d31e-226">identityCertificateForClientAuthentication</span></span>|[<span data-ttu-id="0d31e-227">iosCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="0d31e-227">iosCertificateProfileBase</span></span>](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|<span data-ttu-id="0d31e-228">在单一登录设置中使用的 Kerberos 票证续订的标识证书。</span><span class="sxs-lookup"><span data-stu-id="0d31e-228">Identity Certificate for the renewal of Kerberos ticket used in single sign-on settings.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d31e-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d31e-229">JSON Representation</span></span>
<span data-ttu-id="0d31e-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d31e-230">Here is a JSON representation of the resource.</span></span>
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
  }
}
```





