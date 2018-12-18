---
title: 更新 androidForWorkGeneralDeviceConfiguration
description: 更新 androidForWorkGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: 09f4dd4d17e00ec3515144ad925beeab971ac5a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338526"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="d7a73-103">更新 androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d7a73-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d7a73-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d7a73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7a73-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d7a73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7a73-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d7a73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7a73-107">更新[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7a73-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7a73-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d7a73-108">Prerequisites</span></span>
<span data-ttu-id="d7a73-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d7a73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7a73-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7a73-111">Permission type</span></span>|<span data-ttu-id="d7a73-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7a73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7a73-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7a73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7a73-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a73-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7a73-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7a73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7a73-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7a73-116">Not supported.</span></span>|
|<span data-ttu-id="d7a73-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7a73-117">Application</span></span>|<span data-ttu-id="d7a73-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7a73-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7a73-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7a73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d7a73-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7a73-120">Request headers</span></span>
|<span data-ttu-id="d7a73-121">标头</span><span class="sxs-lookup"><span data-stu-id="d7a73-121">Header</span></span>|<span data-ttu-id="d7a73-122">值</span><span class="sxs-lookup"><span data-stu-id="d7a73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7a73-123">授权</span><span class="sxs-lookup"><span data-stu-id="d7a73-123">Authorization</span></span>|<span data-ttu-id="d7a73-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d7a73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7a73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7a73-125">Accept</span></span>|<span data-ttu-id="d7a73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7a73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7a73-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7a73-127">Request body</span></span>
<span data-ttu-id="d7a73-128">在请求正文中，提供[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7a73-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="d7a73-129">下表显示时创建[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d7a73-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="d7a73-130">属性</span><span class="sxs-lookup"><span data-stu-id="d7a73-130">Property</span></span>|<span data-ttu-id="d7a73-131">类型</span><span class="sxs-lookup"><span data-stu-id="d7a73-131">Type</span></span>|<span data-ttu-id="d7a73-132">说明</span><span class="sxs-lookup"><span data-stu-id="d7a73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7a73-133">id</span><span class="sxs-lookup"><span data-stu-id="d7a73-133">id</span></span>|<span data-ttu-id="d7a73-134">String</span><span class="sxs-lookup"><span data-stu-id="d7a73-134">String</span></span>|<span data-ttu-id="d7a73-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d7a73-135">Key of the entity.</span></span> <span data-ttu-id="d7a73-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7a73-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d7a73-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7a73-138">DateTimeOffset</span></span>|<span data-ttu-id="d7a73-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d7a73-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d7a73-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7a73-141">roleScopeTagIds</span></span>|<span data-ttu-id="d7a73-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d7a73-142">String collection</span></span>|<span data-ttu-id="d7a73-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d7a73-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7a73-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d7a73-145">supportsScopeTags</span></span>|<span data-ttu-id="d7a73-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-146">Boolean</span></span>|<span data-ttu-id="d7a73-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d7a73-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7a73-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d7a73-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7a73-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d7a73-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7a73-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d7a73-150">This property is read-only.</span></span> <span data-ttu-id="d7a73-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7a73-152">createdDateTime</span></span>|<span data-ttu-id="d7a73-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7a73-153">DateTimeOffset</span></span>|<span data-ttu-id="d7a73-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d7a73-154">DateTime the object was created.</span></span> <span data-ttu-id="d7a73-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-156">description</span><span class="sxs-lookup"><span data-stu-id="d7a73-156">description</span></span>|<span data-ttu-id="d7a73-157">String</span><span class="sxs-lookup"><span data-stu-id="d7a73-157">String</span></span>|<span data-ttu-id="d7a73-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d7a73-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7a73-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d7a73-160">displayName</span></span>|<span data-ttu-id="d7a73-161">String</span><span class="sxs-lookup"><span data-stu-id="d7a73-161">String</span></span>|<span data-ttu-id="d7a73-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d7a73-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7a73-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-164">version</span><span class="sxs-lookup"><span data-stu-id="d7a73-164">version</span></span>|<span data-ttu-id="d7a73-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-165">Int32</span></span>|<span data-ttu-id="d7a73-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d7a73-166">Version of the device configuration.</span></span> <span data-ttu-id="d7a73-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7a73-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7a73-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d7a73-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d7a73-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-169">Boolean</span></span>|<span data-ttu-id="d7a73-170">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="d7a73-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d7a73-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d7a73-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="d7a73-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-172">Boolean</span></span>|<span data-ttu-id="d7a73-173">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="d7a73-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="d7a73-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d7a73-174">passwordExpirationDays</span></span>|<span data-ttu-id="d7a73-175">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-175">Int32</span></span>|<span data-ttu-id="d7a73-176">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="d7a73-176">Number of days before the password expires.</span></span> <span data-ttu-id="d7a73-177">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="d7a73-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d7a73-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d7a73-178">passwordMinimumLength</span></span>|<span data-ttu-id="d7a73-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-179">Int32</span></span>|<span data-ttu-id="d7a73-180">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="d7a73-180">Minimum length of passwords.</span></span> <span data-ttu-id="d7a73-181">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="d7a73-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d7a73-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d7a73-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d7a73-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-183">Int32</span></span>|<span data-ttu-id="d7a73-184">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="d7a73-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d7a73-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d7a73-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d7a73-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-186">Int32</span></span>|<span data-ttu-id="d7a73-187">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="d7a73-187">Number of previous passwords to block.</span></span> <span data-ttu-id="d7a73-188">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="d7a73-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d7a73-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d7a73-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d7a73-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-190">Int32</span></span>|<span data-ttu-id="d7a73-191">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="d7a73-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="d7a73-192">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="d7a73-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d7a73-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d7a73-193">passwordRequiredType</span></span>|[<span data-ttu-id="d7a73-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d7a73-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="d7a73-195">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d7a73-195">Type of password that is required.</span></span> <span data-ttu-id="d7a73-196">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="d7a73-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d7a73-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d7a73-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="d7a73-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="d7a73-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="d7a73-199">允许共享的数据的类型。</span><span class="sxs-lookup"><span data-stu-id="d7a73-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="d7a73-200">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="d7a73-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="d7a73-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="d7a73-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="d7a73-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-202">Boolean</span></span>|<span data-ttu-id="d7a73-203">指示阻止通知时设备锁定。</span><span class="sxs-lookup"><span data-stu-id="d7a73-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="d7a73-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="d7a73-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="d7a73-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-205">Boolean</span></span>|<span data-ttu-id="d7a73-206">阻止用户添加/移除工作配置文件中的帐户。</span><span class="sxs-lookup"><span data-stu-id="d7a73-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="d7a73-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="d7a73-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="d7a73-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-208">Boolean</span></span>|<span data-ttu-id="d7a73-209">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="d7a73-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="d7a73-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="d7a73-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="d7a73-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-211">Boolean</span></span>|<span data-ttu-id="d7a73-212">阻止工作配置文件中的屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="d7a73-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="d7a73-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="d7a73-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="d7a73-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-214">Boolean</span></span>|<span data-ttu-id="d7a73-215">阻止显示工作 profile 呼叫者 ID 个人配置文件中。</span><span class="sxs-lookup"><span data-stu-id="d7a73-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="d7a73-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="d7a73-216">workProfileBlockCamera</span></span>|<span data-ttu-id="d7a73-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-217">Boolean</span></span>|<span data-ttu-id="d7a73-218">阻止工作 profile 摄像头。</span><span class="sxs-lookup"><span data-stu-id="d7a73-218">Block work profile camera.</span></span>|
|<span data-ttu-id="d7a73-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="d7a73-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="d7a73-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-220">Boolean</span></span>|<span data-ttu-id="d7a73-221">个人配置文件中，阻止工作 profile 联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="d7a73-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="d7a73-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="d7a73-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="d7a73-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-223">Boolean</span></span>|<span data-ttu-id="d7a73-224">布尔值，指示设置不允许跨是否启用配置文件复制/粘贴。</span><span class="sxs-lookup"><span data-stu-id="d7a73-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="d7a73-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="d7a73-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="d7a73-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="d7a73-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="d7a73-227">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d7a73-227">Type of password that is required.</span></span> <span data-ttu-id="d7a73-228">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="d7a73-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="d7a73-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d7a73-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d7a73-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-230">Boolean</span></span>|<span data-ttu-id="d7a73-231">指示是否阻止指纹解锁工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="d7a73-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="d7a73-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d7a73-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="d7a73-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-233">Boolean</span></span>|<span data-ttu-id="d7a73-234">指示阻止智能锁定和其他信任代理工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="d7a73-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="d7a73-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d7a73-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="d7a73-236">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-236">Int32</span></span>|<span data-ttu-id="d7a73-237">过期工作配置文件密码之前的天数。</span><span class="sxs-lookup"><span data-stu-id="d7a73-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="d7a73-238">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="d7a73-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d7a73-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d7a73-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="d7a73-240">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-240">Int32</span></span>|<span data-ttu-id="d7a73-241">工作配置文件密码最小长度。</span><span class="sxs-lookup"><span data-stu-id="d7a73-241">Minimum length of work profile password.</span></span> <span data-ttu-id="d7a73-242">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="d7a73-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d7a73-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="d7a73-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="d7a73-244">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-244">Int32</span></span>|<span data-ttu-id="d7a73-245">最小 ハ  工作配置文件密码中所需的数字字符。</span><span class="sxs-lookup"><span data-stu-id="d7a73-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="d7a73-246">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="d7a73-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7a73-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d7a73-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="d7a73-248">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-248">Int32</span></span>|<span data-ttu-id="d7a73-249">最小 ハ  中工作配置文件密码必须包含非字母字符。</span><span class="sxs-lookup"><span data-stu-id="d7a73-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="d7a73-250">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="d7a73-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7a73-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="d7a73-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="d7a73-252">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-252">Int32</span></span>|<span data-ttu-id="d7a73-253">最小 ハ  中工作配置文件密码必须包含字母字符。</span><span class="sxs-lookup"><span data-stu-id="d7a73-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="d7a73-254">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="d7a73-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7a73-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d7a73-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="d7a73-256">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-256">Int32</span></span>|<span data-ttu-id="d7a73-257">最小 ハ  工作配置文件密码中需要的小写字符。</span><span class="sxs-lookup"><span data-stu-id="d7a73-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="d7a73-258">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="d7a73-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7a73-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="d7a73-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="d7a73-260">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-260">Int32</span></span>|<span data-ttu-id="d7a73-261">最小 ハ  中工作配置文件密码必须大写字符。</span><span class="sxs-lookup"><span data-stu-id="d7a73-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="d7a73-262">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="d7a73-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7a73-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="d7a73-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="d7a73-264">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-264">Int32</span></span>|<span data-ttu-id="d7a73-265">最小 ハ  工作配置文件密码中需要的符号。</span><span class="sxs-lookup"><span data-stu-id="d7a73-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="d7a73-266">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="d7a73-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="d7a73-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d7a73-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d7a73-268">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-268">Int32</span></span>|<span data-ttu-id="d7a73-269">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="d7a73-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d7a73-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d7a73-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d7a73-271">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-271">Int32</span></span>|<span data-ttu-id="d7a73-272">以前的工作配置文件密码，以阻止数。</span><span class="sxs-lookup"><span data-stu-id="d7a73-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="d7a73-273">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="d7a73-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d7a73-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d7a73-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d7a73-275">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a73-275">Int32</span></span>|<span data-ttu-id="d7a73-276">登录失败之前删除工作配置文件允许和已删除的所有企业数据的数量。</span><span class="sxs-lookup"><span data-stu-id="d7a73-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="d7a73-277">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="d7a73-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d7a73-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d7a73-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="d7a73-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d7a73-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="d7a73-280">工作所需的配置文件密码的类型。</span><span class="sxs-lookup"><span data-stu-id="d7a73-280">Type of work profile password that is required.</span></span> <span data-ttu-id="d7a73-281">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="d7a73-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="d7a73-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d7a73-282">workProfileRequirePassword</span></span>|<span data-ttu-id="d7a73-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-283">Boolean</span></span>|<span data-ttu-id="d7a73-284">密码，则需要或不工作配置文件</span><span class="sxs-lookup"><span data-stu-id="d7a73-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="d7a73-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="d7a73-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="d7a73-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-286">Boolean</span></span>|<span data-ttu-id="d7a73-287">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="d7a73-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="d7a73-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7a73-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="d7a73-289">字符串</span><span class="sxs-lookup"><span data-stu-id="d7a73-289">String</span></span>|<span data-ttu-id="d7a73-290">始终在 VPN 中启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="d7a73-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="d7a73-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="d7a73-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="d7a73-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a73-292">Boolean</span></span>|<span data-ttu-id="d7a73-293">始终在 VPN 中启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="d7a73-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="d7a73-294">响应</span><span class="sxs-lookup"><span data-stu-id="d7a73-294">Response</span></span>
<span data-ttu-id="d7a73-295">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7a73-295">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7a73-296">示例</span><span class="sxs-lookup"><span data-stu-id="d7a73-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7a73-297">请求</span><span class="sxs-lookup"><span data-stu-id="d7a73-297">Request</span></span>
<span data-ttu-id="d7a73-298">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7a73-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2023

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d7a73-299">响应</span><span class="sxs-lookup"><span data-stu-id="d7a73-299">Response</span></span>
<span data-ttu-id="d7a73-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7a73-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





