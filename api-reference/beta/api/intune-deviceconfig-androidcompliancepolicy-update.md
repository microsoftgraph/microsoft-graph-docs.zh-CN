---
title: 更新 androidCompliancePolicy
description: 更新 androidCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 710be96249654d405132a06c4f2ba0b86055fd1f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126757"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="e5b19-103">更新 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e5b19-103">Update androidCompliancePolicy</span></span>

<span data-ttu-id="e5b19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5b19-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5b19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5b19-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5b19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b19-107">更新 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5b19-107">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5b19-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5b19-108">Prerequisites</span></span>
<span data-ttu-id="e5b19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5b19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b19-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5b19-111">Permission type</span></span>|<span data-ttu-id="e5b19-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5b19-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5b19-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5b19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5b19-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5b19-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5b19-116">Not supported.</span></span>|
|<span data-ttu-id="e5b19-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5b19-117">Application</span></span>|<span data-ttu-id="e5b19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5b19-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5b19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e5b19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5b19-120">Request headers</span></span>
|<span data-ttu-id="e5b19-121">标头</span><span class="sxs-lookup"><span data-stu-id="e5b19-121">Header</span></span>|<span data-ttu-id="e5b19-122">值</span><span class="sxs-lookup"><span data-stu-id="e5b19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5b19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b19-123">Authorization</span></span>|<span data-ttu-id="e5b19-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5b19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5b19-125">接受</span><span class="sxs-lookup"><span data-stu-id="e5b19-125">Accept</span></span>|<span data-ttu-id="e5b19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5b19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b19-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5b19-127">Request body</span></span>
<span data-ttu-id="e5b19-128">在请求正文中，提供 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5b19-128">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="e5b19-129">下表显示了创建 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5b19-129">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="e5b19-130">属性</span><span class="sxs-lookup"><span data-stu-id="e5b19-130">Property</span></span>|<span data-ttu-id="e5b19-131">类型</span><span class="sxs-lookup"><span data-stu-id="e5b19-131">Type</span></span>|<span data-ttu-id="e5b19-132">说明</span><span class="sxs-lookup"><span data-stu-id="e5b19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b19-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5b19-133">roleScopeTagIds</span></span>|<span data-ttu-id="e5b19-134">String collection</span><span class="sxs-lookup"><span data-stu-id="e5b19-134">String collection</span></span>|<span data-ttu-id="e5b19-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e5b19-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5b19-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-137">id</span><span class="sxs-lookup"><span data-stu-id="e5b19-137">id</span></span>|<span data-ttu-id="e5b19-138">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-138">String</span></span>|<span data-ttu-id="e5b19-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e5b19-139">Key of the entity.</span></span> <span data-ttu-id="e5b19-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b19-141">createdDateTime</span></span>|<span data-ttu-id="e5b19-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b19-142">DateTimeOffset</span></span>|<span data-ttu-id="e5b19-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e5b19-143">DateTime the object was created.</span></span> <span data-ttu-id="e5b19-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-145">说明</span><span class="sxs-lookup"><span data-stu-id="e5b19-145">description</span></span>|<span data-ttu-id="e5b19-146">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-146">String</span></span>|<span data-ttu-id="e5b19-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e5b19-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5b19-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b19-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e5b19-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b19-150">DateTimeOffset</span></span>|<span data-ttu-id="e5b19-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e5b19-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e5b19-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e5b19-153">displayName</span></span>|<span data-ttu-id="e5b19-154">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-154">String</span></span>|<span data-ttu-id="e5b19-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e5b19-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5b19-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-157">version</span><span class="sxs-lookup"><span data-stu-id="e5b19-157">version</span></span>|<span data-ttu-id="e5b19-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b19-158">Int32</span></span>|<span data-ttu-id="e5b19-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e5b19-159">Version of the device configuration.</span></span> <span data-ttu-id="e5b19-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e5b19-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5b19-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e5b19-161">passwordRequired</span></span>|<span data-ttu-id="e5b19-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-162">Boolean</span></span>|<span data-ttu-id="e5b19-163">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="e5b19-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="e5b19-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e5b19-164">passwordMinimumLength</span></span>|<span data-ttu-id="e5b19-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b19-165">Int32</span></span>|<span data-ttu-id="e5b19-166">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="e5b19-166">Minimum password length.</span></span> <span data-ttu-id="e5b19-167">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="e5b19-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e5b19-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e5b19-168">passwordRequiredType</span></span>|[<span data-ttu-id="e5b19-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e5b19-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="e5b19-170">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="e5b19-170">Type of characters in password.</span></span> <span data-ttu-id="e5b19-171">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="e5b19-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="e5b19-172">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="e5b19-172">requiredPasswordComplexity</span></span>|[<span data-ttu-id="e5b19-173">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="e5b19-173">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="e5b19-174">指示 Android 上所需的密码复杂性。</span><span class="sxs-lookup"><span data-stu-id="e5b19-174">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="e5b19-175">其中一个：NONE、LOW、MEDIUM、HIGH。</span><span class="sxs-lookup"><span data-stu-id="e5b19-175">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="e5b19-176">这是面向 Android 11+的新 API。</span><span class="sxs-lookup"><span data-stu-id="e5b19-176">This is a new API targeted to Android 11+.</span></span> <span data-ttu-id="e5b19-177">可取值为：`none`、`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e5b19-177">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e5b19-178">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e5b19-178">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e5b19-179">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b19-179">Int32</span></span>|<span data-ttu-id="e5b19-180">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e5b19-180">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e5b19-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e5b19-181">passwordExpirationDays</span></span>|<span data-ttu-id="e5b19-182">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b19-182">Int32</span></span>|<span data-ttu-id="e5b19-183">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e5b19-183">Number of days before the password expires.</span></span> <span data-ttu-id="e5b19-184">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="e5b19-184">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e5b19-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e5b19-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e5b19-186">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b19-186">Int32</span></span>|<span data-ttu-id="e5b19-187">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e5b19-187">Number of previous passwords to block.</span></span> <span data-ttu-id="e5b19-188">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="e5b19-188">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e5b19-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e5b19-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e5b19-190">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b19-190">Int32</span></span>|<span data-ttu-id="e5b19-191">恢复出厂设置之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="e5b19-191">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="e5b19-192">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="e5b19-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e5b19-193">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="e5b19-193">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="e5b19-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-194">Boolean</span></span>|<span data-ttu-id="e5b19-195">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="e5b19-195">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="e5b19-196">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="e5b19-196">securityDisableUsbDebugging</span></span>|<span data-ttu-id="e5b19-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-197">Boolean</span></span>|<span data-ttu-id="e5b19-198">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="e5b19-198">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="e5b19-199">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e5b19-199">securityRequireVerifyApps</span></span>|<span data-ttu-id="e5b19-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-200">Boolean</span></span>|<span data-ttu-id="e5b19-201">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="e5b19-201">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="e5b19-202">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e5b19-202">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e5b19-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-203">Boolean</span></span>|<span data-ttu-id="e5b19-204">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="e5b19-204">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="e5b19-205">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e5b19-205">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e5b19-206">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e5b19-206">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e5b19-207">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="e5b19-207">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e5b19-208">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="e5b19-208">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e5b19-209">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e5b19-209">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e5b19-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e5b19-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e5b19-211">MDATP 要求移动威胁防护最低风险级别来报告不相容情况。</span><span class="sxs-lookup"><span data-stu-id="e5b19-211">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e5b19-212">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="e5b19-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e5b19-213">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="e5b19-213">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="e5b19-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-214">Boolean</span></span>|<span data-ttu-id="e5b19-215">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="e5b19-215">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="e5b19-216">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="e5b19-216">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="e5b19-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-217">Boolean</span></span>|<span data-ttu-id="e5b19-218">阻止设备管理员管理的设备。</span><span class="sxs-lookup"><span data-stu-id="e5b19-218">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="e5b19-219">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e5b19-219">osMinimumVersion</span></span>|<span data-ttu-id="e5b19-220">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-220">String</span></span>|<span data-ttu-id="e5b19-221">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="e5b19-221">Minimum Android version.</span></span>|
|<span data-ttu-id="e5b19-222">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e5b19-222">osMaximumVersion</span></span>|<span data-ttu-id="e5b19-223">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-223">String</span></span>|<span data-ttu-id="e5b19-224">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="e5b19-224">Maximum Android version.</span></span>|
|<span data-ttu-id="e5b19-225">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="e5b19-225">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="e5b19-226">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-226">String</span></span>|<span data-ttu-id="e5b19-227">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="e5b19-227">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="e5b19-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e5b19-228">storageRequireEncryption</span></span>|<span data-ttu-id="e5b19-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-229">Boolean</span></span>|<span data-ttu-id="e5b19-230">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="e5b19-230">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="e5b19-231">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="e5b19-231">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="e5b19-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-232">Boolean</span></span>|<span data-ttu-id="e5b19-233">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="e5b19-233">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="e5b19-234">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="e5b19-234">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="e5b19-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-235">Boolean</span></span>|<span data-ttu-id="e5b19-236">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="e5b19-236">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="e5b19-237">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="e5b19-237">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="e5b19-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-238">Boolean</span></span>|<span data-ttu-id="e5b19-239">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="e5b19-239">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="e5b19-240">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="e5b19-240">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="e5b19-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-241">Boolean</span></span>|<span data-ttu-id="e5b19-242">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="e5b19-242">Require the device to have up to date security providers.</span></span> <span data-ttu-id="e5b19-243">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="e5b19-243">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="e5b19-244">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="e5b19-244">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="e5b19-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b19-245">Boolean</span></span>|<span data-ttu-id="e5b19-246">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="e5b19-246">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="e5b19-247">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="e5b19-247">conditionStatementId</span></span>|<span data-ttu-id="e5b19-248">String</span><span class="sxs-lookup"><span data-stu-id="e5b19-248">String</span></span>|<span data-ttu-id="e5b19-249">条件语句 id。</span><span class="sxs-lookup"><span data-stu-id="e5b19-249">Condition statement id.</span></span>|
|<span data-ttu-id="e5b19-250">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e5b19-250">restrictedApps</span></span>|<span data-ttu-id="e5b19-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5b19-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e5b19-252">要求设备未安装指定的应用。</span><span class="sxs-lookup"><span data-stu-id="e5b19-252">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="e5b19-253">此集合最多可包含 100 个元素。</span><span class="sxs-lookup"><span data-stu-id="e5b19-253">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e5b19-254">响应</span><span class="sxs-lookup"><span data-stu-id="e5b19-254">Response</span></span>
<span data-ttu-id="e5b19-255">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5b19-255">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b19-256">示例</span><span class="sxs-lookup"><span data-stu-id="e5b19-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5b19-257">请求</span><span class="sxs-lookup"><span data-stu-id="e5b19-257">Request</span></span>
<span data-ttu-id="e5b19-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5b19-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1750

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "securityBlockDeviceAdministratorManagedDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e5b19-259">响应</span><span class="sxs-lookup"><span data-stu-id="e5b19-259">Response</span></span>
<span data-ttu-id="e5b19-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5b19-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1922

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "securityBlockDeviceAdministratorManagedDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




