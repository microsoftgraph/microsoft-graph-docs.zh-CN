---
title: 更新 androidDeviceOwnerCompliancePolicy
description: 更新 androidDeviceOwnerCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f75c206698bbc5f47e3e43abf722ed8f648645e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809195"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="b6fac-103">更新 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b6fac-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="b6fac-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6fac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6fac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6fac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6fac-106">更新[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6fac-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6fac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6fac-107">Prerequisites</span></span>
<span data-ttu-id="b6fac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6fac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6fac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6fac-110">Permission type</span></span>|<span data-ttu-id="b6fac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6fac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6fac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6fac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6fac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6fac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6fac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6fac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6fac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6fac-115">Not supported.</span></span>|
|<span data-ttu-id="b6fac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6fac-116">Application</span></span>|<span data-ttu-id="b6fac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6fac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6fac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6fac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b6fac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6fac-119">Request headers</span></span>
|<span data-ttu-id="b6fac-120">标头</span><span class="sxs-lookup"><span data-stu-id="b6fac-120">Header</span></span>|<span data-ttu-id="b6fac-121">值</span><span class="sxs-lookup"><span data-stu-id="b6fac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6fac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6fac-122">Authorization</span></span>|<span data-ttu-id="b6fac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6fac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6fac-124">接受</span><span class="sxs-lookup"><span data-stu-id="b6fac-124">Accept</span></span>|<span data-ttu-id="b6fac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6fac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6fac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6fac-126">Request body</span></span>
<span data-ttu-id="b6fac-127">在请求正文中, 提供[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6fac-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="b6fac-128">下表显示创建[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6fac-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="b6fac-129">属性</span><span class="sxs-lookup"><span data-stu-id="b6fac-129">Property</span></span>|<span data-ttu-id="b6fac-130">类型</span><span class="sxs-lookup"><span data-stu-id="b6fac-130">Type</span></span>|<span data-ttu-id="b6fac-131">说明</span><span class="sxs-lookup"><span data-stu-id="b6fac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6fac-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6fac-132">roleScopeTagIds</span></span>|<span data-ttu-id="b6fac-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="b6fac-133">String collection</span></span>|<span data-ttu-id="b6fac-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b6fac-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6fac-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-136">id</span><span class="sxs-lookup"><span data-stu-id="b6fac-136">id</span></span>|<span data-ttu-id="b6fac-137">String</span><span class="sxs-lookup"><span data-stu-id="b6fac-137">String</span></span>|<span data-ttu-id="b6fac-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6fac-138">Key of the entity.</span></span> <span data-ttu-id="b6fac-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6fac-140">createdDateTime</span></span>|<span data-ttu-id="b6fac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6fac-141">DateTimeOffset</span></span>|<span data-ttu-id="b6fac-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6fac-142">DateTime the object was created.</span></span> <span data-ttu-id="b6fac-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-144">description</span><span class="sxs-lookup"><span data-stu-id="b6fac-144">description</span></span>|<span data-ttu-id="b6fac-145">String</span><span class="sxs-lookup"><span data-stu-id="b6fac-145">String</span></span>|<span data-ttu-id="b6fac-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b6fac-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6fac-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6fac-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b6fac-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6fac-149">DateTimeOffset</span></span>|<span data-ttu-id="b6fac-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6fac-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b6fac-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b6fac-152">displayName</span></span>|<span data-ttu-id="b6fac-153">String</span><span class="sxs-lookup"><span data-stu-id="b6fac-153">String</span></span>|<span data-ttu-id="b6fac-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b6fac-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6fac-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-156">version</span><span class="sxs-lookup"><span data-stu-id="b6fac-156">version</span></span>|<span data-ttu-id="b6fac-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-157">Int32</span></span>|<span data-ttu-id="b6fac-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b6fac-158">Version of the device configuration.</span></span> <span data-ttu-id="b6fac-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6fac-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6fac-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b6fac-160">osMinimumVersion</span></span>|<span data-ttu-id="b6fac-161">String</span><span class="sxs-lookup"><span data-stu-id="b6fac-161">String</span></span>|<span data-ttu-id="b6fac-162">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b6fac-162">Minimum Android version.</span></span>|
|<span data-ttu-id="b6fac-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b6fac-163">osMaximumVersion</span></span>|<span data-ttu-id="b6fac-164">String</span><span class="sxs-lookup"><span data-stu-id="b6fac-164">String</span></span>|<span data-ttu-id="b6fac-165">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b6fac-165">Maximum Android version.</span></span>|
|<span data-ttu-id="b6fac-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b6fac-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b6fac-167">String</span><span class="sxs-lookup"><span data-stu-id="b6fac-167">String</span></span>|<span data-ttu-id="b6fac-168">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="b6fac-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b6fac-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b6fac-169">passwordRequired</span></span>|<span data-ttu-id="b6fac-170">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6fac-170">Boolean</span></span>|<span data-ttu-id="b6fac-171">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="b6fac-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b6fac-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6fac-172">passwordMinimumLength</span></span>|<span data-ttu-id="b6fac-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-173">Int32</span></span>|<span data-ttu-id="b6fac-174">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="b6fac-174">Minimum password length.</span></span> <span data-ttu-id="b6fac-175">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b6fac-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b6fac-176">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b6fac-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="b6fac-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-177">Int32</span></span>|<span data-ttu-id="b6fac-178">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="b6fac-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="b6fac-179">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b6fac-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6fac-180">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b6fac-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="b6fac-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-181">Int32</span></span>|<span data-ttu-id="b6fac-182">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="b6fac-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="b6fac-183">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b6fac-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6fac-184">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="b6fac-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="b6fac-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-185">Int32</span></span>|<span data-ttu-id="b6fac-186">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="b6fac-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="b6fac-187">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b6fac-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6fac-188">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="b6fac-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="b6fac-189">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-189">Int32</span></span>|<span data-ttu-id="b6fac-190">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="b6fac-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="b6fac-191">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b6fac-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6fac-192">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="b6fac-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="b6fac-193">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-193">Int32</span></span>|<span data-ttu-id="b6fac-194">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="b6fac-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="b6fac-195">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b6fac-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6fac-196">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="b6fac-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="b6fac-197">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-197">Int32</span></span>|<span data-ttu-id="b6fac-198">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="b6fac-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="b6fac-199">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b6fac-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6fac-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6fac-200">passwordRequiredType</span></span>|[<span data-ttu-id="b6fac-201">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b6fac-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="b6fac-202">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="b6fac-202">Type of characters in password.</span></span> <span data-ttu-id="b6fac-203">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。</span><span class="sxs-lookup"><span data-stu-id="b6fac-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="b6fac-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b6fac-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b6fac-205">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-205">Int32</span></span>|<span data-ttu-id="b6fac-206">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b6fac-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b6fac-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6fac-207">passwordExpirationDays</span></span>|<span data-ttu-id="b6fac-208">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-208">Int32</span></span>|<span data-ttu-id="b6fac-209">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="b6fac-209">Number of days before the password expires.</span></span> <span data-ttu-id="b6fac-210">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="b6fac-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b6fac-211">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="b6fac-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="b6fac-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b6fac-212">Int32</span></span>|<span data-ttu-id="b6fac-213">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b6fac-213">Number of previous passwords to block.</span></span> <span data-ttu-id="b6fac-214">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="b6fac-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b6fac-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b6fac-215">storageRequireEncryption</span></span>|<span data-ttu-id="b6fac-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6fac-216">Boolean</span></span>|<span data-ttu-id="b6fac-217">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="b6fac-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b6fac-218">响应</span><span class="sxs-lookup"><span data-stu-id="b6fac-218">Response</span></span>
<span data-ttu-id="b6fac-219">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6fac-219">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6fac-220">示例</span><span class="sxs-lookup"><span data-stu-id="b6fac-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6fac-221">请求</span><span class="sxs-lookup"><span data-stu-id="b6fac-221">Request</span></span>
<span data-ttu-id="b6fac-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6fac-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 932

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="b6fac-223">响应</span><span class="sxs-lookup"><span data-stu-id="b6fac-223">Response</span></span>
<span data-ttu-id="b6fac-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6fac-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1104

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```





