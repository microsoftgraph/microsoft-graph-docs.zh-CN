---
title: 更新 androidDeviceOwnerGeneralDeviceConfiguration
description: 更新 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2166acb42eeb5690486cd40f510416ce5a9a224
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395557"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="c294b-103">更新 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c294b-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c294b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c294b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c294b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c294b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c294b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c294b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c294b-107">更新[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c294b-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c294b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c294b-108">Prerequisites</span></span>
<span data-ttu-id="c294b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c294b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c294b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c294b-111">Permission type</span></span>|<span data-ttu-id="c294b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c294b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c294b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c294b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c294b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c294b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c294b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c294b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c294b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c294b-116">Not supported.</span></span>|
|<span data-ttu-id="c294b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c294b-117">Application</span></span>|<span data-ttu-id="c294b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c294b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c294b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c294b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c294b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c294b-120">Request headers</span></span>
|<span data-ttu-id="c294b-121">标头</span><span class="sxs-lookup"><span data-stu-id="c294b-121">Header</span></span>|<span data-ttu-id="c294b-122">值</span><span class="sxs-lookup"><span data-stu-id="c294b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c294b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c294b-123">Authorization</span></span>|<span data-ttu-id="c294b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c294b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c294b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c294b-125">Accept</span></span>|<span data-ttu-id="c294b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c294b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c294b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c294b-127">Request body</span></span>
<span data-ttu-id="c294b-128">在请求正文中，提供[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c294b-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="c294b-129">下表显示时创建[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c294b-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="c294b-130">属性</span><span class="sxs-lookup"><span data-stu-id="c294b-130">Property</span></span>|<span data-ttu-id="c294b-131">类型</span><span class="sxs-lookup"><span data-stu-id="c294b-131">Type</span></span>|<span data-ttu-id="c294b-132">说明</span><span class="sxs-lookup"><span data-stu-id="c294b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c294b-133">id</span><span class="sxs-lookup"><span data-stu-id="c294b-133">id</span></span>|<span data-ttu-id="c294b-134">String</span><span class="sxs-lookup"><span data-stu-id="c294b-134">String</span></span>|<span data-ttu-id="c294b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c294b-135">Key of the entity.</span></span> <span data-ttu-id="c294b-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c294b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c294b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c294b-138">DateTimeOffset</span></span>|<span data-ttu-id="c294b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c294b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c294b-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c294b-141">roleScopeTagIds</span></span>|<span data-ttu-id="c294b-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="c294b-142">String collection</span></span>|<span data-ttu-id="c294b-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="c294b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c294b-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c294b-145">supportsScopeTags</span></span>|<span data-ttu-id="c294b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-146">Boolean</span></span>|<span data-ttu-id="c294b-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="c294b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c294b-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c294b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c294b-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="c294b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c294b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c294b-150">This property is read-only.</span></span> <span data-ttu-id="c294b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c294b-152">createdDateTime</span></span>|<span data-ttu-id="c294b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c294b-153">DateTimeOffset</span></span>|<span data-ttu-id="c294b-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c294b-154">DateTime the object was created.</span></span> <span data-ttu-id="c294b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-156">description</span><span class="sxs-lookup"><span data-stu-id="c294b-156">description</span></span>|<span data-ttu-id="c294b-157">String</span><span class="sxs-lookup"><span data-stu-id="c294b-157">String</span></span>|<span data-ttu-id="c294b-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c294b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c294b-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c294b-160">displayName</span></span>|<span data-ttu-id="c294b-161">String</span><span class="sxs-lookup"><span data-stu-id="c294b-161">String</span></span>|<span data-ttu-id="c294b-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c294b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c294b-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-164">version</span><span class="sxs-lookup"><span data-stu-id="c294b-164">version</span></span>|<span data-ttu-id="c294b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-165">Int32</span></span>|<span data-ttu-id="c294b-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c294b-166">Version of the device configuration.</span></span> <span data-ttu-id="c294b-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c294b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c294b-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="c294b-168">accountsBlockModification</span></span>|<span data-ttu-id="c294b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-169">Boolean</span></span>|<span data-ttu-id="c294b-170">指示添加或删除帐户被禁用。</span><span class="sxs-lookup"><span data-stu-id="c294b-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="c294b-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c294b-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="c294b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-172">Boolean</span></span>|<span data-ttu-id="c294b-173">指示允许用户启用到未知源设置。</span><span class="sxs-lookup"><span data-stu-id="c294b-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="c294b-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="c294b-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="c294b-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="c294b-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="c294b-176">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="c294b-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="c294b-177">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="c294b-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="c294b-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="c294b-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="c294b-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="c294b-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="c294b-180">如果一个未定义应用程序专门，指示运行时权限请求的权限策略。</span><span class="sxs-lookup"><span data-stu-id="c294b-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="c294b-181">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="c294b-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="c294b-182">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="c294b-182">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="c294b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-183">Boolean</span></span>|<span data-ttu-id="c294b-184">建议所有应用程序，请跳过它们可能已添加任何首次使用提示。</span><span class="sxs-lookup"><span data-stu-id="c294b-184">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="c294b-185">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="c294b-185">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="c294b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-186">Boolean</span></span>|<span data-ttu-id="c294b-187">指示阻止用户与配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="c294b-187">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="c294b-188">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="c294b-188">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="c294b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-189">Boolean</span></span>|<span data-ttu-id="c294b-190">指示阻止用户与共享通过蓝牙的联系人。</span><span class="sxs-lookup"><span data-stu-id="c294b-190">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="c294b-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-191">cameraBlocked</span></span>|<span data-ttu-id="c294b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-192">Boolean</span></span>|<span data-ttu-id="c294b-193">指示禁用照相机使用。</span><span class="sxs-lookup"><span data-stu-id="c294b-193">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="c294b-194">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="c294b-194">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="c294b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-195">Boolean</span></span>|<span data-ttu-id="c294b-196">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="c294b-196">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="c294b-197">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-197">dataRoamingBlocked</span></span>|<span data-ttu-id="c294b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-198">Boolean</span></span>|<span data-ttu-id="c294b-199">指示阻止用户与漫游数据。</span><span class="sxs-lookup"><span data-stu-id="c294b-199">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="c294b-200">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-200">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="c294b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-201">Boolean</span></span>|<span data-ttu-id="c294b-202">指示阻止用户手动更改日期或设备上的时间</span><span class="sxs-lookup"><span data-stu-id="c294b-202">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="c294b-203">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="c294b-203">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="c294b-204">String 集合</span><span class="sxs-lookup"><span data-stu-id="c294b-204">String collection</span></span>|<span data-ttu-id="c294b-205">需要进行身份验证后设备出厂重置之前可以设置它的 Google 帐户电子邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="c294b-205">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="c294b-206">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-206">factoryResetBlocked</span></span>|<span data-ttu-id="c294b-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-207">Boolean</span></span>|<span data-ttu-id="c294b-208">指示禁用中设置的出厂重置选项。</span><span class="sxs-lookup"><span data-stu-id="c294b-208">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="c294b-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="c294b-209">kioskModeApps</span></span>|<span data-ttu-id="c294b-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c294b-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c294b-211">将以展台模式，该设备时显示的托管应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="c294b-211">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="c294b-212">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c294b-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c294b-213">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="c294b-213">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="c294b-214">String</span><span class="sxs-lookup"><span data-stu-id="c294b-214">String</span></span>|<span data-ttu-id="c294b-215">要以展台模式设备时，可用于墙纸可公开访问图像 URL。</span><span class="sxs-lookup"><span data-stu-id="c294b-215">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="c294b-216">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="c294b-216">kioskModeExitCode</span></span>|<span data-ttu-id="c294b-217">String</span><span class="sxs-lookup"><span data-stu-id="c294b-217">String</span></span>|<span data-ttu-id="c294b-218">退出代码以允许用户以展台模式设备时转义从展台模式。</span><span class="sxs-lookup"><span data-stu-id="c294b-218">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="c294b-219">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="c294b-219">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="c294b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-220">Boolean</span></span>|<span data-ttu-id="c294b-221">是否以展台模式设备时显示虚拟主页按钮。</span><span class="sxs-lookup"><span data-stu-id="c294b-221">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="c294b-222">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="c294b-222">microphoneForceMute</span></span>|<span data-ttu-id="c294b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-223">Boolean</span></span>|<span data-ttu-id="c294b-224">指示阻止 unmuting 麦克风设备上。</span><span class="sxs-lookup"><span data-stu-id="c294b-224">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="c294b-225">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="c294b-225">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="c294b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-226">Boolean</span></span>|<span data-ttu-id="c294b-227">指示将允许设备连接到在启动时的临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="c294b-227">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="c294b-228">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="c294b-228">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="c294b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-229">Boolean</span></span>|<span data-ttu-id="c294b-230">指示阻止 NFC 传出无线发送。</span><span class="sxs-lookup"><span data-stu-id="c294b-230">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="c294b-231">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="c294b-231">passwordBlockKeyguard</span></span>|<span data-ttu-id="c294b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-232">Boolean</span></span>|<span data-ttu-id="c294b-233">指示禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="c294b-233">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="c294b-234">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="c294b-234">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="c294b-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)集合</span><span class="sxs-lookup"><span data-stu-id="c294b-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="c294b-236">要阻止的设备 keyguard 功能的列表。</span><span class="sxs-lookup"><span data-stu-id="c294b-236">List of device keyguard features to block.</span></span> <span data-ttu-id="c294b-237">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="c294b-237">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="c294b-238">可取值为：`notConfigured`、`camera`、`notifications`、`unredactedNotifications`、`trustAgents`、`fingerprint`、`remoteInput`、`allFeatures`。</span><span class="sxs-lookup"><span data-stu-id="c294b-238">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="c294b-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c294b-239">passwordExpirationDays</span></span>|<span data-ttu-id="c294b-240">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-240">Int32</span></span>|<span data-ttu-id="c294b-241">指示该帐户到期和新密码需要之前，可以为设置密码以秒为单位的时间量。</span><span class="sxs-lookup"><span data-stu-id="c294b-241">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="c294b-242">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="c294b-242">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c294b-243">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c294b-243">passwordMinimumLength</span></span>|<span data-ttu-id="c294b-244">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-244">Int32</span></span>|<span data-ttu-id="c294b-245">指示在设备上所需的密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c294b-245">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="c294b-246">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="c294b-246">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c294b-247">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c294b-247">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c294b-248">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-248">Int32</span></span>|<span data-ttu-id="c294b-249">屏幕超时前的不活动毫秒。</span><span class="sxs-lookup"><span data-stu-id="c294b-249">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c294b-250">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="c294b-250">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="c294b-251">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-251">Int32</span></span>|<span data-ttu-id="c294b-252">指示密码历史记录，其中用户将无法输入的历史记录中任何密码相同的新密码的长度。</span><span class="sxs-lookup"><span data-stu-id="c294b-252">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="c294b-253">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="c294b-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c294b-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c294b-254">passwordRequiredType</span></span>|[<span data-ttu-id="c294b-255">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c294b-255">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="c294b-256">指示在设备上所需的最短密码质量。</span><span class="sxs-lookup"><span data-stu-id="c294b-256">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="c294b-257">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="c294b-257">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c294b-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c294b-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c294b-259">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-259">Int32</span></span>|<span data-ttu-id="c294b-260">指示擦除设备之前，用户可以输入密码不正确的次数。</span><span class="sxs-lookup"><span data-stu-id="c294b-260">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="c294b-261">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="c294b-261">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c294b-262">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-262">safeBootBlocked</span></span>|<span data-ttu-id="c294b-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-263">Boolean</span></span>|<span data-ttu-id="c294b-264">指示重新启动设备插入安全启动的被禁用。</span><span class="sxs-lookup"><span data-stu-id="c294b-264">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="c294b-265">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-265">screenCaptureBlocked</span></span>|<span data-ttu-id="c294b-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-266">Boolean</span></span>|<span data-ttu-id="c294b-267">指示禁用的功能，才能屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="c294b-267">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="c294b-268">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="c294b-268">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="c294b-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-269">Boolean</span></span>|<span data-ttu-id="c294b-270">指示阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="c294b-270">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="c294b-271">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c294b-271">securityRequireVerifyApps</span></span>|<span data-ttu-id="c294b-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-272">Boolean</span></span>|<span data-ttu-id="c294b-273">指示是否验证应用程序，则需要。</span><span class="sxs-lookup"><span data-stu-id="c294b-273">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="c294b-274">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-274">statusBarBlocked</span></span>|<span data-ttu-id="c294b-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-275">Boolean</span></span>|<span data-ttu-id="c294b-276">指示是否或状态栏已禁用，包括通知、 快速设置和其他屏幕覆盖。</span><span class="sxs-lookup"><span data-stu-id="c294b-276">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="c294b-277">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="c294b-277">stayOnModes</span></span>|<span data-ttu-id="c294b-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="c294b-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="c294b-279">在其中设备的显示将保持电模式的列表。</span><span class="sxs-lookup"><span data-stu-id="c294b-279">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="c294b-280">4 元素的最多可以包含此集合。</span><span class="sxs-lookup"><span data-stu-id="c294b-280">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="c294b-281">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="c294b-281">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="c294b-282">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="c294b-282">storageAllowUsb</span></span>|<span data-ttu-id="c294b-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-283">Boolean</span></span>|<span data-ttu-id="c294b-284">指示允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="c294b-284">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="c294b-285">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="c294b-285">storageBlockExternalMedia</span></span>|<span data-ttu-id="c294b-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-286">Boolean</span></span>|<span data-ttu-id="c294b-287">指示阻止外部介质。</span><span class="sxs-lookup"><span data-stu-id="c294b-287">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="c294b-288">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="c294b-288">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="c294b-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-289">Boolean</span></span>|<span data-ttu-id="c294b-290">指示阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="c294b-290">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="c294b-291">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="c294b-291">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="c294b-292">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-292">Int32</span></span>|<span data-ttu-id="c294b-293">指示系统更新窗口启动的午夜后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c294b-293">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="c294b-294">0 到 1440 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="c294b-294">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="c294b-295">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="c294b-295">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="c294b-296">Int32</span><span class="sxs-lookup"><span data-stu-id="c294b-296">Int32</span></span>|<span data-ttu-id="c294b-297">指示系统更新窗口结束的午夜后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c294b-297">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="c294b-298">0 到 1440 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="c294b-298">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="c294b-299">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="c294b-299">systemUpdateInstallType</span></span>|[<span data-ttu-id="c294b-300">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="c294b-300">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="c294b-301">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="c294b-301">The type of system update configuration.</span></span> <span data-ttu-id="c294b-302">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="c294b-302">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="c294b-303">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="c294b-303">systemWindowsBlocked</span></span>|<span data-ttu-id="c294b-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-304">Boolean</span></span>|<span data-ttu-id="c294b-305">阻止 Android 系统提示窗口中的，如 toast、 电话活动和系统通知。</span><span class="sxs-lookup"><span data-stu-id="c294b-305">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="c294b-306">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="c294b-306">usersBlockAdd</span></span>|<span data-ttu-id="c294b-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-307">Boolean</span></span>|<span data-ttu-id="c294b-308">指示将用户和配置文件添加被禁用。</span><span class="sxs-lookup"><span data-stu-id="c294b-308">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="c294b-309">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="c294b-309">usersBlockRemove</span></span>|<span data-ttu-id="c294b-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-310">Boolean</span></span>|<span data-ttu-id="c294b-311">指示禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="c294b-311">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="c294b-312">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="c294b-312">volumeBlockAdjustment</span></span>|<span data-ttu-id="c294b-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-313">Boolean</span></span>|<span data-ttu-id="c294b-314">指示调整主音量被禁用。</span><span class="sxs-lookup"><span data-stu-id="c294b-314">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="c294b-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="c294b-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="c294b-316">String</span><span class="sxs-lookup"><span data-stu-id="c294b-316">String</span></span>|<span data-ttu-id="c294b-317">在 android 应用包将用来处理始终打开的 VPN 连接的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="c294b-317">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="c294b-318">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="c294b-318">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="c294b-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-319">Boolean</span></span>|<span data-ttu-id="c294b-320">如果始终在 VPN 包名称指定了，锁定网络流量时断开连接的 VPN。</span><span class="sxs-lookup"><span data-stu-id="c294b-320">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="c294b-321">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="c294b-321">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="c294b-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-322">Boolean</span></span>|<span data-ttu-id="c294b-323">指示阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="c294b-323">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="c294b-324">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="c294b-324">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="c294b-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="c294b-325">Boolean</span></span>|<span data-ttu-id="c294b-326">指示阻止用户编辑只策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="c294b-326">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="c294b-327">响应</span><span class="sxs-lookup"><span data-stu-id="c294b-327">Response</span></span>
<span data-ttu-id="c294b-328">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c294b-328">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c294b-329">示例</span><span class="sxs-lookup"><span data-stu-id="c294b-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="c294b-330">请求</span><span class="sxs-lookup"><span data-stu-id="c294b-330">Request</span></span>
<span data-ttu-id="c294b-331">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c294b-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2517

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="c294b-332">响应</span><span class="sxs-lookup"><span data-stu-id="c294b-332">Response</span></span>
<span data-ttu-id="c294b-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c294b-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2689

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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




