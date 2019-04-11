---
title: 创建 androidDeviceOwnerCompliancePolicy
description: 创建新的 androidDeviceOwnerCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19ccb8cc7d778f62528b1558d762a7a938b12645
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808899"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="efcac-103">创建 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="efcac-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="efcac-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efcac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efcac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efcac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efcac-106">创建新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="efcac-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efcac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="efcac-107">Prerequisites</span></span>
<span data-ttu-id="efcac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efcac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efcac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="efcac-110">Permission type</span></span>|<span data-ttu-id="efcac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efcac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efcac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efcac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efcac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efcac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efcac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efcac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efcac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="efcac-115">Not supported.</span></span>|
|<span data-ttu-id="efcac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="efcac-116">Application</span></span>|<span data-ttu-id="efcac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="efcac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efcac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efcac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="efcac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="efcac-119">Request headers</span></span>
|<span data-ttu-id="efcac-120">标头</span><span class="sxs-lookup"><span data-stu-id="efcac-120">Header</span></span>|<span data-ttu-id="efcac-121">值</span><span class="sxs-lookup"><span data-stu-id="efcac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efcac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efcac-122">Authorization</span></span>|<span data-ttu-id="efcac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efcac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efcac-124">接受</span><span class="sxs-lookup"><span data-stu-id="efcac-124">Accept</span></span>|<span data-ttu-id="efcac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efcac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efcac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="efcac-126">Request body</span></span>
<span data-ttu-id="efcac-127">在请求正文中, 提供 androidDeviceOwnerCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efcac-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="efcac-128">下表显示创建 androidDeviceOwnerCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="efcac-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="efcac-129">属性</span><span class="sxs-lookup"><span data-stu-id="efcac-129">Property</span></span>|<span data-ttu-id="efcac-130">类型</span><span class="sxs-lookup"><span data-stu-id="efcac-130">Type</span></span>|<span data-ttu-id="efcac-131">说明</span><span class="sxs-lookup"><span data-stu-id="efcac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efcac-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efcac-132">roleScopeTagIds</span></span>|<span data-ttu-id="efcac-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="efcac-133">String collection</span></span>|<span data-ttu-id="efcac-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="efcac-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="efcac-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-136">id</span><span class="sxs-lookup"><span data-stu-id="efcac-136">id</span></span>|<span data-ttu-id="efcac-137">String</span><span class="sxs-lookup"><span data-stu-id="efcac-137">String</span></span>|<span data-ttu-id="efcac-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="efcac-138">Key of the entity.</span></span> <span data-ttu-id="efcac-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efcac-140">createdDateTime</span></span>|<span data-ttu-id="efcac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcac-141">DateTimeOffset</span></span>|<span data-ttu-id="efcac-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="efcac-142">DateTime the object was created.</span></span> <span data-ttu-id="efcac-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-144">description</span><span class="sxs-lookup"><span data-stu-id="efcac-144">description</span></span>|<span data-ttu-id="efcac-145">String</span><span class="sxs-lookup"><span data-stu-id="efcac-145">String</span></span>|<span data-ttu-id="efcac-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="efcac-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="efcac-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efcac-148">lastModifiedDateTime</span></span>|<span data-ttu-id="efcac-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcac-149">DateTimeOffset</span></span>|<span data-ttu-id="efcac-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="efcac-150">DateTime the object was last modified.</span></span> <span data-ttu-id="efcac-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-152">displayName</span><span class="sxs-lookup"><span data-stu-id="efcac-152">displayName</span></span>|<span data-ttu-id="efcac-153">String</span><span class="sxs-lookup"><span data-stu-id="efcac-153">String</span></span>|<span data-ttu-id="efcac-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="efcac-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="efcac-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-156">version</span><span class="sxs-lookup"><span data-stu-id="efcac-156">version</span></span>|<span data-ttu-id="efcac-157">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-157">Int32</span></span>|<span data-ttu-id="efcac-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="efcac-158">Version of the device configuration.</span></span> <span data-ttu-id="efcac-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efcac-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="efcac-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="efcac-160">osMinimumVersion</span></span>|<span data-ttu-id="efcac-161">String</span><span class="sxs-lookup"><span data-stu-id="efcac-161">String</span></span>|<span data-ttu-id="efcac-162">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="efcac-162">Minimum Android version.</span></span>|
|<span data-ttu-id="efcac-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="efcac-163">osMaximumVersion</span></span>|<span data-ttu-id="efcac-164">String</span><span class="sxs-lookup"><span data-stu-id="efcac-164">String</span></span>|<span data-ttu-id="efcac-165">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="efcac-165">Maximum Android version.</span></span>|
|<span data-ttu-id="efcac-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="efcac-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="efcac-167">String</span><span class="sxs-lookup"><span data-stu-id="efcac-167">String</span></span>|<span data-ttu-id="efcac-168">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="efcac-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="efcac-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="efcac-169">passwordRequired</span></span>|<span data-ttu-id="efcac-170">布尔值</span><span class="sxs-lookup"><span data-stu-id="efcac-170">Boolean</span></span>|<span data-ttu-id="efcac-171">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="efcac-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="efcac-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="efcac-172">passwordMinimumLength</span></span>|<span data-ttu-id="efcac-173">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-173">Int32</span></span>|<span data-ttu-id="efcac-174">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="efcac-174">Minimum password length.</span></span> <span data-ttu-id="efcac-175">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="efcac-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="efcac-176">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="efcac-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="efcac-177">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-177">Int32</span></span>|<span data-ttu-id="efcac-178">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="efcac-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="efcac-179">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="efcac-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="efcac-180">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="efcac-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="efcac-181">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-181">Int32</span></span>|<span data-ttu-id="efcac-182">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="efcac-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="efcac-183">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="efcac-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="efcac-184">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="efcac-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="efcac-185">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-185">Int32</span></span>|<span data-ttu-id="efcac-186">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="efcac-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="efcac-187">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="efcac-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="efcac-188">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="efcac-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="efcac-189">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-189">Int32</span></span>|<span data-ttu-id="efcac-190">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="efcac-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="efcac-191">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="efcac-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="efcac-192">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="efcac-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="efcac-193">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-193">Int32</span></span>|<span data-ttu-id="efcac-194">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="efcac-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="efcac-195">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="efcac-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="efcac-196">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="efcac-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="efcac-197">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-197">Int32</span></span>|<span data-ttu-id="efcac-198">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="efcac-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="efcac-199">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="efcac-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="efcac-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="efcac-200">passwordRequiredType</span></span>|[<span data-ttu-id="efcac-201">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="efcac-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="efcac-202">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="efcac-202">Type of characters in password.</span></span> <span data-ttu-id="efcac-203">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。</span><span class="sxs-lookup"><span data-stu-id="efcac-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="efcac-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="efcac-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="efcac-205">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-205">Int32</span></span>|<span data-ttu-id="efcac-206">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="efcac-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="efcac-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="efcac-207">passwordExpirationDays</span></span>|<span data-ttu-id="efcac-208">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-208">Int32</span></span>|<span data-ttu-id="efcac-209">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="efcac-209">Number of days before the password expires.</span></span> <span data-ttu-id="efcac-210">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="efcac-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="efcac-211">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="efcac-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="efcac-212">Int32</span><span class="sxs-lookup"><span data-stu-id="efcac-212">Int32</span></span>|<span data-ttu-id="efcac-213">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="efcac-213">Number of previous passwords to block.</span></span> <span data-ttu-id="efcac-214">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="efcac-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="efcac-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="efcac-215">storageRequireEncryption</span></span>|<span data-ttu-id="efcac-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="efcac-216">Boolean</span></span>|<span data-ttu-id="efcac-217">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="efcac-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="efcac-218">响应</span><span class="sxs-lookup"><span data-stu-id="efcac-218">Response</span></span>
<span data-ttu-id="efcac-219">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="efcac-219">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efcac-220">示例</span><span class="sxs-lookup"><span data-stu-id="efcac-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="efcac-221">请求</span><span class="sxs-lookup"><span data-stu-id="efcac-221">Request</span></span>
<span data-ttu-id="efcac-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efcac-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="efcac-223">响应</span><span class="sxs-lookup"><span data-stu-id="efcac-223">Response</span></span>
<span data-ttu-id="efcac-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efcac-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





