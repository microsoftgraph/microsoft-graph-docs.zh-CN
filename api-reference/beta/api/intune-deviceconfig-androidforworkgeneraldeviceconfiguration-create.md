---
title: 创建 androidForWorkGeneralDeviceConfiguration
description: 创建新的 androidForWorkGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bbbcb446cd21e03dbfe2e61df480d67c2abbc28c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963518"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="42ce4-103">创建 androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="42ce4-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="42ce4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42ce4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42ce4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42ce4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42ce4-106">创建新的[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="42ce4-106">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42ce4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="42ce4-107">Prerequisites</span></span>
<span data-ttu-id="42ce4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42ce4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42ce4-110">Permission type</span></span>|<span data-ttu-id="42ce4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42ce4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42ce4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42ce4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42ce4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42ce4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42ce4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42ce4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42ce4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42ce4-115">Not supported.</span></span>|
|<span data-ttu-id="42ce4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="42ce4-116">Application</span></span>|<span data-ttu-id="42ce4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="42ce4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42ce4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42ce4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="42ce4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="42ce4-119">Request headers</span></span>
|<span data-ttu-id="42ce4-120">标头</span><span class="sxs-lookup"><span data-stu-id="42ce4-120">Header</span></span>|<span data-ttu-id="42ce4-121">值</span><span class="sxs-lookup"><span data-stu-id="42ce4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42ce4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42ce4-122">Authorization</span></span>|<span data-ttu-id="42ce4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42ce4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42ce4-124">接受</span><span class="sxs-lookup"><span data-stu-id="42ce4-124">Accept</span></span>|<span data-ttu-id="42ce4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42ce4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42ce4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42ce4-126">Request body</span></span>
<span data-ttu-id="42ce4-127">在请求正文中, 提供 androidForWorkGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42ce4-127">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="42ce4-128">下表显示创建 androidForWorkGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="42ce4-128">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="42ce4-129">属性</span><span class="sxs-lookup"><span data-stu-id="42ce4-129">Property</span></span>|<span data-ttu-id="42ce4-130">类型</span><span class="sxs-lookup"><span data-stu-id="42ce4-130">Type</span></span>|<span data-ttu-id="42ce4-131">说明</span><span class="sxs-lookup"><span data-stu-id="42ce4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ce4-132">id</span><span class="sxs-lookup"><span data-stu-id="42ce4-132">id</span></span>|<span data-ttu-id="42ce4-133">String</span><span class="sxs-lookup"><span data-stu-id="42ce4-133">String</span></span>|<span data-ttu-id="42ce4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="42ce4-134">Key of the entity.</span></span> <span data-ttu-id="42ce4-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42ce4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="42ce4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ce4-137">DateTimeOffset</span></span>|<span data-ttu-id="42ce4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="42ce4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="42ce4-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42ce4-140">roleScopeTagIds</span></span>|<span data-ttu-id="42ce4-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="42ce4-141">String collection</span></span>|<span data-ttu-id="42ce4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="42ce4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42ce4-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="42ce4-144">supportsScopeTags</span></span>|<span data-ttu-id="42ce4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-145">Boolean</span></span>|<span data-ttu-id="42ce4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="42ce4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42ce4-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="42ce4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42ce4-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="42ce4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42ce4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="42ce4-149">This property is read-only.</span></span> <span data-ttu-id="42ce4-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42ce4-151">createdDateTime</span></span>|<span data-ttu-id="42ce4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ce4-152">DateTimeOffset</span></span>|<span data-ttu-id="42ce4-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="42ce4-153">DateTime the object was created.</span></span> <span data-ttu-id="42ce4-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-155">description</span><span class="sxs-lookup"><span data-stu-id="42ce4-155">description</span></span>|<span data-ttu-id="42ce4-156">String</span><span class="sxs-lookup"><span data-stu-id="42ce4-156">String</span></span>|<span data-ttu-id="42ce4-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="42ce4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42ce4-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="42ce4-159">displayName</span></span>|<span data-ttu-id="42ce4-160">String</span><span class="sxs-lookup"><span data-stu-id="42ce4-160">String</span></span>|<span data-ttu-id="42ce4-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="42ce4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42ce4-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-163">version</span><span class="sxs-lookup"><span data-stu-id="42ce4-163">version</span></span>|<span data-ttu-id="42ce4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-164">Int32</span></span>|<span data-ttu-id="42ce4-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="42ce4-165">Version of the device configuration.</span></span> <span data-ttu-id="42ce4-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42ce4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42ce4-167">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="42ce4-167">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="42ce4-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-168">Boolean</span></span>|<span data-ttu-id="42ce4-169">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="42ce4-169">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="42ce4-170">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="42ce4-170">passwordBlockTrustAgents</span></span>|<span data-ttu-id="42ce4-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-171">Boolean</span></span>|<span data-ttu-id="42ce4-172">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="42ce4-172">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="42ce4-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="42ce4-173">passwordExpirationDays</span></span>|<span data-ttu-id="42ce4-174">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-174">Int32</span></span>|<span data-ttu-id="42ce4-175">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-175">Number of days before the password expires.</span></span> <span data-ttu-id="42ce4-176">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="42ce4-176">Valid values 1 to 365</span></span>|
|<span data-ttu-id="42ce4-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42ce4-177">passwordMinimumLength</span></span>|<span data-ttu-id="42ce4-178">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-178">Int32</span></span>|<span data-ttu-id="42ce4-179">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="42ce4-179">Minimum length of passwords.</span></span> <span data-ttu-id="42ce4-180">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="42ce4-180">Valid values 4 to 16</span></span>|
|<span data-ttu-id="42ce4-181">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="42ce4-181">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="42ce4-182">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-182">Int32</span></span>|<span data-ttu-id="42ce4-183">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-183">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="42ce4-184">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="42ce4-184">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="42ce4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-185">Int32</span></span>|<span data-ttu-id="42ce4-186">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="42ce4-186">Number of previous passwords to block.</span></span> <span data-ttu-id="42ce4-187">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="42ce4-187">Valid values 0 to 24</span></span>|
|<span data-ttu-id="42ce4-188">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="42ce4-188">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="42ce4-189">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-189">Int32</span></span>|<span data-ttu-id="42ce4-190">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-190">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="42ce4-191">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="42ce4-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="42ce4-192">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="42ce4-192">passwordRequiredType</span></span>|[<span data-ttu-id="42ce4-193">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="42ce4-193">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="42ce4-194">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="42ce4-194">Type of password that is required.</span></span> <span data-ttu-id="42ce4-195">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="42ce4-195">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="42ce4-196">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="42ce4-196">workProfileDataSharingType</span></span>|[<span data-ttu-id="42ce4-197">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="42ce4-197">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="42ce4-198">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="42ce4-198">Type of data sharing that is allowed.</span></span> <span data-ttu-id="42ce4-199">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="42ce4-199">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="42ce4-200">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="42ce4-200">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="42ce4-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-201">Boolean</span></span>|<span data-ttu-id="42ce4-202">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="42ce4-202">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="42ce4-203">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="42ce4-203">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="42ce4-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-204">Boolean</span></span>|<span data-ttu-id="42ce4-205">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="42ce4-205">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="42ce4-206">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="42ce4-206">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="42ce4-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-207">Boolean</span></span>|<span data-ttu-id="42ce4-208">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="42ce4-208">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="42ce4-209">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="42ce4-209">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="42ce4-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-210">Boolean</span></span>|<span data-ttu-id="42ce4-211">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="42ce4-211">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="42ce4-212">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="42ce4-212">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="42ce4-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-213">Boolean</span></span>|<span data-ttu-id="42ce4-214">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="42ce4-214">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="42ce4-215">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="42ce4-215">workProfileBlockCamera</span></span>|<span data-ttu-id="42ce4-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-216">Boolean</span></span>|<span data-ttu-id="42ce4-217">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="42ce4-217">Block work profile camera.</span></span>|
|<span data-ttu-id="42ce4-218">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="42ce4-218">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="42ce4-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-219">Boolean</span></span>|<span data-ttu-id="42ce4-220">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="42ce4-220">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="42ce4-221">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="42ce4-221">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="42ce4-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-222">Boolean</span></span>|<span data-ttu-id="42ce4-223">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="42ce4-223">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="42ce4-224">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="42ce4-224">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="42ce4-225">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="42ce4-225">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="42ce4-226">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="42ce4-226">Type of password that is required.</span></span> <span data-ttu-id="42ce4-227">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="42ce4-227">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="42ce4-228">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="42ce4-228">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="42ce4-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-229">Boolean</span></span>|<span data-ttu-id="42ce4-230">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="42ce4-230">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="42ce4-231">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="42ce4-231">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="42ce4-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-232">Boolean</span></span>|<span data-ttu-id="42ce4-233">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="42ce4-233">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="42ce4-234">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="42ce4-234">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="42ce4-235">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-235">Int32</span></span>|<span data-ttu-id="42ce4-236">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-236">Number of days before the work profile password expires.</span></span> <span data-ttu-id="42ce4-237">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="42ce4-237">Valid values 1 to 365</span></span>|
|<span data-ttu-id="42ce4-238">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42ce4-238">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="42ce4-239">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-239">Int32</span></span>|<span data-ttu-id="42ce4-240">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="42ce4-240">Minimum length of work profile password.</span></span> <span data-ttu-id="42ce4-241">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="42ce4-241">Valid values 4 to 16</span></span>|
|<span data-ttu-id="42ce4-242">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="42ce4-242">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="42ce4-243">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-243">Int32</span></span>|<span data-ttu-id="42ce4-244">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-244">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="42ce4-245">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="42ce4-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="42ce4-246">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="42ce4-246">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="42ce4-247">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-247">Int32</span></span>|<span data-ttu-id="42ce4-248">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-248">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="42ce4-249">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="42ce4-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="42ce4-250">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="42ce4-250">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="42ce4-251">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-251">Int32</span></span>|<span data-ttu-id="42ce4-252">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="42ce4-252">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="42ce4-253">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="42ce4-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="42ce4-254">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="42ce4-254">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="42ce4-255">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-255">Int32</span></span>|<span data-ttu-id="42ce4-256">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="42ce4-256">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="42ce4-257">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="42ce4-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="42ce4-258">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="42ce4-258">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="42ce4-259">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-259">Int32</span></span>|<span data-ttu-id="42ce4-260">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="42ce4-260">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="42ce4-261">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="42ce4-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="42ce4-262">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="42ce4-262">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="42ce4-263">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-263">Int32</span></span>|<span data-ttu-id="42ce4-264">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-264">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="42ce4-265">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="42ce4-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="42ce4-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="42ce4-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="42ce4-267">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-267">Int32</span></span>|<span data-ttu-id="42ce4-268">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-268">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="42ce4-269">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="42ce4-269">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="42ce4-270">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-270">Int32</span></span>|<span data-ttu-id="42ce4-271">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="42ce4-271">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="42ce4-272">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="42ce4-272">Valid values 0 to 24</span></span>|
|<span data-ttu-id="42ce4-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="42ce4-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="42ce4-274">Int32</span><span class="sxs-lookup"><span data-stu-id="42ce4-274">Int32</span></span>|<span data-ttu-id="42ce4-275">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="42ce4-275">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="42ce4-276">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="42ce4-276">Valid values 1 to 16</span></span>|
|<span data-ttu-id="42ce4-277">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="42ce4-277">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="42ce4-278">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="42ce4-278">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="42ce4-279">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="42ce4-279">Type of work profile password that is required.</span></span> <span data-ttu-id="42ce4-280">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="42ce4-280">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="42ce4-281">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="42ce4-281">workProfileRequirePassword</span></span>|<span data-ttu-id="42ce4-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-282">Boolean</span></span>|<span data-ttu-id="42ce4-283">对于工作配置文件, 密码是必需的</span><span class="sxs-lookup"><span data-stu-id="42ce4-283">Password is required or not for work profile</span></span>|
|<span data-ttu-id="42ce4-284">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="42ce4-284">securityRequireVerifyApps</span></span>|<span data-ttu-id="42ce4-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-285">Boolean</span></span>|<span data-ttu-id="42ce4-286">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="42ce4-286">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="42ce4-287">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="42ce4-287">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="42ce4-288">String</span><span class="sxs-lookup"><span data-stu-id="42ce4-288">String</span></span>|<span data-ttu-id="42ce4-289">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="42ce4-289">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="42ce4-290">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="42ce4-290">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="42ce4-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ce4-291">Boolean</span></span>|<span data-ttu-id="42ce4-292">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="42ce4-292">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="42ce4-293">响应</span><span class="sxs-lookup"><span data-stu-id="42ce4-293">Response</span></span>
<span data-ttu-id="42ce4-294">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="42ce4-294">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42ce4-295">示例</span><span class="sxs-lookup"><span data-stu-id="42ce4-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="42ce4-296">请求</span><span class="sxs-lookup"><span data-stu-id="42ce4-296">Request</span></span>
<span data-ttu-id="42ce4-297">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42ce4-297">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="42ce4-298">响应</span><span class="sxs-lookup"><span data-stu-id="42ce4-298">Response</span></span>
<span data-ttu-id="42ce4-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42ce4-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




