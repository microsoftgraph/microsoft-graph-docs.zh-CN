---
title: 创建 androidCompliancePolicy
description: 创建新的 androidCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8affcd773474c025acf0371f96bb401b1dcad17f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126792"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="ddd7e-103">创建 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ddd7e-103">Create androidCompliancePolicy</span></span>

<span data-ttu-id="ddd7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddd7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddd7e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddd7e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddd7e-107">创建新的 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddd7e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddd7e-108">Prerequisites</span></span>
<span data-ttu-id="ddd7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd7e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddd7e-111">Permission type</span></span>|<span data-ttu-id="ddd7e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddd7e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddd7e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddd7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddd7e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd7e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddd7e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddd7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddd7e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-116">Not supported.</span></span>|
|<span data-ttu-id="ddd7e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddd7e-117">Application</span></span>|<span data-ttu-id="ddd7e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd7e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddd7e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddd7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ddd7e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddd7e-120">Request headers</span></span>
|<span data-ttu-id="ddd7e-121">标头</span><span class="sxs-lookup"><span data-stu-id="ddd7e-121">Header</span></span>|<span data-ttu-id="ddd7e-122">值</span><span class="sxs-lookup"><span data-stu-id="ddd7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddd7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd7e-123">Authorization</span></span>|<span data-ttu-id="ddd7e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddd7e-125">接受</span><span class="sxs-lookup"><span data-stu-id="ddd7e-125">Accept</span></span>|<span data-ttu-id="ddd7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddd7e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddd7e-127">Request body</span></span>
<span data-ttu-id="ddd7e-128">在请求正文中，提供 androidCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="ddd7e-129">下表显示了创建 androidCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="ddd7e-130">属性</span><span class="sxs-lookup"><span data-stu-id="ddd7e-130">Property</span></span>|<span data-ttu-id="ddd7e-131">类型</span><span class="sxs-lookup"><span data-stu-id="ddd7e-131">Type</span></span>|<span data-ttu-id="ddd7e-132">说明</span><span class="sxs-lookup"><span data-stu-id="ddd7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd7e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddd7e-133">roleScopeTagIds</span></span>|<span data-ttu-id="ddd7e-134">String collection</span><span class="sxs-lookup"><span data-stu-id="ddd7e-134">String collection</span></span>|<span data-ttu-id="ddd7e-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ddd7e-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-137">id</span><span class="sxs-lookup"><span data-stu-id="ddd7e-137">id</span></span>|<span data-ttu-id="ddd7e-138">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-138">String</span></span>|<span data-ttu-id="ddd7e-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-139">Key of the entity.</span></span> <span data-ttu-id="ddd7e-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddd7e-141">createdDateTime</span></span>|<span data-ttu-id="ddd7e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddd7e-142">DateTimeOffset</span></span>|<span data-ttu-id="ddd7e-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-143">DateTime the object was created.</span></span> <span data-ttu-id="ddd7e-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-145">说明</span><span class="sxs-lookup"><span data-stu-id="ddd7e-145">description</span></span>|<span data-ttu-id="ddd7e-146">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-146">String</span></span>|<span data-ttu-id="ddd7e-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddd7e-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddd7e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ddd7e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddd7e-150">DateTimeOffset</span></span>|<span data-ttu-id="ddd7e-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="ddd7e-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ddd7e-153">displayName</span></span>|<span data-ttu-id="ddd7e-154">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-154">String</span></span>|<span data-ttu-id="ddd7e-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddd7e-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-157">version</span><span class="sxs-lookup"><span data-stu-id="ddd7e-157">version</span></span>|<span data-ttu-id="ddd7e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd7e-158">Int32</span></span>|<span data-ttu-id="ddd7e-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-159">Version of the device configuration.</span></span> <span data-ttu-id="ddd7e-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ddd7e-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ddd7e-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ddd7e-161">passwordRequired</span></span>|<span data-ttu-id="ddd7e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-162">Boolean</span></span>|<span data-ttu-id="ddd7e-163">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="ddd7e-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ddd7e-164">passwordMinimumLength</span></span>|<span data-ttu-id="ddd7e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd7e-165">Int32</span></span>|<span data-ttu-id="ddd7e-166">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-166">Minimum password length.</span></span> <span data-ttu-id="ddd7e-167">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="ddd7e-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ddd7e-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ddd7e-168">passwordRequiredType</span></span>|[<span data-ttu-id="ddd7e-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ddd7e-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="ddd7e-170">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-170">Type of characters in password.</span></span> <span data-ttu-id="ddd7e-171">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="ddd7e-172">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="ddd7e-172">requiredPasswordComplexity</span></span>|[<span data-ttu-id="ddd7e-173">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="ddd7e-173">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="ddd7e-174">指示 Android 上所需的密码复杂性。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-174">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="ddd7e-175">其中一个：NONE、LOW、MEDIUM、HIGH。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-175">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="ddd7e-176">这是面向 Android 11+的新 API。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-176">This is a new API targeted to Android 11+.</span></span> <span data-ttu-id="ddd7e-177">可取值为：`none`、`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-177">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ddd7e-178">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ddd7e-178">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ddd7e-179">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd7e-179">Int32</span></span>|<span data-ttu-id="ddd7e-180">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-180">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ddd7e-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ddd7e-181">passwordExpirationDays</span></span>|<span data-ttu-id="ddd7e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd7e-182">Int32</span></span>|<span data-ttu-id="ddd7e-183">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-183">Number of days before the password expires.</span></span> <span data-ttu-id="ddd7e-184">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="ddd7e-184">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ddd7e-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ddd7e-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ddd7e-186">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd7e-186">Int32</span></span>|<span data-ttu-id="ddd7e-187">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-187">Number of previous passwords to block.</span></span> <span data-ttu-id="ddd7e-188">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="ddd7e-188">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ddd7e-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ddd7e-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ddd7e-190">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd7e-190">Int32</span></span>|<span data-ttu-id="ddd7e-191">恢复出厂设置之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-191">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="ddd7e-192">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="ddd7e-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ddd7e-193">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="ddd7e-193">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="ddd7e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-194">Boolean</span></span>|<span data-ttu-id="ddd7e-195">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-195">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="ddd7e-196">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="ddd7e-196">securityDisableUsbDebugging</span></span>|<span data-ttu-id="ddd7e-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-197">Boolean</span></span>|<span data-ttu-id="ddd7e-198">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-198">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="ddd7e-199">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="ddd7e-199">securityRequireVerifyApps</span></span>|<span data-ttu-id="ddd7e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-200">Boolean</span></span>|<span data-ttu-id="ddd7e-201">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-201">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="ddd7e-202">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ddd7e-202">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ddd7e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-203">Boolean</span></span>|<span data-ttu-id="ddd7e-204">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-204">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ddd7e-205">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddd7e-205">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ddd7e-206">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ddd7e-206">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ddd7e-207">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-207">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ddd7e-208">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-208">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ddd7e-209">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddd7e-209">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ddd7e-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ddd7e-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ddd7e-211">MDATP 要求移动威胁防护最低风险级别来报告不相容情况。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-211">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ddd7e-212">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ddd7e-213">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="ddd7e-213">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="ddd7e-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-214">Boolean</span></span>|<span data-ttu-id="ddd7e-215">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-215">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="ddd7e-216">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="ddd7e-216">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="ddd7e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-217">Boolean</span></span>|<span data-ttu-id="ddd7e-218">阻止设备管理员管理的设备。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-218">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="ddd7e-219">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ddd7e-219">osMinimumVersion</span></span>|<span data-ttu-id="ddd7e-220">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-220">String</span></span>|<span data-ttu-id="ddd7e-221">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-221">Minimum Android version.</span></span>|
|<span data-ttu-id="ddd7e-222">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ddd7e-222">osMaximumVersion</span></span>|<span data-ttu-id="ddd7e-223">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-223">String</span></span>|<span data-ttu-id="ddd7e-224">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-224">Maximum Android version.</span></span>|
|<span data-ttu-id="ddd7e-225">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ddd7e-225">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="ddd7e-226">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-226">String</span></span>|<span data-ttu-id="ddd7e-227">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-227">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="ddd7e-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ddd7e-228">storageRequireEncryption</span></span>|<span data-ttu-id="ddd7e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-229">Boolean</span></span>|<span data-ttu-id="ddd7e-230">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-230">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="ddd7e-231">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="ddd7e-231">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="ddd7e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-232">Boolean</span></span>|<span data-ttu-id="ddd7e-233">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-233">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="ddd7e-234">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="ddd7e-234">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="ddd7e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-235">Boolean</span></span>|<span data-ttu-id="ddd7e-236">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-236">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="ddd7e-237">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="ddd7e-237">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="ddd7e-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-238">Boolean</span></span>|<span data-ttu-id="ddd7e-239">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-239">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="ddd7e-240">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="ddd7e-240">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="ddd7e-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-241">Boolean</span></span>|<span data-ttu-id="ddd7e-242">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-242">Require the device to have up to date security providers.</span></span> <span data-ttu-id="ddd7e-243">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-243">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="ddd7e-244">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="ddd7e-244">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="ddd7e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd7e-245">Boolean</span></span>|<span data-ttu-id="ddd7e-246">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-246">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="ddd7e-247">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="ddd7e-247">conditionStatementId</span></span>|<span data-ttu-id="ddd7e-248">String</span><span class="sxs-lookup"><span data-stu-id="ddd7e-248">String</span></span>|<span data-ttu-id="ddd7e-249">条件语句 id。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-249">Condition statement id.</span></span>|
|<span data-ttu-id="ddd7e-250">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="ddd7e-250">restrictedApps</span></span>|<span data-ttu-id="ddd7e-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddd7e-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ddd7e-252">要求设备未安装指定的应用。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-252">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="ddd7e-253">此集合最多可包含 100 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-253">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ddd7e-254">响应</span><span class="sxs-lookup"><span data-stu-id="ddd7e-254">Response</span></span>
<span data-ttu-id="ddd7e-255">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-255">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd7e-256">示例</span><span class="sxs-lookup"><span data-stu-id="ddd7e-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddd7e-257">请求</span><span class="sxs-lookup"><span data-stu-id="ddd7e-257">Request</span></span>
<span data-ttu-id="ddd7e-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="ddd7e-259">响应</span><span class="sxs-lookup"><span data-stu-id="ddd7e-259">Response</span></span>
<span data-ttu-id="ddd7e-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddd7e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




