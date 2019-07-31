---
title: 更新 iosDeviceFeaturesConfiguration
description: 更新 iosDeviceFeaturesConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95a454fd5571d13e88efe7bd8dfda948ecae695c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948465"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="6bcfa-103">更新 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bcfa-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6bcfa-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bcfa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bcfa-106">更新 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bcfa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6bcfa-107">Prerequisites</span></span>
<span data-ttu-id="6bcfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bcfa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bcfa-110">Permission type</span></span>|<span data-ttu-id="6bcfa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6bcfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bcfa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bcfa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6bcfa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bcfa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bcfa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bcfa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bcfa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-115">Not supported.</span></span>|
|<span data-ttu-id="6bcfa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bcfa-116">Application</span></span>|<span data-ttu-id="6bcfa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bcfa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bcfa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6bcfa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bcfa-119">Request headers</span></span>
|<span data-ttu-id="6bcfa-120">标头</span><span class="sxs-lookup"><span data-stu-id="6bcfa-120">Header</span></span>|<span data-ttu-id="6bcfa-121">值</span><span class="sxs-lookup"><span data-stu-id="6bcfa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bcfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bcfa-122">Authorization</span></span>|<span data-ttu-id="6bcfa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bcfa-124">接受</span><span class="sxs-lookup"><span data-stu-id="6bcfa-124">Accept</span></span>|<span data-ttu-id="6bcfa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6bcfa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bcfa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bcfa-126">Request body</span></span>
<span data-ttu-id="6bcfa-127">在请求正文中，提供 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6bcfa-128">下表显示创建 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6bcfa-129">属性</span><span class="sxs-lookup"><span data-stu-id="6bcfa-129">Property</span></span>|<span data-ttu-id="6bcfa-130">类型</span><span class="sxs-lookup"><span data-stu-id="6bcfa-130">Type</span></span>|<span data-ttu-id="6bcfa-131">说明</span><span class="sxs-lookup"><span data-stu-id="6bcfa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bcfa-132">id</span><span class="sxs-lookup"><span data-stu-id="6bcfa-132">id</span></span>|<span data-ttu-id="6bcfa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6bcfa-133">String</span></span>|<span data-ttu-id="6bcfa-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-134">Key of the entity.</span></span> <span data-ttu-id="6bcfa-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bcfa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6bcfa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bcfa-137">DateTimeOffset</span></span>|<span data-ttu-id="6bcfa-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6bcfa-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6bcfa-140">roleScopeTagIds</span></span>|<span data-ttu-id="6bcfa-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6bcfa-141">String collection</span></span>|<span data-ttu-id="6bcfa-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6bcfa-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6bcfa-144">supportsScopeTags</span></span>|<span data-ttu-id="6bcfa-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bcfa-145">Boolean</span></span>|<span data-ttu-id="6bcfa-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6bcfa-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6bcfa-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6bcfa-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-149">This property is read-only.</span></span> <span data-ttu-id="6bcfa-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6bcfa-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6bcfa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6bcfa-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6bcfa-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6bcfa-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6bcfa-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6bcfa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6bcfa-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6bcfa-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6bcfa-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6bcfa-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6bcfa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6bcfa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6bcfa-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6bcfa-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bcfa-163">createdDateTime</span></span>|<span data-ttu-id="6bcfa-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bcfa-164">DateTimeOffset</span></span>|<span data-ttu-id="6bcfa-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-165">DateTime the object was created.</span></span> <span data-ttu-id="6bcfa-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-167">说明</span><span class="sxs-lookup"><span data-stu-id="6bcfa-167">description</span></span>|<span data-ttu-id="6bcfa-168">String</span><span class="sxs-lookup"><span data-stu-id="6bcfa-168">String</span></span>|<span data-ttu-id="6bcfa-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bcfa-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6bcfa-171">displayName</span></span>|<span data-ttu-id="6bcfa-172">字符串</span><span class="sxs-lookup"><span data-stu-id="6bcfa-172">String</span></span>|<span data-ttu-id="6bcfa-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bcfa-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-175">version</span><span class="sxs-lookup"><span data-stu-id="6bcfa-175">version</span></span>|<span data-ttu-id="6bcfa-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6bcfa-176">Int32</span></span>|<span data-ttu-id="6bcfa-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-177">Version of the device configuration.</span></span> <span data-ttu-id="6bcfa-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bcfa-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="6bcfa-179">airPrintDestinations</span></span>|<span data-ttu-id="6bcfa-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bcfa-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="6bcfa-181">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="6bcfa-182">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6bcfa-183">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="6bcfa-184">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="6bcfa-184">assetTagTemplate</span></span>|<span data-ttu-id="6bcfa-185">String</span><span class="sxs-lookup"><span data-stu-id="6bcfa-185">String</span></span>|<span data-ttu-id="6bcfa-186">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-186">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="6bcfa-187">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="6bcfa-187">contentFilterSettings</span></span>|[<span data-ttu-id="6bcfa-188">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="6bcfa-188">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="6bcfa-189">获取或设置 iOS Web 内容筛选器设置 (仅限受监督模式)</span><span class="sxs-lookup"><span data-stu-id="6bcfa-189">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="6bcfa-190">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="6bcfa-190">lockScreenFootnote</span></span>|<span data-ttu-id="6bcfa-191">String</span><span class="sxs-lookup"><span data-stu-id="6bcfa-191">String</span></span>|<span data-ttu-id="6bcfa-192">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-192">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="6bcfa-193">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-193">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="6bcfa-194">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="6bcfa-194">homeScreenDockIcons</span></span>|<span data-ttu-id="6bcfa-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bcfa-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="6bcfa-196">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-196">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="6bcfa-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bcfa-198">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="6bcfa-198">homeScreenPages</span></span>|<span data-ttu-id="6bcfa-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bcfa-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="6bcfa-200">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-200">A list of pages on the Home Screen.</span></span> <span data-ttu-id="6bcfa-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bcfa-202">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="6bcfa-202">notificationSettings</span></span>|<span data-ttu-id="6bcfa-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bcfa-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="6bcfa-204">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-204">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="6bcfa-205">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-205">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6bcfa-206">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="6bcfa-206">singleSignOnSettings</span></span>|[<span data-ttu-id="6bcfa-207">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="6bcfa-207">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="6bcfa-208">Kerberos 登录设置, 使接收设备上的应用能够顺利进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-208">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="6bcfa-209">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="6bcfa-209">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="6bcfa-210">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="6bcfa-210">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="6bcfa-211">壁纸显示位置说明符。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-211">A wallpaper display location specifier.</span></span> <span data-ttu-id="6bcfa-212">可取值为：`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens`。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-212">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="6bcfa-213">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="6bcfa-213">wallpaperImage</span></span>|[<span data-ttu-id="6bcfa-214">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6bcfa-214">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6bcfa-215">墙纸图像必须是 PNG 或 JPEG 格式。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-215">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="6bcfa-216">它需要具有 iOS 8 或更高版本的受监督的设备。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-216">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="6bcfa-217">响应</span><span class="sxs-lookup"><span data-stu-id="6bcfa-217">Response</span></span>
<span data-ttu-id="6bcfa-218">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-218">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bcfa-219">示例</span><span class="sxs-lookup"><span data-stu-id="6bcfa-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bcfa-220">请求</span><span class="sxs-lookup"><span data-stu-id="6bcfa-220">Request</span></span>
<span data-ttu-id="6bcfa-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4429

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="6bcfa-222">响应</span><span class="sxs-lookup"><span data-stu-id="6bcfa-222">Response</span></span>
<span data-ttu-id="6bcfa-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6bcfa-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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





