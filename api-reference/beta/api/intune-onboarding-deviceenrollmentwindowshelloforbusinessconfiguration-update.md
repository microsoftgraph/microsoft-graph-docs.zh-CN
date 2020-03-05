---
title: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 更新 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afc1f06e958f15fa2a417d8d32874c1039d65a23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462185"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="b22c3-103">更新 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="b22c3-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="b22c3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b22c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b22c3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b22c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b22c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b22c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b22c3-107">更新 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b22c3-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b22c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b22c3-108">Prerequisites</span></span>
<span data-ttu-id="b22c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b22c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b22c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b22c3-111">Permission type</span></span>|<span data-ttu-id="b22c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b22c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b22c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b22c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b22c3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b22c3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b22c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b22c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b22c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b22c3-116">Not supported.</span></span>|
|<span data-ttu-id="b22c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b22c3-117">Application</span></span>|<span data-ttu-id="b22c3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b22c3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b22c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b22c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b22c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b22c3-120">Request headers</span></span>
|<span data-ttu-id="b22c3-121">标头</span><span class="sxs-lookup"><span data-stu-id="b22c3-121">Header</span></span>|<span data-ttu-id="b22c3-122">值</span><span class="sxs-lookup"><span data-stu-id="b22c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b22c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b22c3-123">Authorization</span></span>|<span data-ttu-id="b22c3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b22c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b22c3-125">接受</span><span class="sxs-lookup"><span data-stu-id="b22c3-125">Accept</span></span>|<span data-ttu-id="b22c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b22c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b22c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b22c3-127">Request body</span></span>
<span data-ttu-id="b22c3-128">在请求正文中，提供 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b22c3-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="b22c3-129">下表显示创建 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b22c3-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="b22c3-130">属性</span><span class="sxs-lookup"><span data-stu-id="b22c3-130">Property</span></span>|<span data-ttu-id="b22c3-131">类型</span><span class="sxs-lookup"><span data-stu-id="b22c3-131">Type</span></span>|<span data-ttu-id="b22c3-132">说明</span><span class="sxs-lookup"><span data-stu-id="b22c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b22c3-133">id</span><span class="sxs-lookup"><span data-stu-id="b22c3-133">id</span></span>|<span data-ttu-id="b22c3-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b22c3-134">String</span></span>|<span data-ttu-id="b22c3-135">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b22c3-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b22c3-136">displayName</span></span>|<span data-ttu-id="b22c3-137">String</span><span class="sxs-lookup"><span data-stu-id="b22c3-137">String</span></span>|<span data-ttu-id="b22c3-138">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="b22c3-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-139">说明</span><span class="sxs-lookup"><span data-stu-id="b22c3-139">description</span></span>|<span data-ttu-id="b22c3-140">String</span><span class="sxs-lookup"><span data-stu-id="b22c3-140">String</span></span>|<span data-ttu-id="b22c3-141">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="b22c3-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-142">priority</span><span class="sxs-lookup"><span data-stu-id="b22c3-142">priority</span></span>|<span data-ttu-id="b22c3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b22c3-143">Int32</span></span>|<span data-ttu-id="b22c3-144">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="b22c3-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="b22c3-145">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="b22c3-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="b22c3-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b22c3-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b22c3-147">createdDateTime</span></span>|<span data-ttu-id="b22c3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b22c3-148">DateTimeOffset</span></span>|<span data-ttu-id="b22c3-149">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="b22c3-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b22c3-150">lastModifiedDateTime</span></span>|<span data-ttu-id="b22c3-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b22c3-151">DateTimeOffset</span></span>|<span data-ttu-id="b22c3-152">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="b22c3-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-153">version</span><span class="sxs-lookup"><span data-stu-id="b22c3-153">version</span></span>|<span data-ttu-id="b22c3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b22c3-154">Int32</span></span>|<span data-ttu-id="b22c3-155">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="b22c3-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b22c3-156">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b22c3-156">pinMinimumLength</span></span>|<span data-ttu-id="b22c3-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b22c3-157">Int32</span></span>|<span data-ttu-id="b22c3-158">控制 Windows Hello 企业版 PIN 所需的最小字符数。</span><span class="sxs-lookup"><span data-stu-id="b22c3-158">Controls the minimum number of characters required for the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="b22c3-159">此值必须介于4和127之间（含这两个值），且小于或等于为最大 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="b22c3-159">This value must be between 4 and 127, inclusive, and less than or equal to the value set for the maximum PIN.</span></span>|
|<span data-ttu-id="b22c3-160">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="b22c3-160">pinMaximumLength</span></span>|<span data-ttu-id="b22c3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b22c3-161">Int32</span></span>|<span data-ttu-id="b22c3-162">控制 Windows Hello 企业版 PIN 所允许的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="b22c3-162">Controls the maximum number of characters allowed for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="b22c3-163">此值必须介于4和127之间（含这两个值）。</span><span class="sxs-lookup"><span data-stu-id="b22c3-163">This value must be between 4 and 127, inclusive.</span></span> <span data-ttu-id="b22c3-164">此值必须大于或等于为最小 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="b22c3-164">This value must be greater than or equal to the value set for the minimum PIN.</span></span>|
|<span data-ttu-id="b22c3-165">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b22c3-165">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="b22c3-166">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b22c3-166">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="b22c3-167">控制在 Windows Hello 企业版 PIN 中使用大写字母的功能。</span><span class="sxs-lookup"><span data-stu-id="b22c3-167">Controls the ability to use uppercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="b22c3-168">允许使用大写字母（s），而必需的字符可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="b22c3-168">Allowed permits the use of uppercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="b22c3-169">如果设置为 "不允许"，则不允许使用大写字母。</span><span class="sxs-lookup"><span data-stu-id="b22c3-169">If set to Not Allowed, uppercase letters will not be permitted.</span></span> <span data-ttu-id="b22c3-170">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="b22c3-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b22c3-171">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b22c3-171">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="b22c3-172">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b22c3-172">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="b22c3-173">控制在 Windows Hello 企业版 PIN 中使用小写字母的功能。</span><span class="sxs-lookup"><span data-stu-id="b22c3-173">Controls the ability to use lowercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="b22c3-174">允许使用小写字母，而必需的则可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="b22c3-174">Allowed permits the use of lowercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="b22c3-175">如果设置为 "不允许"，则不允许使用小写字母。</span><span class="sxs-lookup"><span data-stu-id="b22c3-175">If set to Not Allowed, lowercase letters will not be permitted.</span></span> <span data-ttu-id="b22c3-176">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="b22c3-176">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b22c3-177">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b22c3-177">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="b22c3-178">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="b22c3-178">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="b22c3-179">控制在 Windows Hello 企业版 PIN 中使用特殊字符的功能。</span><span class="sxs-lookup"><span data-stu-id="b22c3-179">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="b22c3-180">允许使用特殊字符，而必需的字符可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="b22c3-180">Allowed permits the use of special character(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="b22c3-181">如果设置为 "不允许"，则不允许使用特殊字符。</span><span class="sxs-lookup"><span data-stu-id="b22c3-181">If set to Not Allowed, special character(s) will not be permitted.</span></span> <span data-ttu-id="b22c3-182">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="b22c3-182">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b22c3-183">state</span><span class="sxs-lookup"><span data-stu-id="b22c3-183">state</span></span>|[<span data-ttu-id="b22c3-184">启用</span><span class="sxs-lookup"><span data-stu-id="b22c3-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b22c3-185">控制是否允许为 Windows Hello 企业版配置设备。</span><span class="sxs-lookup"><span data-stu-id="b22c3-185">Controls whether to allow the device to be configured for Windows Hello for Business.</span></span> <span data-ttu-id="b22c3-186">如果设置为 "禁用"，则用户将无法预配 Windows Hello 企业版，除非在其他情况下有必要时在 Azure Active Directory 加入移动电话上。</span><span class="sxs-lookup"><span data-stu-id="b22c3-186">If set to disabled, the user cannot provision Windows Hello for Business except on Azure Active Directory joined mobile phones if otherwise required.</span></span> <span data-ttu-id="b22c3-187">如果设置为 "未配置"，Intune 将不会覆盖客户端默认设置。</span><span class="sxs-lookup"><span data-stu-id="b22c3-187">If set to Not Configured, Intune will not override client defaults.</span></span> <span data-ttu-id="b22c3-188">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b22c3-188">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b22c3-189">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="b22c3-189">securityDeviceRequired</span></span>|<span data-ttu-id="b22c3-190">布尔</span><span class="sxs-lookup"><span data-stu-id="b22c3-190">Boolean</span></span>|<span data-ttu-id="b22c3-191">控制是否需要用于设置 Windows Hello 企业版的受信任的平台模块（TPM）。</span><span class="sxs-lookup"><span data-stu-id="b22c3-191">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="b22c3-192">TPM 在其他设备上不能使用存储在其上的数据带来额外的安全性优势。</span><span class="sxs-lookup"><span data-stu-id="b22c3-192">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="b22c3-193">如果设置为 False，即使没有可用的 TPM，所有设备也可以预配 Windows Hello 企业版。</span><span class="sxs-lookup"><span data-stu-id="b22c3-193">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="b22c3-194">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="b22c3-194">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="b22c3-195">布尔</span><span class="sxs-lookup"><span data-stu-id="b22c3-195">Boolean</span></span>|<span data-ttu-id="b22c3-196">控制使用生物特征手势（如面孔和指纹）作为 Windows Hello 企业版 PIN 的替代方法。</span><span class="sxs-lookup"><span data-stu-id="b22c3-196">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="b22c3-197">如果设置为 False，则不允许使用生物特征手势。</span><span class="sxs-lookup"><span data-stu-id="b22c3-197">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="b22c3-198">用户仍必须在发生故障时将 PIN 配置为备份。</span><span class="sxs-lookup"><span data-stu-id="b22c3-198">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="b22c3-199">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="b22c3-199">remotePassportEnabled</span></span>|<span data-ttu-id="b22c3-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b22c3-200">Boolean</span></span>|<span data-ttu-id="b22c3-201">控制远程 Windows Hello 企业版的使用。</span><span class="sxs-lookup"><span data-stu-id="b22c3-201">Controls the use of Remote Windows Hello for Business.</span></span> <span data-ttu-id="b22c3-202">远程 Windows Hello 企业版使便携式、注册设备可用作桌面身份验证的配套功能。</span><span class="sxs-lookup"><span data-stu-id="b22c3-202">Remote Windows Hello for Business provides the ability for a portable, registered device to be usable as a companion for desktop authentication.</span></span> <span data-ttu-id="b22c3-203">桌面必须已加入 Azure AD，且配套设备必须具有 Windows Hello 企业版 PIN。</span><span class="sxs-lookup"><span data-stu-id="b22c3-203">The desktop must be Azure AD joined and the companion device must have a Windows Hello for Business PIN.</span></span>|
|<span data-ttu-id="b22c3-204">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="b22c3-204">pinPreviousBlockCount</span></span>|<span data-ttu-id="b22c3-205">Int32</span><span class="sxs-lookup"><span data-stu-id="b22c3-205">Int32</span></span>|<span data-ttu-id="b22c3-206">控制阻止用户使用过去的 Pin 的功能。</span><span class="sxs-lookup"><span data-stu-id="b22c3-206">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="b22c3-207">必须在0和50之间设置此值（包括这两个值），并且用户的当前 PIN 包含在该计数中。</span><span class="sxs-lookup"><span data-stu-id="b22c3-207">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="b22c3-208">如果设置为0，则不存储以前的 Pin。</span><span class="sxs-lookup"><span data-stu-id="b22c3-208">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="b22c3-209">PIN 历史记录不会通过 PIN 重置来保留。</span><span class="sxs-lookup"><span data-stu-id="b22c3-209">PIN history is not preserved through a PIN reset.</span></span>|
|<span data-ttu-id="b22c3-210">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="b22c3-210">pinExpirationInDays</span></span>|<span data-ttu-id="b22c3-211">Int32</span><span class="sxs-lookup"><span data-stu-id="b22c3-211">Int32</span></span>|<span data-ttu-id="b22c3-212">控制在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="b22c3-212">Controls the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="b22c3-213">必须在0和730之间设置此值（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="b22c3-213">This must be set between 0 and 730, inclusive.</span></span> <span data-ttu-id="b22c3-214">如果设置为0，则用户的 PIN 永不过期</span><span class="sxs-lookup"><span data-stu-id="b22c3-214">If set to 0, the user's PIN will never expire</span></span>|
|<span data-ttu-id="b22c3-215">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="b22c3-215">enhancedBiometricsState</span></span>|[<span data-ttu-id="b22c3-216">启用</span><span class="sxs-lookup"><span data-stu-id="b22c3-216">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b22c3-217">控制在支持它的设备上使用反欺骗功能进行面部识别。</span><span class="sxs-lookup"><span data-stu-id="b22c3-217">Controls the ability to use the anti-spoofing features for facial recognition on devices which support it.</span></span> <span data-ttu-id="b22c3-218">如果设置为 "禁用"，则不允许反欺骗功能。</span><span class="sxs-lookup"><span data-stu-id="b22c3-218">If set to disabled, anti-spoofing features are not allowed.</span></span> <span data-ttu-id="b22c3-219">如果设置为 "未配置"，则用户可以选择是否要使用反欺骗。</span><span class="sxs-lookup"><span data-stu-id="b22c3-219">If set to Not Configured, the user can choose whether they want to use anti-spoofing.</span></span> <span data-ttu-id="b22c3-220">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b22c3-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b22c3-221">securityKeyForSignIn</span><span class="sxs-lookup"><span data-stu-id="b22c3-221">securityKeyForSignIn</span></span>|[<span data-ttu-id="b22c3-222">启用</span><span class="sxs-lookup"><span data-stu-id="b22c3-222">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b22c3-223">登录的安全密钥提供远程开启/关闭 Windows Hello Sercurity Keyl 的容量。未配置将服从在 clinet 上完成的配置。</span><span class="sxs-lookup"><span data-stu-id="b22c3-223">Security key for Sign In provides the capacity for remotely turning ON/OFF Windows Hello Sercurity Keyl Not configured will honor configurations done on the clinet.</span></span> <span data-ttu-id="b22c3-224">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b22c3-224">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="b22c3-225">响应</span><span class="sxs-lookup"><span data-stu-id="b22c3-225">Response</span></span>
<span data-ttu-id="b22c3-226">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b22c3-226">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b22c3-227">示例</span><span class="sxs-lookup"><span data-stu-id="b22c3-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="b22c3-228">请求</span><span class="sxs-lookup"><span data-stu-id="b22c3-228">Request</span></span>
<span data-ttu-id="b22c3-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b22c3-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 667

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
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="b22c3-230">响应</span><span class="sxs-lookup"><span data-stu-id="b22c3-230">Response</span></span>
<span data-ttu-id="b22c3-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b22c3-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 839

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
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```





