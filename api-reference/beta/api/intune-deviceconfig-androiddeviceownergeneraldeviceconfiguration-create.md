---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26a546a0ca63b8e1f967a5ac90108ea6b8e54999
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933226"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="ffe19-103">创建 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffe19-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ffe19-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffe19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffe19-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffe19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffe19-106">创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffe19-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffe19-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffe19-107">Prerequisites</span></span>
<span data-ttu-id="ffe19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffe19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffe19-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffe19-110">Permission type</span></span>|<span data-ttu-id="ffe19-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffe19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffe19-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffe19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffe19-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe19-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffe19-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffe19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffe19-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffe19-115">Not supported.</span></span>|
|<span data-ttu-id="ffe19-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffe19-116">Application</span></span>|<span data-ttu-id="ffe19-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffe19-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffe19-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffe19-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ffe19-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffe19-119">Request headers</span></span>
|<span data-ttu-id="ffe19-120">标头</span><span class="sxs-lookup"><span data-stu-id="ffe19-120">Header</span></span>|<span data-ttu-id="ffe19-121">值</span><span class="sxs-lookup"><span data-stu-id="ffe19-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffe19-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffe19-122">Authorization</span></span>|<span data-ttu-id="ffe19-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffe19-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffe19-124">接受</span><span class="sxs-lookup"><span data-stu-id="ffe19-124">Accept</span></span>|<span data-ttu-id="ffe19-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffe19-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffe19-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffe19-126">Request body</span></span>
<span data-ttu-id="ffe19-127">在请求正文中, 提供 androidDeviceOwnerGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffe19-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="ffe19-128">下表显示创建 androidDeviceOwnerGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ffe19-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="ffe19-129">属性</span><span class="sxs-lookup"><span data-stu-id="ffe19-129">Property</span></span>|<span data-ttu-id="ffe19-130">类型</span><span class="sxs-lookup"><span data-stu-id="ffe19-130">Type</span></span>|<span data-ttu-id="ffe19-131">说明</span><span class="sxs-lookup"><span data-stu-id="ffe19-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe19-132">id</span><span class="sxs-lookup"><span data-stu-id="ffe19-132">id</span></span>|<span data-ttu-id="ffe19-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ffe19-133">String</span></span>|<span data-ttu-id="ffe19-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ffe19-134">Key of the entity.</span></span> <span data-ttu-id="ffe19-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffe19-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ffe19-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe19-137">DateTimeOffset</span></span>|<span data-ttu-id="ffe19-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ffe19-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ffe19-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ffe19-140">roleScopeTagIds</span></span>|<span data-ttu-id="ffe19-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ffe19-141">String collection</span></span>|<span data-ttu-id="ffe19-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ffe19-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ffe19-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ffe19-144">supportsScopeTags</span></span>|<span data-ttu-id="ffe19-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-145">Boolean</span></span>|<span data-ttu-id="ffe19-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ffe19-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ffe19-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ffe19-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ffe19-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ffe19-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ffe19-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ffe19-149">This property is read-only.</span></span> <span data-ttu-id="ffe19-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffe19-151">createdDateTime</span></span>|<span data-ttu-id="ffe19-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe19-152">DateTimeOffset</span></span>|<span data-ttu-id="ffe19-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ffe19-153">DateTime the object was created.</span></span> <span data-ttu-id="ffe19-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-155">说明</span><span class="sxs-lookup"><span data-stu-id="ffe19-155">description</span></span>|<span data-ttu-id="ffe19-156">String</span><span class="sxs-lookup"><span data-stu-id="ffe19-156">String</span></span>|<span data-ttu-id="ffe19-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ffe19-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ffe19-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ffe19-159">displayName</span></span>|<span data-ttu-id="ffe19-160">String</span><span class="sxs-lookup"><span data-stu-id="ffe19-160">String</span></span>|<span data-ttu-id="ffe19-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ffe19-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ffe19-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-163">version</span><span class="sxs-lookup"><span data-stu-id="ffe19-163">version</span></span>|<span data-ttu-id="ffe19-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-164">Int32</span></span>|<span data-ttu-id="ffe19-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ffe19-165">Version of the device configuration.</span></span> <span data-ttu-id="ffe19-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffe19-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffe19-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="ffe19-167">accountsBlockModification</span></span>|<span data-ttu-id="ffe19-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-168">Boolean</span></span>|<span data-ttu-id="ffe19-169">指示是否禁用添加或删除帐户。</span><span class="sxs-lookup"><span data-stu-id="ffe19-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="ffe19-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="ffe19-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="ffe19-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-171">Boolean</span></span>|<span data-ttu-id="ffe19-172">指示是否允许用户启用 "未知源" 设置。</span><span class="sxs-lookup"><span data-stu-id="ffe19-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="ffe19-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="ffe19-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="ffe19-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="ffe19-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="ffe19-175">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="ffe19-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="ffe19-176">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="ffe19-177">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="ffe19-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="ffe19-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="ffe19-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="ffe19-179">指示对运行时权限请求的权限策略 (如果专门没有为应用程序定义)。</span><span class="sxs-lookup"><span data-stu-id="ffe19-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="ffe19-180">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="ffe19-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="ffe19-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="ffe19-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-182">Boolean</span></span>|<span data-ttu-id="ffe19-183">是否建议所有应用都将跳过他们可能已添加的任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="ffe19-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="ffe19-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffe19-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="ffe19-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-185">Boolean</span></span>|<span data-ttu-id="ffe19-186">指示是否阻止用户配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="ffe19-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="ffe19-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="ffe19-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="ffe19-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-188">Boolean</span></span>|<span data-ttu-id="ffe19-189">指示是否阻止用户通过蓝牙共享联系人。</span><span class="sxs-lookup"><span data-stu-id="ffe19-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="ffe19-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-190">cameraBlocked</span></span>|<span data-ttu-id="ffe19-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-191">Boolean</span></span>|<span data-ttu-id="ffe19-192">指示是否禁用相机的使用。</span><span class="sxs-lookup"><span data-stu-id="ffe19-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="ffe19-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="ffe19-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="ffe19-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-194">Boolean</span></span>|<span data-ttu-id="ffe19-195">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="ffe19-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="ffe19-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-196">dataRoamingBlocked</span></span>|<span data-ttu-id="ffe19-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-197">Boolean</span></span>|<span data-ttu-id="ffe19-198">指示是否阻止用户使用数据漫游。</span><span class="sxs-lookup"><span data-stu-id="ffe19-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="ffe19-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="ffe19-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-200">Boolean</span></span>|<span data-ttu-id="ffe19-201">指示是否阻止用户手动更改设备上的日期或时间</span><span class="sxs-lookup"><span data-stu-id="ffe19-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="ffe19-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="ffe19-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="ffe19-203">String collection</span><span class="sxs-lookup"><span data-stu-id="ffe19-203">String collection</span></span>|<span data-ttu-id="ffe19-204">在设备出厂重置之前, 将需要进行身份验证的 Google 帐户电子邮件的列表, 然后才能对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="ffe19-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="ffe19-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-205">factoryResetBlocked</span></span>|<span data-ttu-id="ffe19-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-206">Boolean</span></span>|<span data-ttu-id="ffe19-207">指示是否禁用了 "设置" 中的 "恢复出厂设置" 选项。</span><span class="sxs-lookup"><span data-stu-id="ffe19-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="ffe19-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="ffe19-208">kioskModeApps</span></span>|<span data-ttu-id="ffe19-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ffe19-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ffe19-210">设备处于展台模式时将显示的托管应用列表。</span><span class="sxs-lookup"><span data-stu-id="ffe19-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="ffe19-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ffe19-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ffe19-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="ffe19-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="ffe19-213">String</span><span class="sxs-lookup"><span data-stu-id="ffe19-213">String</span></span>|<span data-ttu-id="ffe19-214">在设备处于展台模式时用于墙纸的可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="ffe19-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="ffe19-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="ffe19-215">kioskModeExitCode</span></span>|<span data-ttu-id="ffe19-216">String</span><span class="sxs-lookup"><span data-stu-id="ffe19-216">String</span></span>|<span data-ttu-id="ffe19-217">退出代码, 以允许用户在设备处于展台模式时从展台模式中进行转义。</span><span class="sxs-lookup"><span data-stu-id="ffe19-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="ffe19-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="ffe19-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="ffe19-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-219">Boolean</span></span>|<span data-ttu-id="ffe19-220">设备处于展台模式时是否显示虚拟 "主页" 按钮。</span><span class="sxs-lookup"><span data-stu-id="ffe19-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="ffe19-221">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="ffe19-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="ffe19-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-222">Boolean</span></span>|<span data-ttu-id="ffe19-223">是否允许用户在展台模式下配置蓝牙设置。</span><span class="sxs-lookup"><span data-stu-id="ffe19-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="ffe19-224">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="ffe19-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="ffe19-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-225">Boolean</span></span>|<span data-ttu-id="ffe19-226">是否允许用户在展台模式下配置 Wi-fi 设置。</span><span class="sxs-lookup"><span data-stu-id="ffe19-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="ffe19-227">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="ffe19-227">microphoneForceMute</span></span>|<span data-ttu-id="ffe19-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-228">Boolean</span></span>|<span data-ttu-id="ffe19-229">指示是否阻止观众在设备上的麦克风。</span><span class="sxs-lookup"><span data-stu-id="ffe19-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="ffe19-230">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="ffe19-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="ffe19-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-231">Boolean</span></span>|<span data-ttu-id="ffe19-232">指示在引导时设备是否允许连接到临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="ffe19-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="ffe19-233">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="ffe19-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="ffe19-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-234">Boolean</span></span>|<span data-ttu-id="ffe19-235">指示是否阻止 NFC 传出横梁。</span><span class="sxs-lookup"><span data-stu-id="ffe19-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="ffe19-236">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="ffe19-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="ffe19-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-237">Boolean</span></span>|<span data-ttu-id="ffe19-238">指示是否禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="ffe19-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="ffe19-239">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="ffe19-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="ffe19-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffe19-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="ffe19-241">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="ffe19-241">List of device keyguard features to block.</span></span> <span data-ttu-id="ffe19-242">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="ffe19-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="ffe19-243">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="ffe19-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ffe19-244">passwordExpirationDays</span></span>|<span data-ttu-id="ffe19-245">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-245">Int32</span></span>|<span data-ttu-id="ffe19-246">指示在密码过期之前可以设置密码的时间量 (以秒为单位) 以及需要新密码的时间 (以秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="ffe19-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="ffe19-247">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="ffe19-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ffe19-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ffe19-248">passwordMinimumLength</span></span>|<span data-ttu-id="ffe19-249">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-249">Int32</span></span>|<span data-ttu-id="ffe19-250">指示设备上所需密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="ffe19-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="ffe19-251">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="ffe19-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ffe19-252">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="ffe19-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="ffe19-253">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-253">Int32</span></span>|<span data-ttu-id="ffe19-254">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="ffe19-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="ffe19-255">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ffe19-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ffe19-256">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="ffe19-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="ffe19-257">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-257">Int32</span></span>|<span data-ttu-id="ffe19-258">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="ffe19-259">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ffe19-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ffe19-260">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="ffe19-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="ffe19-261">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-261">Int32</span></span>|<span data-ttu-id="ffe19-262">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="ffe19-263">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ffe19-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ffe19-264">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="ffe19-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="ffe19-265">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-265">Int32</span></span>|<span data-ttu-id="ffe19-266">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="ffe19-267">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ffe19-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ffe19-268">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="ffe19-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="ffe19-269">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-269">Int32</span></span>|<span data-ttu-id="ffe19-270">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="ffe19-271">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ffe19-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ffe19-272">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="ffe19-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="ffe19-273">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-273">Int32</span></span>|<span data-ttu-id="ffe19-274">指示设备密码所需的最小上限 caseletter 字符数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="ffe19-275">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ffe19-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ffe19-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ffe19-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ffe19-277">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-277">Int32</span></span>|<span data-ttu-id="ffe19-278">屏幕超时之前的不活动时间 (毫秒)。</span><span class="sxs-lookup"><span data-stu-id="ffe19-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ffe19-279">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="ffe19-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="ffe19-280">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-280">Int32</span></span>|<span data-ttu-id="ffe19-281">指示密码历史记录的长度, 其中用户将不能输入与历史记录中的任何密码相同的新密码。</span><span class="sxs-lookup"><span data-stu-id="ffe19-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="ffe19-282">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="ffe19-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ffe19-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ffe19-283">passwordRequiredType</span></span>|[<span data-ttu-id="ffe19-284">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ffe19-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="ffe19-285">指示设备上所需的最小密码质量。</span><span class="sxs-lookup"><span data-stu-id="ffe19-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="ffe19-286">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="ffe19-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ffe19-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ffe19-288">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-288">Int32</span></span>|<span data-ttu-id="ffe19-289">指示用户在擦除设备之前可以输入不正确密码的次数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="ffe19-290">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="ffe19-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ffe19-291">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="ffe19-291">playStoreMode</span></span>|[<span data-ttu-id="ffe19-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="ffe19-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="ffe19-293">指示设备的播放存储模式。</span><span class="sxs-lookup"><span data-stu-id="ffe19-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="ffe19-294">可取值为：`notConfigured`、`allowList`、`blockList`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="ffe19-295">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-295">safeBootBlocked</span></span>|<span data-ttu-id="ffe19-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-296">Boolean</span></span>|<span data-ttu-id="ffe19-297">指示是否禁用重新启动设备到安全启动。</span><span class="sxs-lookup"><span data-stu-id="ffe19-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="ffe19-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-298">screenCaptureBlocked</span></span>|<span data-ttu-id="ffe19-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-299">Boolean</span></span>|<span data-ttu-id="ffe19-300">指示是否禁用获取屏幕截图的功能。</span><span class="sxs-lookup"><span data-stu-id="ffe19-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="ffe19-301">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="ffe19-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="ffe19-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-302">Boolean</span></span>|<span data-ttu-id="ffe19-303">指示是否阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="ffe19-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="ffe19-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="ffe19-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="ffe19-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-305">Boolean</span></span>|<span data-ttu-id="ffe19-306">指示是否需要验证应用。</span><span class="sxs-lookup"><span data-stu-id="ffe19-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="ffe19-307">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-307">statusBarBlocked</span></span>|<span data-ttu-id="ffe19-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-308">Boolean</span></span>|<span data-ttu-id="ffe19-309">指示是否禁用状态栏, 包括通知、快速设置和其他屏幕重叠。</span><span class="sxs-lookup"><span data-stu-id="ffe19-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="ffe19-310">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="ffe19-310">stayOnModes</span></span>|<span data-ttu-id="ffe19-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffe19-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="ffe19-312">设备的显示将保持开机状态的模式列表。</span><span class="sxs-lookup"><span data-stu-id="ffe19-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="ffe19-313">此集合最多可包含4个元素。</span><span class="sxs-lookup"><span data-stu-id="ffe19-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="ffe19-314">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="ffe19-315">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="ffe19-315">storageAllowUsb</span></span>|<span data-ttu-id="ffe19-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-316">Boolean</span></span>|<span data-ttu-id="ffe19-317">指示是否允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="ffe19-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="ffe19-318">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="ffe19-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="ffe19-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-319">Boolean</span></span>|<span data-ttu-id="ffe19-320">指示是否阻止外部媒体。</span><span class="sxs-lookup"><span data-stu-id="ffe19-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="ffe19-321">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="ffe19-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="ffe19-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-322">Boolean</span></span>|<span data-ttu-id="ffe19-323">指示是否阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="ffe19-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="ffe19-324">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="ffe19-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="ffe19-325">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-325">Int32</span></span>|<span data-ttu-id="ffe19-326">指示系统更新窗口午夜后启动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="ffe19-327">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="ffe19-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="ffe19-328">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="ffe19-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="ffe19-329">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe19-329">Int32</span></span>|<span data-ttu-id="ffe19-330">指示系统更新窗口结束后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="ffe19-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="ffe19-331">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="ffe19-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="ffe19-332">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="ffe19-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="ffe19-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="ffe19-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="ffe19-334">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="ffe19-334">The type of system update configuration.</span></span> <span data-ttu-id="ffe19-335">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="ffe19-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="ffe19-336">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="ffe19-336">systemWindowsBlocked</span></span>|<span data-ttu-id="ffe19-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-337">Boolean</span></span>|<span data-ttu-id="ffe19-338">是否阻止 Android 系统提示符窗口, 如 toast、电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="ffe19-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="ffe19-339">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="ffe19-339">usersBlockAdd</span></span>|<span data-ttu-id="ffe19-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-340">Boolean</span></span>|<span data-ttu-id="ffe19-341">指示是否禁用添加用户和配置文件。</span><span class="sxs-lookup"><span data-stu-id="ffe19-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="ffe19-342">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="ffe19-342">usersBlockRemove</span></span>|<span data-ttu-id="ffe19-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-343">Boolean</span></span>|<span data-ttu-id="ffe19-344">指示是否禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="ffe19-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="ffe19-345">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="ffe19-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="ffe19-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-346">Boolean</span></span>|<span data-ttu-id="ffe19-347">指示是否禁用了调整主音量。</span><span class="sxs-lookup"><span data-stu-id="ffe19-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="ffe19-348">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="ffe19-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="ffe19-349">String</span><span class="sxs-lookup"><span data-stu-id="ffe19-349">String</span></span>|<span data-ttu-id="ffe19-350">将处理永不启用 VPN 连接的应用程序的 Android 应用程序包名称。</span><span class="sxs-lookup"><span data-stu-id="ffe19-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="ffe19-351">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="ffe19-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="ffe19-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-352">Boolean</span></span>|<span data-ttu-id="ffe19-353">如果指定了 always on VPN 包名称, 则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="ffe19-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="ffe19-354">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="ffe19-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="ffe19-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-355">Boolean</span></span>|<span data-ttu-id="ffe19-356">指示是否阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="ffe19-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="ffe19-357">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="ffe19-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="ffe19-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffe19-358">Boolean</span></span>|<span data-ttu-id="ffe19-359">指示是否阻止用户仅编辑策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="ffe19-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ffe19-360">响应</span><span class="sxs-lookup"><span data-stu-id="ffe19-360">Response</span></span>
<span data-ttu-id="ffe19-361">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffe19-361">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffe19-362">示例</span><span class="sxs-lookup"><span data-stu-id="ffe19-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffe19-363">请求</span><span class="sxs-lookup"><span data-stu-id="ffe19-363">Request</span></span>
<span data-ttu-id="ffe19-364">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffe19-364">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2905

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="ffe19-365">响应</span><span class="sxs-lookup"><span data-stu-id="ffe19-365">Response</span></span>
<span data-ttu-id="ffe19-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffe19-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3077

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




