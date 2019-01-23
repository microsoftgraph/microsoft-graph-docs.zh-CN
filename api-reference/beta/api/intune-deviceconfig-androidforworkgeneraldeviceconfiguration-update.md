---
title: 更新 androidForWorkGeneralDeviceConfiguration
description: 更新 androidForWorkGeneralDeviceConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4f76cea5a5d0f4949ad581da8b73857391859d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395417"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="30d60-103">更新 androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="30d60-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="30d60-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="30d60-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30d60-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="30d60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30d60-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30d60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30d60-107">更新[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30d60-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30d60-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="30d60-108">Prerequisites</span></span>
<span data-ttu-id="30d60-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="30d60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="30d60-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30d60-111">Permission type</span></span>|<span data-ttu-id="30d60-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30d60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30d60-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30d60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30d60-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30d60-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30d60-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30d60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30d60-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30d60-116">Not supported.</span></span>|
|<span data-ttu-id="30d60-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="30d60-117">Application</span></span>|<span data-ttu-id="30d60-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="30d60-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30d60-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30d60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="30d60-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="30d60-120">Request headers</span></span>
|<span data-ttu-id="30d60-121">标头</span><span class="sxs-lookup"><span data-stu-id="30d60-121">Header</span></span>|<span data-ttu-id="30d60-122">值</span><span class="sxs-lookup"><span data-stu-id="30d60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30d60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30d60-123">Authorization</span></span>|<span data-ttu-id="30d60-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30d60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30d60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30d60-125">Accept</span></span>|<span data-ttu-id="30d60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30d60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30d60-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="30d60-127">Request body</span></span>
<span data-ttu-id="30d60-128">在请求正文中，提供[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30d60-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="30d60-129">下表显示时创建[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="30d60-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="30d60-130">属性</span><span class="sxs-lookup"><span data-stu-id="30d60-130">Property</span></span>|<span data-ttu-id="30d60-131">类型</span><span class="sxs-lookup"><span data-stu-id="30d60-131">Type</span></span>|<span data-ttu-id="30d60-132">说明</span><span class="sxs-lookup"><span data-stu-id="30d60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d60-133">id</span><span class="sxs-lookup"><span data-stu-id="30d60-133">id</span></span>|<span data-ttu-id="30d60-134">String</span><span class="sxs-lookup"><span data-stu-id="30d60-134">String</span></span>|<span data-ttu-id="30d60-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30d60-135">Key of the entity.</span></span> <span data-ttu-id="30d60-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d60-137">lastModifiedDateTime</span></span>|<span data-ttu-id="30d60-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d60-138">DateTimeOffset</span></span>|<span data-ttu-id="30d60-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="30d60-139">DateTime the object was last modified.</span></span> <span data-ttu-id="30d60-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30d60-141">roleScopeTagIds</span></span>|<span data-ttu-id="30d60-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="30d60-142">String collection</span></span>|<span data-ttu-id="30d60-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="30d60-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="30d60-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="30d60-145">supportsScopeTags</span></span>|<span data-ttu-id="30d60-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-146">Boolean</span></span>|<span data-ttu-id="30d60-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="30d60-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="30d60-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="30d60-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="30d60-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="30d60-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="30d60-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="30d60-150">This property is read-only.</span></span> <span data-ttu-id="30d60-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30d60-152">createdDateTime</span></span>|<span data-ttu-id="30d60-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d60-153">DateTimeOffset</span></span>|<span data-ttu-id="30d60-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="30d60-154">DateTime the object was created.</span></span> <span data-ttu-id="30d60-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-156">description</span><span class="sxs-lookup"><span data-stu-id="30d60-156">description</span></span>|<span data-ttu-id="30d60-157">String</span><span class="sxs-lookup"><span data-stu-id="30d60-157">String</span></span>|<span data-ttu-id="30d60-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="30d60-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="30d60-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-160">displayName</span><span class="sxs-lookup"><span data-stu-id="30d60-160">displayName</span></span>|<span data-ttu-id="30d60-161">String</span><span class="sxs-lookup"><span data-stu-id="30d60-161">String</span></span>|<span data-ttu-id="30d60-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="30d60-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="30d60-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-164">version</span><span class="sxs-lookup"><span data-stu-id="30d60-164">version</span></span>|<span data-ttu-id="30d60-165">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-165">Int32</span></span>|<span data-ttu-id="30d60-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="30d60-166">Version of the device configuration.</span></span> <span data-ttu-id="30d60-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d60-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d60-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="30d60-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="30d60-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-169">Boolean</span></span>|<span data-ttu-id="30d60-170">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="30d60-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="30d60-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="30d60-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="30d60-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-172">Boolean</span></span>|<span data-ttu-id="30d60-173">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="30d60-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="30d60-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="30d60-174">passwordExpirationDays</span></span>|<span data-ttu-id="30d60-175">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-175">Int32</span></span>|<span data-ttu-id="30d60-176">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="30d60-176">Number of days before the password expires.</span></span> <span data-ttu-id="30d60-177">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="30d60-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="30d60-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="30d60-178">passwordMinimumLength</span></span>|<span data-ttu-id="30d60-179">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-179">Int32</span></span>|<span data-ttu-id="30d60-180">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="30d60-180">Minimum length of passwords.</span></span> <span data-ttu-id="30d60-181">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="30d60-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="30d60-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="30d60-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="30d60-183">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-183">Int32</span></span>|<span data-ttu-id="30d60-184">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="30d60-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="30d60-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="30d60-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="30d60-186">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-186">Int32</span></span>|<span data-ttu-id="30d60-187">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="30d60-187">Number of previous passwords to block.</span></span> <span data-ttu-id="30d60-188">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="30d60-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="30d60-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="30d60-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="30d60-190">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-190">Int32</span></span>|<span data-ttu-id="30d60-191">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="30d60-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="30d60-192">有效的值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="30d60-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="30d60-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="30d60-193">passwordRequiredType</span></span>|[<span data-ttu-id="30d60-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="30d60-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="30d60-195">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="30d60-195">Type of password that is required.</span></span> <span data-ttu-id="30d60-196">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="30d60-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="30d60-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="30d60-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="30d60-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="30d60-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="30d60-199">允许共享的数据的类型。</span><span class="sxs-lookup"><span data-stu-id="30d60-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="30d60-200">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="30d60-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="30d60-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="30d60-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="30d60-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-202">Boolean</span></span>|<span data-ttu-id="30d60-203">指示阻止通知时设备锁定。</span><span class="sxs-lookup"><span data-stu-id="30d60-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="30d60-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="30d60-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="30d60-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-205">Boolean</span></span>|<span data-ttu-id="30d60-206">阻止用户添加/移除工作配置文件中的帐户。</span><span class="sxs-lookup"><span data-stu-id="30d60-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="30d60-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="30d60-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="30d60-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-208">Boolean</span></span>|<span data-ttu-id="30d60-209">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="30d60-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="30d60-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="30d60-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="30d60-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-211">Boolean</span></span>|<span data-ttu-id="30d60-212">阻止工作配置文件中的屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="30d60-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="30d60-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="30d60-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="30d60-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-214">Boolean</span></span>|<span data-ttu-id="30d60-215">阻止显示工作 profile 呼叫者 ID 个人配置文件中。</span><span class="sxs-lookup"><span data-stu-id="30d60-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="30d60-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="30d60-216">workProfileBlockCamera</span></span>|<span data-ttu-id="30d60-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-217">Boolean</span></span>|<span data-ttu-id="30d60-218">阻止工作 profile 摄像头。</span><span class="sxs-lookup"><span data-stu-id="30d60-218">Block work profile camera.</span></span>|
|<span data-ttu-id="30d60-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="30d60-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="30d60-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-220">Boolean</span></span>|<span data-ttu-id="30d60-221">个人配置文件中，阻止工作 profile 联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="30d60-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="30d60-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="30d60-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="30d60-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-223">Boolean</span></span>|<span data-ttu-id="30d60-224">布尔值，指示设置不允许跨是否启用配置文件复制/粘贴。</span><span class="sxs-lookup"><span data-stu-id="30d60-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="30d60-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="30d60-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="30d60-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="30d60-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="30d60-227">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="30d60-227">Type of password that is required.</span></span> <span data-ttu-id="30d60-228">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="30d60-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="30d60-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="30d60-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="30d60-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-230">Boolean</span></span>|<span data-ttu-id="30d60-231">指示是否阻止指纹解锁工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="30d60-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="30d60-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="30d60-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="30d60-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-233">Boolean</span></span>|<span data-ttu-id="30d60-234">指示阻止智能锁定和其他信任代理工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="30d60-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="30d60-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="30d60-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="30d60-236">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-236">Int32</span></span>|<span data-ttu-id="30d60-237">过期工作配置文件密码之前的天数。</span><span class="sxs-lookup"><span data-stu-id="30d60-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="30d60-238">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="30d60-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="30d60-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="30d60-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="30d60-240">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-240">Int32</span></span>|<span data-ttu-id="30d60-241">工作配置文件密码最小长度。</span><span class="sxs-lookup"><span data-stu-id="30d60-241">Minimum length of work profile password.</span></span> <span data-ttu-id="30d60-242">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="30d60-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="30d60-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="30d60-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="30d60-244">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-244">Int32</span></span>|<span data-ttu-id="30d60-245">最小 ハ  工作配置文件密码中所需的数字字符。</span><span class="sxs-lookup"><span data-stu-id="30d60-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="30d60-246">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="30d60-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="30d60-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="30d60-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="30d60-248">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-248">Int32</span></span>|<span data-ttu-id="30d60-249">最小 ハ  中工作配置文件密码必须包含非字母字符。</span><span class="sxs-lookup"><span data-stu-id="30d60-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="30d60-250">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="30d60-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="30d60-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="30d60-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="30d60-252">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-252">Int32</span></span>|<span data-ttu-id="30d60-253">最小 ハ  中工作配置文件密码必须包含字母字符。</span><span class="sxs-lookup"><span data-stu-id="30d60-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="30d60-254">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="30d60-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="30d60-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="30d60-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="30d60-256">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-256">Int32</span></span>|<span data-ttu-id="30d60-257">最小 ハ  工作配置文件密码中需要的小写字符。</span><span class="sxs-lookup"><span data-stu-id="30d60-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="30d60-258">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="30d60-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="30d60-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="30d60-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="30d60-260">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-260">Int32</span></span>|<span data-ttu-id="30d60-261">最小 ハ  中工作配置文件密码必须大写字符。</span><span class="sxs-lookup"><span data-stu-id="30d60-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="30d60-262">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="30d60-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="30d60-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="30d60-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="30d60-264">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-264">Int32</span></span>|<span data-ttu-id="30d60-265">最小 ハ  工作配置文件密码中需要的符号。</span><span class="sxs-lookup"><span data-stu-id="30d60-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="30d60-266">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="30d60-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="30d60-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="30d60-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="30d60-268">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-268">Int32</span></span>|<span data-ttu-id="30d60-269">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="30d60-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="30d60-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="30d60-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="30d60-271">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-271">Int32</span></span>|<span data-ttu-id="30d60-272">以前的工作配置文件密码，以阻止数。</span><span class="sxs-lookup"><span data-stu-id="30d60-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="30d60-273">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="30d60-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="30d60-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="30d60-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="30d60-275">Int32</span><span class="sxs-lookup"><span data-stu-id="30d60-275">Int32</span></span>|<span data-ttu-id="30d60-276">登录失败之前删除工作配置文件允许和已删除的所有企业数据的数量。</span><span class="sxs-lookup"><span data-stu-id="30d60-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="30d60-277">有效的值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="30d60-277">Valid values 1 to 16</span></span>|
|<span data-ttu-id="30d60-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="30d60-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="30d60-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="30d60-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="30d60-280">工作所需的配置文件密码的类型。</span><span class="sxs-lookup"><span data-stu-id="30d60-280">Type of work profile password that is required.</span></span> <span data-ttu-id="30d60-281">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="30d60-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="30d60-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="30d60-282">workProfileRequirePassword</span></span>|<span data-ttu-id="30d60-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-283">Boolean</span></span>|<span data-ttu-id="30d60-284">密码，则需要或不工作配置文件</span><span class="sxs-lookup"><span data-stu-id="30d60-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="30d60-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="30d60-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="30d60-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-286">Boolean</span></span>|<span data-ttu-id="30d60-287">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="30d60-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="30d60-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="30d60-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="30d60-289">String</span><span class="sxs-lookup"><span data-stu-id="30d60-289">String</span></span>|<span data-ttu-id="30d60-290">始终在 VPN 中启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="30d60-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="30d60-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="30d60-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="30d60-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d60-292">Boolean</span></span>|<span data-ttu-id="30d60-293">始终在 VPN 中启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="30d60-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="30d60-294">响应</span><span class="sxs-lookup"><span data-stu-id="30d60-294">Response</span></span>
<span data-ttu-id="30d60-295">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="30d60-295">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30d60-296">示例</span><span class="sxs-lookup"><span data-stu-id="30d60-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="30d60-297">请求</span><span class="sxs-lookup"><span data-stu-id="30d60-297">Request</span></span>
<span data-ttu-id="30d60-298">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30d60-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2038

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="30d60-299">响应</span><span class="sxs-lookup"><span data-stu-id="30d60-299">Response</span></span>
<span data-ttu-id="30d60-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30d60-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2210

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```




