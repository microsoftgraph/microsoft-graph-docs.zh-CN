---
title: 创建 androidDeviceOwnerCompliancePolicy
description: 创建新的 androidDeviceOwnerCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0c605380f12d9144f322f8e2d5ef46c62c37e58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312682"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="f6233-103">创建 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f6233-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="f6233-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6233-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6233-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6233-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6233-106">创建新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f6233-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6233-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6233-107">Prerequisites</span></span>
<span data-ttu-id="f6233-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6233-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6233-110">Permission type</span></span>|<span data-ttu-id="f6233-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f6233-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6233-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6233-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6233-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6233-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6233-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6233-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6233-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6233-115">Not supported.</span></span>|
|<span data-ttu-id="f6233-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6233-116">Application</span></span>|<span data-ttu-id="f6233-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6233-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6233-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6233-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f6233-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6233-119">Request headers</span></span>
|<span data-ttu-id="f6233-120">标头</span><span class="sxs-lookup"><span data-stu-id="f6233-120">Header</span></span>|<span data-ttu-id="f6233-121">值</span><span class="sxs-lookup"><span data-stu-id="f6233-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6233-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6233-122">Authorization</span></span>|<span data-ttu-id="f6233-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6233-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6233-124">接受</span><span class="sxs-lookup"><span data-stu-id="f6233-124">Accept</span></span>|<span data-ttu-id="f6233-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6233-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6233-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6233-126">Request body</span></span>
<span data-ttu-id="f6233-127">在请求正文中, 提供 androidDeviceOwnerCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6233-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="f6233-128">下表显示创建 androidDeviceOwnerCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f6233-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="f6233-129">属性</span><span class="sxs-lookup"><span data-stu-id="f6233-129">Property</span></span>|<span data-ttu-id="f6233-130">类型</span><span class="sxs-lookup"><span data-stu-id="f6233-130">Type</span></span>|<span data-ttu-id="f6233-131">说明</span><span class="sxs-lookup"><span data-stu-id="f6233-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6233-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6233-132">roleScopeTagIds</span></span>|<span data-ttu-id="f6233-133">String collection</span><span class="sxs-lookup"><span data-stu-id="f6233-133">String collection</span></span>|<span data-ttu-id="f6233-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f6233-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6233-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-136">id</span><span class="sxs-lookup"><span data-stu-id="f6233-136">id</span></span>|<span data-ttu-id="f6233-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f6233-137">String</span></span>|<span data-ttu-id="f6233-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f6233-138">Key of the entity.</span></span> <span data-ttu-id="f6233-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6233-140">createdDateTime</span></span>|<span data-ttu-id="f6233-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6233-141">DateTimeOffset</span></span>|<span data-ttu-id="f6233-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6233-142">DateTime the object was created.</span></span> <span data-ttu-id="f6233-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-144">说明</span><span class="sxs-lookup"><span data-stu-id="f6233-144">description</span></span>|<span data-ttu-id="f6233-145">String</span><span class="sxs-lookup"><span data-stu-id="f6233-145">String</span></span>|<span data-ttu-id="f6233-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f6233-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6233-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6233-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f6233-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6233-149">DateTimeOffset</span></span>|<span data-ttu-id="f6233-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6233-150">DateTime the object was last modified.</span></span> <span data-ttu-id="f6233-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f6233-152">displayName</span></span>|<span data-ttu-id="f6233-153">字符串</span><span class="sxs-lookup"><span data-stu-id="f6233-153">String</span></span>|<span data-ttu-id="f6233-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f6233-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6233-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-156">version</span><span class="sxs-lookup"><span data-stu-id="f6233-156">version</span></span>|<span data-ttu-id="f6233-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-157">Int32</span></span>|<span data-ttu-id="f6233-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f6233-158">Version of the device configuration.</span></span> <span data-ttu-id="f6233-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6233-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6233-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f6233-160">osMinimumVersion</span></span>|<span data-ttu-id="f6233-161">String</span><span class="sxs-lookup"><span data-stu-id="f6233-161">String</span></span>|<span data-ttu-id="f6233-162">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="f6233-162">Minimum Android version.</span></span>|
|<span data-ttu-id="f6233-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f6233-163">osMaximumVersion</span></span>|<span data-ttu-id="f6233-164">String</span><span class="sxs-lookup"><span data-stu-id="f6233-164">String</span></span>|<span data-ttu-id="f6233-165">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="f6233-165">Maximum Android version.</span></span>|
|<span data-ttu-id="f6233-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f6233-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="f6233-167">String</span><span class="sxs-lookup"><span data-stu-id="f6233-167">String</span></span>|<span data-ttu-id="f6233-168">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="f6233-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="f6233-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f6233-169">passwordRequired</span></span>|<span data-ttu-id="f6233-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6233-170">Boolean</span></span>|<span data-ttu-id="f6233-171">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="f6233-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="f6233-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f6233-172">passwordMinimumLength</span></span>|<span data-ttu-id="f6233-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-173">Int32</span></span>|<span data-ttu-id="f6233-174">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="f6233-174">Minimum password length.</span></span> <span data-ttu-id="f6233-175">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="f6233-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f6233-176">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f6233-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="f6233-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-177">Int32</span></span>|<span data-ttu-id="f6233-178">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="f6233-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="f6233-179">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="f6233-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f6233-180">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f6233-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="f6233-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-181">Int32</span></span>|<span data-ttu-id="f6233-182">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="f6233-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="f6233-183">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="f6233-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f6233-184">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f6233-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="f6233-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-185">Int32</span></span>|<span data-ttu-id="f6233-186">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="f6233-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="f6233-187">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="f6233-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f6233-188">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="f6233-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="f6233-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-189">Int32</span></span>|<span data-ttu-id="f6233-190">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="f6233-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="f6233-191">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="f6233-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f6233-192">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="f6233-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="f6233-193">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-193">Int32</span></span>|<span data-ttu-id="f6233-194">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="f6233-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="f6233-195">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="f6233-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f6233-196">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f6233-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="f6233-197">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-197">Int32</span></span>|<span data-ttu-id="f6233-198">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="f6233-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="f6233-199">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="f6233-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f6233-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f6233-200">passwordRequiredType</span></span>|[<span data-ttu-id="f6233-201">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f6233-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="f6233-202">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="f6233-202">Type of characters in password.</span></span> <span data-ttu-id="f6233-203">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。</span><span class="sxs-lookup"><span data-stu-id="f6233-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="f6233-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f6233-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f6233-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-205">Int32</span></span>|<span data-ttu-id="f6233-206">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f6233-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f6233-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f6233-207">passwordExpirationDays</span></span>|<span data-ttu-id="f6233-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-208">Int32</span></span>|<span data-ttu-id="f6233-209">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="f6233-209">Number of days before the password expires.</span></span> <span data-ttu-id="f6233-210">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="f6233-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f6233-211">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="f6233-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="f6233-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f6233-212">Int32</span></span>|<span data-ttu-id="f6233-213">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f6233-213">Number of previous passwords to block.</span></span> <span data-ttu-id="f6233-214">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="f6233-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f6233-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f6233-215">storageRequireEncryption</span></span>|<span data-ttu-id="f6233-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6233-216">Boolean</span></span>|<span data-ttu-id="f6233-217">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="f6233-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f6233-218">响应</span><span class="sxs-lookup"><span data-stu-id="f6233-218">Response</span></span>
<span data-ttu-id="f6233-219">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f6233-219">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6233-220">示例</span><span class="sxs-lookup"><span data-stu-id="f6233-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6233-221">请求</span><span class="sxs-lookup"><span data-stu-id="f6233-221">Request</span></span>
<span data-ttu-id="f6233-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6233-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6233-223">响应</span><span class="sxs-lookup"><span data-stu-id="f6233-223">Response</span></span>
<span data-ttu-id="f6233-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6233-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






