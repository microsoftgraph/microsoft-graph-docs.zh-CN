---
title: 创建 androidDeviceOwnerGeneralDeviceConfiguration
description: 创建新的 androidDeviceOwnerGeneralDeviceConfiguration 对象。
ms.openlocfilehash: 0c95c47638378271d40f1c76327c1ea54e37e0cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048971"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="a2b9f-103">创建 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2b9f-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a2b9f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2b9f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2b9f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2b9f-107">创建新的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2b9f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2b9f-108">Prerequisites</span></span>
<span data-ttu-id="a2b9f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a2b9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b9f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2b9f-111">Permission type</span></span>|<span data-ttu-id="a2b9f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2b9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b9f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2b9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2b9f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b9f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-116">Not supported.</span></span>|
|<span data-ttu-id="a2b9f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2b9f-117">Application</span></span>|<span data-ttu-id="a2b9f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b9f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2b9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2b9f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2b9f-120">Request headers</span></span>
|<span data-ttu-id="a2b9f-121">标头</span><span class="sxs-lookup"><span data-stu-id="a2b9f-121">Header</span></span>|<span data-ttu-id="a2b9f-122">值</span><span class="sxs-lookup"><span data-stu-id="a2b9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2b9f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b9f-123">Authorization</span></span>|<span data-ttu-id="a2b9f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2b9f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2b9f-125">Accept</span></span>|<span data-ttu-id="a2b9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2b9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b9f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2b9f-127">Request body</span></span>
<span data-ttu-id="a2b9f-128">在请求正文中，提供 androidDeviceOwnerGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="a2b9f-129">下表显示时创建 androidDeviceOwnerGeneralDeviceConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="a2b9f-130">属性</span><span class="sxs-lookup"><span data-stu-id="a2b9f-130">Property</span></span>|<span data-ttu-id="a2b9f-131">类型</span><span class="sxs-lookup"><span data-stu-id="a2b9f-131">Type</span></span>|<span data-ttu-id="a2b9f-132">说明</span><span class="sxs-lookup"><span data-stu-id="a2b9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b9f-133">id</span><span class="sxs-lookup"><span data-stu-id="a2b9f-133">id</span></span>|<span data-ttu-id="a2b9f-134">String</span><span class="sxs-lookup"><span data-stu-id="a2b9f-134">String</span></span>|<span data-ttu-id="a2b9f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-135">Key of the entity.</span></span> <span data-ttu-id="a2b9f-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b9f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a2b9f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b9f-138">DateTimeOffset</span></span>|<span data-ttu-id="a2b9f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a2b9f-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2b9f-141">roleScopeTagIds</span></span>|<span data-ttu-id="a2b9f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2b9f-142">String collection</span></span>|<span data-ttu-id="a2b9f-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2b9f-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a2b9f-145">supportsScopeTags</span></span>|<span data-ttu-id="a2b9f-146">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-146">Boolean</span></span>|<span data-ttu-id="a2b9f-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a2b9f-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a2b9f-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a2b9f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-150">This property is read-only.</span></span> <span data-ttu-id="a2b9f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b9f-152">createdDateTime</span></span>|<span data-ttu-id="a2b9f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b9f-153">DateTimeOffset</span></span>|<span data-ttu-id="a2b9f-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-154">DateTime the object was created.</span></span> <span data-ttu-id="a2b9f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-156">description</span><span class="sxs-lookup"><span data-stu-id="a2b9f-156">description</span></span>|<span data-ttu-id="a2b9f-157">String</span><span class="sxs-lookup"><span data-stu-id="a2b9f-157">String</span></span>|<span data-ttu-id="a2b9f-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2b9f-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a2b9f-160">displayName</span></span>|<span data-ttu-id="a2b9f-161">String</span><span class="sxs-lookup"><span data-stu-id="a2b9f-161">String</span></span>|<span data-ttu-id="a2b9f-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2b9f-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-164">version</span><span class="sxs-lookup"><span data-stu-id="a2b9f-164">version</span></span>|<span data-ttu-id="a2b9f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-165">Int32</span></span>|<span data-ttu-id="a2b9f-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-166">Version of the device configuration.</span></span> <span data-ttu-id="a2b9f-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2b9f-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="a2b9f-168">accountsBlockModification</span></span>|<span data-ttu-id="a2b9f-169">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-169">Boolean</span></span>|<span data-ttu-id="a2b9f-170">指示添加或删除帐户被禁用。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="a2b9f-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a2b9f-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="a2b9f-172">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-172">Boolean</span></span>|<span data-ttu-id="a2b9f-173">指示允许用户启用到未知源设置。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="a2b9f-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="a2b9f-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="a2b9f-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="a2b9f-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="a2b9f-176">指示应用程序自动更新策略的值。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="a2b9f-177">可取值为：`notConfigured`、`userChoice`、`never`、`wiFiOnly`、`always`。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="a2b9f-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="a2b9f-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="a2b9f-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a2b9f-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="a2b9f-180">如果一个未定义应用程序专门，指示运行时权限请求的权限策略。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="a2b9f-181">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="a2b9f-182">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2b9f-182">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="a2b9f-183">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-183">Boolean</span></span>|<span data-ttu-id="a2b9f-184">指示阻止用户与配置蓝牙。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-184">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="a2b9f-185">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="a2b9f-185">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="a2b9f-186">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-186">Boolean</span></span>|<span data-ttu-id="a2b9f-187">指示阻止用户与共享通过蓝牙的联系人。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-187">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="a2b9f-188">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-188">cameraBlocked</span></span>|<span data-ttu-id="a2b9f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b9f-189">Boolean</span></span>|<span data-ttu-id="a2b9f-190">指示禁用照相机使用。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-190">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="a2b9f-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="a2b9f-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="a2b9f-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b9f-192">Boolean</span></span>|<span data-ttu-id="a2b9f-193">指示是否阻止 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-193">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="a2b9f-194">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-194">dataRoamingBlocked</span></span>|<span data-ttu-id="a2b9f-195">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-195">Boolean</span></span>|<span data-ttu-id="a2b9f-196">指示阻止用户与漫游数据。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-196">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="a2b9f-197">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-197">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="a2b9f-198">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-198">Boolean</span></span>|<span data-ttu-id="a2b9f-199">指示阻止用户手动更改日期或设备上的时间</span><span class="sxs-lookup"><span data-stu-id="a2b9f-199">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="a2b9f-200">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="a2b9f-200">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="a2b9f-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2b9f-201">String collection</span></span>|<span data-ttu-id="a2b9f-202">需要进行身份验证后设备出厂重置之前可以设置它的 Google 帐户电子邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-202">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="a2b9f-203">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-203">factoryResetBlocked</span></span>|<span data-ttu-id="a2b9f-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b9f-204">Boolean</span></span>|<span data-ttu-id="a2b9f-205">指示禁用中设置的出厂重置选项。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-205">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="a2b9f-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="a2b9f-206">kioskModeApps</span></span>|<span data-ttu-id="a2b9f-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2b9f-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a2b9f-208">将以展台模式，该设备时显示的托管应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-208">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="a2b9f-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a2b9f-210">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="a2b9f-210">microphoneForceMute</span></span>|<span data-ttu-id="a2b9f-211">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-211">Boolean</span></span>|<span data-ttu-id="a2b9f-212">指示阻止 unmuting 麦克风设备上。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-212">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="a2b9f-213">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="a2b9f-213">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="a2b9f-214">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-214">Boolean</span></span>|<span data-ttu-id="a2b9f-215">指示将允许设备连接到在启动时的临时网络连接。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-215">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="a2b9f-216">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="a2b9f-216">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="a2b9f-217">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-217">Boolean</span></span>|<span data-ttu-id="a2b9f-218">指示阻止 NFC 传出无线发送。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-218">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="a2b9f-219">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="a2b9f-219">passwordBlockKeyguard</span></span>|<span data-ttu-id="a2b9f-220">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-220">Boolean</span></span>|<span data-ttu-id="a2b9f-221">指示禁用 keyguard。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-221">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="a2b9f-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a2b9f-222">passwordExpirationDays</span></span>|<span data-ttu-id="a2b9f-223">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-223">Int32</span></span>|<span data-ttu-id="a2b9f-224">指示该帐户到期和新密码需要之前，可以为设置密码以秒为单位的时间量。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-224">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="a2b9f-225">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a2b9f-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2b9f-226">passwordMinimumLength</span></span>|<span data-ttu-id="a2b9f-227">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-227">Int32</span></span>|<span data-ttu-id="a2b9f-228">指示在设备上所需的密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-228">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="a2b9f-229">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="a2b9f-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a2b9f-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a2b9f-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a2b9f-231">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-231">Int32</span></span>|<span data-ttu-id="a2b9f-232">屏幕超时前的不活动毫秒。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-232">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a2b9f-233">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="a2b9f-233">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="a2b9f-234">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-234">Int32</span></span>|<span data-ttu-id="a2b9f-235">指示密码历史记录，其中用户将无法输入的历史记录中任何密码相同的新密码的长度。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-235">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="a2b9f-236">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="a2b9f-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a2b9f-237">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a2b9f-237">passwordRequiredType</span></span>|[<span data-ttu-id="a2b9f-238">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a2b9f-238">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="a2b9f-239">指示在设备上所需的最短密码质量。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-239">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="a2b9f-240">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-240">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a2b9f-241">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a2b9f-241">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a2b9f-242">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-242">Int32</span></span>|<span data-ttu-id="a2b9f-243">指示擦除设备之前，用户可以输入密码不正确的次数。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-243">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="a2b9f-244">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="a2b9f-244">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a2b9f-245">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-245">safeBootBlocked</span></span>|<span data-ttu-id="a2b9f-246">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-246">Boolean</span></span>|<span data-ttu-id="a2b9f-247">指示重新启动设备插入安全启动的被禁用。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-247">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="a2b9f-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-248">screenCaptureBlocked</span></span>|<span data-ttu-id="a2b9f-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b9f-249">Boolean</span></span>|<span data-ttu-id="a2b9f-250">指示禁用的功能，才能屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-250">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="a2b9f-251">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="a2b9f-251">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="a2b9f-252">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-252">Boolean</span></span>|<span data-ttu-id="a2b9f-253">指示阻止用户启用设备上的调试功能。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-253">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="a2b9f-254">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a2b9f-254">securityRequireVerifyApps</span></span>|<span data-ttu-id="a2b9f-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b9f-255">Boolean</span></span>|<span data-ttu-id="a2b9f-256">指示是否验证应用程序，则需要。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-256">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="a2b9f-257">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="a2b9f-257">statusBarBlocked</span></span>|<span data-ttu-id="a2b9f-258">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-258">Boolean</span></span>|<span data-ttu-id="a2b9f-259">指示是否或状态栏已禁用，包括通知、 快速设置和其他屏幕覆盖。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-259">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="a2b9f-260">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="a2b9f-260">stayOnModes</span></span>|<span data-ttu-id="a2b9f-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2b9f-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="a2b9f-262">在其中设备的显示将保持电模式的列表。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-262">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="a2b9f-263">4 元素的最多可以包含此集合。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-263">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="a2b9f-264">可取值为：`notConfigured`、`ac`、`usb`、`wireless`。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-264">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="a2b9f-265">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="a2b9f-265">storageAllowUsb</span></span>|<span data-ttu-id="a2b9f-266">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-266">Boolean</span></span>|<span data-ttu-id="a2b9f-267">指示允许 USB 大容量存储。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-267">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="a2b9f-268">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="a2b9f-268">storageBlockExternalMedia</span></span>|<span data-ttu-id="a2b9f-269">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-269">Boolean</span></span>|<span data-ttu-id="a2b9f-270">指示阻止外部介质。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-270">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="a2b9f-271">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="a2b9f-271">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="a2b9f-272">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-272">Boolean</span></span>|<span data-ttu-id="a2b9f-273">指示阻止 USB 文件传输。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-273">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="a2b9f-274">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="a2b9f-274">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="a2b9f-275">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-275">Int32</span></span>|<span data-ttu-id="a2b9f-276">指示系统更新窗口启动的午夜后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-276">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="a2b9f-277">0 到 1440 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="a2b9f-277">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="a2b9f-278">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="a2b9f-278">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="a2b9f-279">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b9f-279">Int32</span></span>|<span data-ttu-id="a2b9f-280">指示系统更新窗口结束的午夜后的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-280">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="a2b9f-281">0 到 1440 之间的有效值</span><span class="sxs-lookup"><span data-stu-id="a2b9f-281">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="a2b9f-282">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="a2b9f-282">systemUpdateInstallType</span></span>|[<span data-ttu-id="a2b9f-283">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="a2b9f-283">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="a2b9f-284">系统更新配置的类型。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-284">The type of system update configuration.</span></span> <span data-ttu-id="a2b9f-285">可取值为：`deviceDefault`、`postpone`、`windowed`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-285">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="a2b9f-286">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="a2b9f-286">usersBlockAdd</span></span>|<span data-ttu-id="a2b9f-287">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-287">Boolean</span></span>|<span data-ttu-id="a2b9f-288">指示将用户和配置文件添加被禁用。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-288">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="a2b9f-289">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="a2b9f-289">usersBlockRemove</span></span>|<span data-ttu-id="a2b9f-290">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-290">Boolean</span></span>|<span data-ttu-id="a2b9f-291">指示禁用从设备中删除其他用户。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-291">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="a2b9f-292">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="a2b9f-292">volumeBlockAdjustment</span></span>|<span data-ttu-id="a2b9f-293">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-293">Boolean</span></span>|<span data-ttu-id="a2b9f-294">指示调整主音量被禁用。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-294">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="a2b9f-295">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="a2b9f-295">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="a2b9f-296">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-296">Boolean</span></span>|<span data-ttu-id="a2b9f-297">指示阻止用户编辑 wifi 连接设置。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-297">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="a2b9f-298">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="a2b9f-298">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="a2b9f-299">布尔</span><span class="sxs-lookup"><span data-stu-id="a2b9f-299">Boolean</span></span>|<span data-ttu-id="a2b9f-300">指示阻止用户编辑只策略定义的网络。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-300">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="a2b9f-301">响应</span><span class="sxs-lookup"><span data-stu-id="a2b9f-301">Response</span></span>
<span data-ttu-id="a2b9f-302">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-302">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b9f-303">示例</span><span class="sxs-lookup"><span data-stu-id="a2b9f-303">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2b9f-304">请求</span><span class="sxs-lookup"><span data-stu-id="a2b9f-304">Request</span></span>
<span data-ttu-id="a2b9f-305">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-305">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2156

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="a2b9f-306">响应</span><span class="sxs-lookup"><span data-stu-id="a2b9f-306">Response</span></span>
<span data-ttu-id="a2b9f-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2b9f-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2264

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





