---
title: 更新 iosDeviceFeaturesConfiguration
description: 更新 iosDeviceFeaturesConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc31cb020894562e58f1c71dfc4261f1cefdbfdd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130047"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="2df2e-103">更新 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="2df2e-103">Update iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="2df2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2df2e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2df2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2df2e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2df2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2df2e-107">更新 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2df2e-107">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2df2e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2df2e-108">Prerequisites</span></span>
<span data-ttu-id="2df2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2df2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df2e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2df2e-111">Permission type</span></span>|<span data-ttu-id="2df2e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2df2e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df2e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2df2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2df2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2df2e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2df2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df2e-116">Not supported.</span></span>|
|<span data-ttu-id="2df2e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2df2e-117">Application</span></span>|<span data-ttu-id="2df2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df2e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2df2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2df2e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2df2e-120">Request headers</span></span>
|<span data-ttu-id="2df2e-121">标头</span><span class="sxs-lookup"><span data-stu-id="2df2e-121">Header</span></span>|<span data-ttu-id="2df2e-122">值</span><span class="sxs-lookup"><span data-stu-id="2df2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df2e-123">Authorization</span></span>|<span data-ttu-id="2df2e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2df2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df2e-125">接受</span><span class="sxs-lookup"><span data-stu-id="2df2e-125">Accept</span></span>|<span data-ttu-id="2df2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2df2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df2e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2df2e-127">Request body</span></span>
<span data-ttu-id="2df2e-128">在请求正文中，提供 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2df2e-128">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="2df2e-129">下表显示创建 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2df2e-129">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="2df2e-130">属性</span><span class="sxs-lookup"><span data-stu-id="2df2e-130">Property</span></span>|<span data-ttu-id="2df2e-131">类型</span><span class="sxs-lookup"><span data-stu-id="2df2e-131">Type</span></span>|<span data-ttu-id="2df2e-132">说明</span><span class="sxs-lookup"><span data-stu-id="2df2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df2e-133">id</span><span class="sxs-lookup"><span data-stu-id="2df2e-133">id</span></span>|<span data-ttu-id="2df2e-134">String</span><span class="sxs-lookup"><span data-stu-id="2df2e-134">String</span></span>|<span data-ttu-id="2df2e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2df2e-135">Key of the entity.</span></span> <span data-ttu-id="2df2e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2df2e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2df2e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df2e-138">DateTimeOffset</span></span>|<span data-ttu-id="2df2e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2df2e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2df2e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2df2e-141">roleScopeTagIds</span></span>|<span data-ttu-id="2df2e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2df2e-142">String collection</span></span>|<span data-ttu-id="2df2e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2df2e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2df2e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2df2e-145">supportsScopeTags</span></span>|<span data-ttu-id="2df2e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2df2e-146">Boolean</span></span>|<span data-ttu-id="2df2e-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="2df2e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2df2e-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="2df2e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2df2e-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="2df2e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2df2e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2df2e-150">This property is read-only.</span></span> <span data-ttu-id="2df2e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2df2e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2df2e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2df2e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2df2e-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="2df2e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2df2e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2df2e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2df2e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2df2e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2df2e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2df2e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2df2e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2df2e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2df2e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2df2e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2df2e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2df2e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2df2e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2df2e-164">createdDateTime</span></span>|<span data-ttu-id="2df2e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df2e-165">DateTimeOffset</span></span>|<span data-ttu-id="2df2e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2df2e-166">DateTime the object was created.</span></span> <span data-ttu-id="2df2e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-168">说明</span><span class="sxs-lookup"><span data-stu-id="2df2e-168">description</span></span>|<span data-ttu-id="2df2e-169">String</span><span class="sxs-lookup"><span data-stu-id="2df2e-169">String</span></span>|<span data-ttu-id="2df2e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2df2e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2df2e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2df2e-172">displayName</span></span>|<span data-ttu-id="2df2e-173">String</span><span class="sxs-lookup"><span data-stu-id="2df2e-173">String</span></span>|<span data-ttu-id="2df2e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2df2e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2df2e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-176">version</span><span class="sxs-lookup"><span data-stu-id="2df2e-176">version</span></span>|<span data-ttu-id="2df2e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2df2e-177">Int32</span></span>|<span data-ttu-id="2df2e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2df2e-178">Version of the device configuration.</span></span> <span data-ttu-id="2df2e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2df2e-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="2df2e-180">airPrintDestinations</span></span>|<span data-ttu-id="2df2e-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2df2e-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="2df2e-182">应始终显示的 AirPrint 打印机数组。</span><span class="sxs-lookup"><span data-stu-id="2df2e-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="2df2e-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2df2e-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2df2e-184">继承自 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="2df2e-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="2df2e-185">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="2df2e-185">assetTagTemplate</span></span>|<span data-ttu-id="2df2e-186">String</span><span class="sxs-lookup"><span data-stu-id="2df2e-186">String</span></span>|<span data-ttu-id="2df2e-187">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="2df2e-187">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="2df2e-188">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="2df2e-188">contentFilterSettings</span></span>|[<span data-ttu-id="2df2e-189">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="2df2e-189">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="2df2e-190">获取或设置 iOS Web 内容筛选器设置，仅限监督模式</span><span class="sxs-lookup"><span data-stu-id="2df2e-190">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="2df2e-191">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="2df2e-191">lockScreenFootnote</span></span>|<span data-ttu-id="2df2e-192">String</span><span class="sxs-lookup"><span data-stu-id="2df2e-192">String</span></span>|<span data-ttu-id="2df2e-193">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="2df2e-193">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="2df2e-194">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="2df2e-194">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="2df2e-195">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="2df2e-195">homeScreenDockIcons</span></span>|<span data-ttu-id="2df2e-196">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2df2e-196">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="2df2e-197">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="2df2e-197">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="2df2e-198">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2df2e-198">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2df2e-199">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="2df2e-199">homeScreenPages</span></span>|<span data-ttu-id="2df2e-200">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2df2e-200">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="2df2e-201">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="2df2e-201">A list of pages on the Home Screen.</span></span> <span data-ttu-id="2df2e-202">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2df2e-202">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2df2e-203">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="2df2e-203">notificationSettings</span></span>|<span data-ttu-id="2df2e-204">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2df2e-204">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="2df2e-205">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="2df2e-205">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="2df2e-206">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2df2e-206">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2df2e-207">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="2df2e-207">singleSignOnSettings</span></span>|[<span data-ttu-id="2df2e-208">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="2df2e-208">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="2df2e-209">Kerberos 登录设置，使接收设备上的应用能够顺利进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="2df2e-209">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="2df2e-210">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="2df2e-210">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="2df2e-211">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="2df2e-211">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="2df2e-212">墙纸显示位置说明器。</span><span class="sxs-lookup"><span data-stu-id="2df2e-212">A wallpaper display location specifier.</span></span> <span data-ttu-id="2df2e-213">可取值为：`notConfigured`、`lockScreen`、`homeScreen`、`lockAndHomeScreens`。</span><span class="sxs-lookup"><span data-stu-id="2df2e-213">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="2df2e-214">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="2df2e-214">wallpaperImage</span></span>|[<span data-ttu-id="2df2e-215">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2df2e-215">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2df2e-216">墙纸图像必须为 PNG 或 JPEG 格式。</span><span class="sxs-lookup"><span data-stu-id="2df2e-216">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="2df2e-217">它需要具有 iOS 8 或更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="2df2e-217">It requires a supervised device with iOS 8 or later version.</span></span>|
|<span data-ttu-id="2df2e-218">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2df2e-218">singleSignOnExtension</span></span>|[<span data-ttu-id="2df2e-219">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2df2e-219">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="2df2e-220">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="2df2e-220">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="2df2e-221">已弃用：改为使用 IOSSingleSignOnExtension。</span><span class="sxs-lookup"><span data-stu-id="2df2e-221">Deprecated: use IOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="2df2e-222">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2df2e-222">iosSingleSignOnExtension</span></span>|[<span data-ttu-id="2df2e-223">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="2df2e-223">iosSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-iossinglesignonextension.md)|<span data-ttu-id="2df2e-224">获取或设置单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="2df2e-224">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="2df2e-225">响应</span><span class="sxs-lookup"><span data-stu-id="2df2e-225">Response</span></span>
<span data-ttu-id="2df2e-226">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2df2e-226">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df2e-227">示例</span><span class="sxs-lookup"><span data-stu-id="2df2e-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="2df2e-228">请求</span><span class="sxs-lookup"><span data-stu-id="2df2e-228">Request</span></span>
<span data-ttu-id="2df2e-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2df2e-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 6830

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
              "bundleID": "Bundle ID value",
              "isWebClip": true
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
                  "bundleID": "Bundle ID value",
                  "isWebClip": true
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
      "soundsEnabled": true,
      "previewVisibility": "alwaysShow"
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
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "iosSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  }
}
```

### <a name="response"></a><span data-ttu-id="2df2e-230">响应</span><span class="sxs-lookup"><span data-stu-id="2df2e-230">Response</span></span>
<span data-ttu-id="2df2e-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2df2e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7002

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
              "bundleID": "Bundle ID value",
              "isWebClip": true
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
                  "bundleID": "Bundle ID value",
                  "isWebClip": true
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
      "soundsEnabled": true,
      "previewVisibility": "alwaysShow"
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
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "iosSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  }
}
```




