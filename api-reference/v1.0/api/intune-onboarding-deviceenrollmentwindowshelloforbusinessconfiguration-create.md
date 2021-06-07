---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88b85008bed7c918f109d20994d11881150942e9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743719"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1824f-103">创建 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="1824f-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="1824f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1824f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1824f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1824f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1824f-106">创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1824f-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1824f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1824f-107">Prerequisites</span></span>
<span data-ttu-id="1824f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1824f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1824f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1824f-110">Permission type</span></span>|<span data-ttu-id="1824f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1824f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1824f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1824f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1824f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1824f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1824f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1824f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1824f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1824f-115">Not supported.</span></span>|
|<span data-ttu-id="1824f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1824f-116">Application</span></span>|<span data-ttu-id="1824f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1824f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1824f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1824f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1824f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1824f-119">Request headers</span></span>
|<span data-ttu-id="1824f-120">标头</span><span class="sxs-lookup"><span data-stu-id="1824f-120">Header</span></span>|<span data-ttu-id="1824f-121">值</span><span class="sxs-lookup"><span data-stu-id="1824f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1824f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1824f-122">Authorization</span></span>|<span data-ttu-id="1824f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1824f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1824f-124">接受</span><span class="sxs-lookup"><span data-stu-id="1824f-124">Accept</span></span>|<span data-ttu-id="1824f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1824f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1824f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1824f-126">Request body</span></span>
<span data-ttu-id="1824f-127">在请求正文中，提供 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1824f-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="1824f-128">下表显示创建 deviceEnrollmentWindowsHelloForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1824f-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="1824f-129">属性</span><span class="sxs-lookup"><span data-stu-id="1824f-129">Property</span></span>|<span data-ttu-id="1824f-130">类型</span><span class="sxs-lookup"><span data-stu-id="1824f-130">Type</span></span>|<span data-ttu-id="1824f-131">说明</span><span class="sxs-lookup"><span data-stu-id="1824f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1824f-132">id</span><span class="sxs-lookup"><span data-stu-id="1824f-132">id</span></span>|<span data-ttu-id="1824f-133">String</span><span class="sxs-lookup"><span data-stu-id="1824f-133">String</span></span>|<span data-ttu-id="1824f-134">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1824f-135">displayName</span></span>|<span data-ttu-id="1824f-136">String</span><span class="sxs-lookup"><span data-stu-id="1824f-136">String</span></span>|<span data-ttu-id="1824f-137">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-138">说明</span><span class="sxs-lookup"><span data-stu-id="1824f-138">description</span></span>|<span data-ttu-id="1824f-139">String</span><span class="sxs-lookup"><span data-stu-id="1824f-139">String</span></span>|<span data-ttu-id="1824f-140">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-141">priority</span><span class="sxs-lookup"><span data-stu-id="1824f-141">priority</span></span>|<span data-ttu-id="1824f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1824f-142">Int32</span></span>|<span data-ttu-id="1824f-143">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="1824f-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="1824f-144">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="1824f-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="1824f-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1824f-146">createdDateTime</span></span>|<span data-ttu-id="1824f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1824f-147">DateTimeOffset</span></span>|<span data-ttu-id="1824f-148">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1824f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="1824f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1824f-150">DateTimeOffset</span></span>|<span data-ttu-id="1824f-151">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-152">version</span><span class="sxs-lookup"><span data-stu-id="1824f-152">version</span></span>|<span data-ttu-id="1824f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1824f-153">Int32</span></span>|<span data-ttu-id="1824f-154">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1824f-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1824f-155">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1824f-155">pinMinimumLength</span></span>|<span data-ttu-id="1824f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1824f-156">Int32</span></span>|<span data-ttu-id="1824f-157">控制 Hello 企业 PIN 所需的最少Windows字符数。</span><span class="sxs-lookup"><span data-stu-id="1824f-157">Controls the minimum number of characters required for the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="1824f-158">此值必须介于 4 到 127 之间（包含 4 和 127 之间，并且小于或等于为最大 PIN 设置的值）。</span><span class="sxs-lookup"><span data-stu-id="1824f-158">This value must be between 4 and 127, inclusive, and less than or equal to the value set for the maximum PIN.</span></span>|
|<span data-ttu-id="1824f-159">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1824f-159">pinMaximumLength</span></span>|<span data-ttu-id="1824f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1824f-160">Int32</span></span>|<span data-ttu-id="1824f-161">控制 Hello 企业 PIN 允许的最大Windows数。</span><span class="sxs-lookup"><span data-stu-id="1824f-161">Controls the maximum number of characters allowed for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="1824f-162">此值必须介于 4 和 127 之间（包含两者）。</span><span class="sxs-lookup"><span data-stu-id="1824f-162">This value must be between 4 and 127, inclusive.</span></span> <span data-ttu-id="1824f-163">此值必须大于或等于为最小 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="1824f-163">This value must be greater than or equal to the value set for the minimum PIN.</span></span>|
|<span data-ttu-id="1824f-164">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1824f-164">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1824f-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1824f-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1824f-166">控制在 Hello 企业 PIN Windows大写字母的能力。</span><span class="sxs-lookup"><span data-stu-id="1824f-166">Controls the ability to use uppercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="1824f-167">Allowed 允许使用大写字母 (大写) ，而 Required 可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="1824f-167">Allowed permits the use of uppercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="1824f-168">如果设置为"不允许"，则不允许使用大写字母。</span><span class="sxs-lookup"><span data-stu-id="1824f-168">If set to Not Allowed, uppercase letters will not be permitted.</span></span> <span data-ttu-id="1824f-169">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="1824f-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1824f-170">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1824f-170">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1824f-171">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1824f-171">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1824f-172">控制在 Hello 企业 PIN 中Windows小写字母的能力。</span><span class="sxs-lookup"><span data-stu-id="1824f-172">Controls the ability to use lowercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="1824f-173">Allowed 允许使用小写字母 () ，而 Required 可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="1824f-173">Allowed permits the use of lowercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="1824f-174">如果设置为"不允许"，则不允许使用小写字母。</span><span class="sxs-lookup"><span data-stu-id="1824f-174">If set to Not Allowed, lowercase letters will not be permitted.</span></span> <span data-ttu-id="1824f-175">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="1824f-175">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1824f-176">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1824f-176">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1824f-177">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1824f-177">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1824f-178">控制在 Hello 企业 PIN 中Windows字符的能力。</span><span class="sxs-lookup"><span data-stu-id="1824f-178">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="1824f-179">允许允许使用特殊字符 (字符) ，而 Required 可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="1824f-179">Allowed permits the use of special character(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="1824f-180">如果设置为"不允许"， (不允许) 特殊字符。</span><span class="sxs-lookup"><span data-stu-id="1824f-180">If set to Not Allowed, special character(s) will not be permitted.</span></span> <span data-ttu-id="1824f-181">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="1824f-181">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1824f-182">state</span><span class="sxs-lookup"><span data-stu-id="1824f-182">state</span></span>|[<span data-ttu-id="1824f-183">enablement</span><span class="sxs-lookup"><span data-stu-id="1824f-183">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="1824f-184">控制是否允许为 Hello 企业Windows设备。</span><span class="sxs-lookup"><span data-stu-id="1824f-184">Controls whether to allow the device to be configured for Windows Hello for Business.</span></span> <span data-ttu-id="1824f-185">如果设置为禁用，则用户无法预配 Windows Hello 企业版，除非Azure Active Directory已加入的移动电话上（如果需要）。</span><span class="sxs-lookup"><span data-stu-id="1824f-185">If set to disabled, the user cannot provision Windows Hello for Business except on Azure Active Directory joined mobile phones if otherwise required.</span></span> <span data-ttu-id="1824f-186">如果设置为"未配置"，Intune 将不会覆盖客户端默认值。</span><span class="sxs-lookup"><span data-stu-id="1824f-186">If set to Not Configured, Intune will not override client defaults.</span></span> <span data-ttu-id="1824f-187">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1824f-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1824f-188">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1824f-188">securityDeviceRequired</span></span>|<span data-ttu-id="1824f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1824f-189">Boolean</span></span>|<span data-ttu-id="1824f-190">控制是否需要受信任的平台模块 (TPM) Hello 企业Windows预配。</span><span class="sxs-lookup"><span data-stu-id="1824f-190">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="1824f-191">TPM 提供了额外的安全优势，因为存储在 TPM 上的数据不能用于其他设备。</span><span class="sxs-lookup"><span data-stu-id="1824f-191">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="1824f-192">如果设置为 False，则所有设备都可以预配 Windows Hello 企业，即使没有可用 TPM。</span><span class="sxs-lookup"><span data-stu-id="1824f-192">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="1824f-193">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1824f-193">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1824f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1824f-194">Boolean</span></span>|<span data-ttu-id="1824f-195">控制将生物识别手势（如人脸和指纹）用作 Windows Hello 企业 PIN 的替代方法。</span><span class="sxs-lookup"><span data-stu-id="1824f-195">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="1824f-196">如果设置为 False，则不允许生物识别手势。</span><span class="sxs-lookup"><span data-stu-id="1824f-196">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="1824f-197">用户仍必须将 PIN 配置为备份，以防发生故障。</span><span class="sxs-lookup"><span data-stu-id="1824f-197">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="1824f-198">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="1824f-198">remotePassportEnabled</span></span>|<span data-ttu-id="1824f-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1824f-199">Boolean</span></span>|<span data-ttu-id="1824f-200">控制使用远程 Windows Hello 企业。</span><span class="sxs-lookup"><span data-stu-id="1824f-200">Controls the use of Remote Windows Hello for Business.</span></span> <span data-ttu-id="1824f-201">通过Windows Hello 企业版，可移植的已注册设备可以用作桌面身份验证的配套设备。</span><span class="sxs-lookup"><span data-stu-id="1824f-201">Remote Windows Hello for Business provides the ability for a portable, registered device to be usable as a companion for desktop authentication.</span></span> <span data-ttu-id="1824f-202">桌面必须加入 Azure AD，配套设备必须具有 Windows Hello 企业版 PIN。</span><span class="sxs-lookup"><span data-stu-id="1824f-202">The desktop must be Azure AD joined and the companion device must have a Windows Hello for Business PIN.</span></span>|
|<span data-ttu-id="1824f-203">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1824f-203">pinPreviousBlockCount</span></span>|<span data-ttu-id="1824f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="1824f-204">Int32</span></span>|<span data-ttu-id="1824f-205">控制阻止用户使用过去 PIN 的能力。</span><span class="sxs-lookup"><span data-stu-id="1824f-205">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="1824f-206">必须将其设置为 0 到 50（含 0 和 50）之间，并且用户的当前 PIN 包含在该计数中。</span><span class="sxs-lookup"><span data-stu-id="1824f-206">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="1824f-207">如果设置为 0，则不存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="1824f-207">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="1824f-208">PIN 历史记录不会通过 PIN 重置保留。</span><span class="sxs-lookup"><span data-stu-id="1824f-208">PIN history is not preserved through a PIN reset.</span></span>|
|<span data-ttu-id="1824f-209">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1824f-209">pinExpirationInDays</span></span>|<span data-ttu-id="1824f-210">Int32</span><span class="sxs-lookup"><span data-stu-id="1824f-210">Int32</span></span>|<span data-ttu-id="1824f-211">控制在系统 (PIN 之前) PIN 的时间段（以天表示）。</span><span class="sxs-lookup"><span data-stu-id="1824f-211">Controls the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="1824f-212">这必须设置为 0 到 730 之间（包含这两者）。</span><span class="sxs-lookup"><span data-stu-id="1824f-212">This must be set between 0 and 730, inclusive.</span></span> <span data-ttu-id="1824f-213">如果设置为 0，则用户的 PIN 永不过期</span><span class="sxs-lookup"><span data-stu-id="1824f-213">If set to 0, the user's PIN will never expire</span></span>|
|<span data-ttu-id="1824f-214">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="1824f-214">enhancedBiometricsState</span></span>|[<span data-ttu-id="1824f-215">enablement</span><span class="sxs-lookup"><span data-stu-id="1824f-215">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="1824f-216">控制在支持防欺骗功能的设备上使用反欺骗功能进行面部识别的能力。</span><span class="sxs-lookup"><span data-stu-id="1824f-216">Controls the ability to use the anti-spoofing features for facial recognition on devices which support it.</span></span> <span data-ttu-id="1824f-217">如果设置为禁用，则不允许使用反欺骗功能。</span><span class="sxs-lookup"><span data-stu-id="1824f-217">If set to disabled, anti-spoofing features are not allowed.</span></span> <span data-ttu-id="1824f-218">如果设置为"未配置"，用户可以选择是否要使用反欺骗。</span><span class="sxs-lookup"><span data-stu-id="1824f-218">If set to Not Configured, the user can choose whether they want to use anti-spoofing.</span></span> <span data-ttu-id="1824f-219">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1824f-219">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1824f-220">响应</span><span class="sxs-lookup"><span data-stu-id="1824f-220">Response</span></span>
<span data-ttu-id="1824f-221">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1824f-221">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1824f-222">示例</span><span class="sxs-lookup"><span data-stu-id="1824f-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="1824f-223">请求</span><span class="sxs-lookup"><span data-stu-id="1824f-223">Request</span></span>
<span data-ttu-id="1824f-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1824f-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="1824f-225">响应</span><span class="sxs-lookup"><span data-stu-id="1824f-225">Response</span></span>
<span data-ttu-id="1824f-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1824f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```




