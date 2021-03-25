---
title: 创建 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 创建新的 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b07a10f3a3a5e7ceb590c2f56650c03eaa1cad10
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158855"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="a9fea-103">创建 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9fea-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="a9fea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9fea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9fea-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9fea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9fea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9fea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9fea-107">创建新的 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9fea-107">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9fea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9fea-108">Prerequisites</span></span>
<span data-ttu-id="a9fea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9fea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9fea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9fea-111">Permission type</span></span>|<span data-ttu-id="a9fea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9fea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9fea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9fea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9fea-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9fea-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a9fea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9fea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9fea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9fea-116">Not supported.</span></span>|
|<span data-ttu-id="a9fea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9fea-117">Application</span></span>|<span data-ttu-id="a9fea-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9fea-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9fea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9fea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9fea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9fea-120">Request headers</span></span>
|<span data-ttu-id="a9fea-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9fea-121">Header</span></span>|<span data-ttu-id="a9fea-122">值</span><span class="sxs-lookup"><span data-stu-id="a9fea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9fea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9fea-123">Authorization</span></span>|<span data-ttu-id="a9fea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9fea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9fea-125">接受</span><span class="sxs-lookup"><span data-stu-id="a9fea-125">Accept</span></span>|<span data-ttu-id="a9fea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9fea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9fea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9fea-127">Request body</span></span>
<span data-ttu-id="a9fea-128">在请求正文中，提供 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9fea-128">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="a9fea-129">下表显示创建 deviceEnrollmentWindowsHelloForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9fea-129">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="a9fea-130">属性</span><span class="sxs-lookup"><span data-stu-id="a9fea-130">Property</span></span>|<span data-ttu-id="a9fea-131">类型</span><span class="sxs-lookup"><span data-stu-id="a9fea-131">Type</span></span>|<span data-ttu-id="a9fea-132">说明</span><span class="sxs-lookup"><span data-stu-id="a9fea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9fea-133">id</span><span class="sxs-lookup"><span data-stu-id="a9fea-133">id</span></span>|<span data-ttu-id="a9fea-134">String</span><span class="sxs-lookup"><span data-stu-id="a9fea-134">String</span></span>|<span data-ttu-id="a9fea-135">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a9fea-136">displayName</span></span>|<span data-ttu-id="a9fea-137">String</span><span class="sxs-lookup"><span data-stu-id="a9fea-137">String</span></span>|<span data-ttu-id="a9fea-138">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-139">说明</span><span class="sxs-lookup"><span data-stu-id="a9fea-139">description</span></span>|<span data-ttu-id="a9fea-140">String</span><span class="sxs-lookup"><span data-stu-id="a9fea-140">String</span></span>|<span data-ttu-id="a9fea-141">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-142">priority</span><span class="sxs-lookup"><span data-stu-id="a9fea-142">priority</span></span>|<span data-ttu-id="a9fea-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fea-143">Int32</span></span>|<span data-ttu-id="a9fea-144">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="a9fea-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a9fea-145">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="a9fea-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="a9fea-146">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9fea-147">createdDateTime</span></span>|<span data-ttu-id="a9fea-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9fea-148">DateTimeOffset</span></span>|<span data-ttu-id="a9fea-149">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9fea-150">lastModifiedDateTime</span></span>|<span data-ttu-id="a9fea-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9fea-151">DateTimeOffset</span></span>|<span data-ttu-id="a9fea-152">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-153">version</span><span class="sxs-lookup"><span data-stu-id="a9fea-153">version</span></span>|<span data-ttu-id="a9fea-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fea-154">Int32</span></span>|<span data-ttu-id="a9fea-155">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9fea-156">roleScopeTagIds</span></span>|<span data-ttu-id="a9fea-157">String collection</span><span class="sxs-lookup"><span data-stu-id="a9fea-157">String collection</span></span>|<span data-ttu-id="a9fea-158">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="a9fea-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="a9fea-159">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fea-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a9fea-160">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a9fea-160">pinMinimumLength</span></span>|<span data-ttu-id="a9fea-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fea-161">Int32</span></span>|<span data-ttu-id="a9fea-162">控制 Windows Hello 企业 PIN 所需的最少字符数。</span><span class="sxs-lookup"><span data-stu-id="a9fea-162">Controls the minimum number of characters required for the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a9fea-163">此值必须介于 4 到 127 之间（包含 4 和 127 之间，并且小于或等于为最大 PIN 设置的值）。</span><span class="sxs-lookup"><span data-stu-id="a9fea-163">This value must be between 4 and 127, inclusive, and less than or equal to the value set for the maximum PIN.</span></span>|
|<span data-ttu-id="a9fea-164">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a9fea-164">pinMaximumLength</span></span>|<span data-ttu-id="a9fea-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fea-165">Int32</span></span>|<span data-ttu-id="a9fea-166">控制 Windows Hello 企业 PIN 允许的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="a9fea-166">Controls the maximum number of characters allowed for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a9fea-167">此值必须介于 4 和 127 之间（包含两者）。</span><span class="sxs-lookup"><span data-stu-id="a9fea-167">This value must be between 4 and 127, inclusive.</span></span> <span data-ttu-id="a9fea-168">此值必须大于或等于为最小 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="a9fea-168">This value must be greater than or equal to the value set for the minimum PIN.</span></span>|
|<span data-ttu-id="a9fea-169">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a9fea-169">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a9fea-170">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a9fea-170">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a9fea-171">控制在 Windows Hello 企业 PIN 中使用大写字母的能力。</span><span class="sxs-lookup"><span data-stu-id="a9fea-171">Controls the ability to use uppercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a9fea-172">Allowed 允许使用大写字母 (大写) ，而 Required 可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="a9fea-172">Allowed permits the use of uppercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="a9fea-173">如果设置为"不允许"，则不允许使用大写字母。</span><span class="sxs-lookup"><span data-stu-id="a9fea-173">If set to Not Allowed, uppercase letters will not be permitted.</span></span> <span data-ttu-id="a9fea-174">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="a9fea-174">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a9fea-175">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a9fea-175">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a9fea-176">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a9fea-176">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a9fea-177">控制在 Windows Hello 企业 PIN 中使用小写字母的能力。</span><span class="sxs-lookup"><span data-stu-id="a9fea-177">Controls the ability to use lowercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a9fea-178">Allowed 允许使用小写字母 () ，而 Required 可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="a9fea-178">Allowed permits the use of lowercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="a9fea-179">如果设置为"不允许"，则不允许使用小写字母。</span><span class="sxs-lookup"><span data-stu-id="a9fea-179">If set to Not Allowed, lowercase letters will not be permitted.</span></span> <span data-ttu-id="a9fea-180">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="a9fea-180">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a9fea-181">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a9fea-181">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a9fea-182">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a9fea-182">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a9fea-183">控制在 Windows Hello 企业 PIN 中使用特殊字符的能力。</span><span class="sxs-lookup"><span data-stu-id="a9fea-183">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a9fea-184">允许允许使用特殊字符 (字符) ，而 Required 可确保它们存在。</span><span class="sxs-lookup"><span data-stu-id="a9fea-184">Allowed permits the use of special character(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="a9fea-185">如果设置为"不允许"， (不允许) 特殊字符。</span><span class="sxs-lookup"><span data-stu-id="a9fea-185">If set to Not Allowed, special character(s) will not be permitted.</span></span> <span data-ttu-id="a9fea-186">可取值为：`allowed`、`required`、`disallowed`。</span><span class="sxs-lookup"><span data-stu-id="a9fea-186">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a9fea-187">state</span><span class="sxs-lookup"><span data-stu-id="a9fea-187">state</span></span>|[<span data-ttu-id="a9fea-188">enablement</span><span class="sxs-lookup"><span data-stu-id="a9fea-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a9fea-189">控制是否允许为 Windows Hello 企业版本配置设备。</span><span class="sxs-lookup"><span data-stu-id="a9fea-189">Controls whether to allow the device to be configured for Windows Hello for Business.</span></span> <span data-ttu-id="a9fea-190">如果设置为禁用，则用户无法预配 Windows Hello 企业版，除非在加入 Azure Active Directory 的移动电话上（如果需要）。</span><span class="sxs-lookup"><span data-stu-id="a9fea-190">If set to disabled, the user cannot provision Windows Hello for Business except on Azure Active Directory joined mobile phones if otherwise required.</span></span> <span data-ttu-id="a9fea-191">如果设置为"未配置"，Intune 将不会覆盖客户端默认值。</span><span class="sxs-lookup"><span data-stu-id="a9fea-191">If set to Not Configured, Intune will not override client defaults.</span></span> <span data-ttu-id="a9fea-192">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a9fea-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a9fea-193">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a9fea-193">securityDeviceRequired</span></span>|<span data-ttu-id="a9fea-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9fea-194">Boolean</span></span>|<span data-ttu-id="a9fea-195">控制是否需要受信任的平台模块 (TPM) 预配 Windows Hello 企业版本。</span><span class="sxs-lookup"><span data-stu-id="a9fea-195">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="a9fea-196">TPM 提供了额外的安全优势，因为存储在 TPM 上的数据不能用于其他设备。</span><span class="sxs-lookup"><span data-stu-id="a9fea-196">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="a9fea-197">如果设置为 False，则所有设备都可以预配 Windows Hello 企业版本，即使没有可用 TPM。</span><span class="sxs-lookup"><span data-stu-id="a9fea-197">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="a9fea-198">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a9fea-198">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a9fea-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9fea-199">Boolean</span></span>|<span data-ttu-id="a9fea-200">控制将生物识别手势（如人脸和指纹）用作 Windows Hello 企业 PIN 的替代方法。</span><span class="sxs-lookup"><span data-stu-id="a9fea-200">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a9fea-201">如果设置为 False，则不允许生物识别手势。</span><span class="sxs-lookup"><span data-stu-id="a9fea-201">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="a9fea-202">用户仍必须将 PIN 配置为备份，以防发生故障。</span><span class="sxs-lookup"><span data-stu-id="a9fea-202">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="a9fea-203">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="a9fea-203">remotePassportEnabled</span></span>|<span data-ttu-id="a9fea-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9fea-204">Boolean</span></span>|<span data-ttu-id="a9fea-205">控制远程 Windows Hello 企业计划的使用。</span><span class="sxs-lookup"><span data-stu-id="a9fea-205">Controls the use of Remote Windows Hello for Business.</span></span> <span data-ttu-id="a9fea-206">远程 Windows Hello 企业版提供可移植的已注册设备用作桌面身份验证配套设备的能力。</span><span class="sxs-lookup"><span data-stu-id="a9fea-206">Remote Windows Hello for Business provides the ability for a portable, registered device to be usable as a companion for desktop authentication.</span></span> <span data-ttu-id="a9fea-207">桌面必须加入 Azure AD，配套设备必须具有 Windows Hello 企业版 PIN。</span><span class="sxs-lookup"><span data-stu-id="a9fea-207">The desktop must be Azure AD joined and the companion device must have a Windows Hello for Business PIN.</span></span>|
|<span data-ttu-id="a9fea-208">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a9fea-208">pinPreviousBlockCount</span></span>|<span data-ttu-id="a9fea-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fea-209">Int32</span></span>|<span data-ttu-id="a9fea-210">控制阻止用户使用过去 PIN 的能力。</span><span class="sxs-lookup"><span data-stu-id="a9fea-210">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="a9fea-211">必须将其设置为 0 到 50（含 0 和 50）之间，并且用户的当前 PIN 包含在该计数中。</span><span class="sxs-lookup"><span data-stu-id="a9fea-211">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="a9fea-212">如果设置为 0，则不存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="a9fea-212">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="a9fea-213">PIN 历史记录不会通过 PIN 重置保留。</span><span class="sxs-lookup"><span data-stu-id="a9fea-213">PIN history is not preserved through a PIN reset.</span></span>|
|<span data-ttu-id="a9fea-214">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a9fea-214">pinExpirationInDays</span></span>|<span data-ttu-id="a9fea-215">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fea-215">Int32</span></span>|<span data-ttu-id="a9fea-216">控制在系统 (PIN 之前) PIN 的时间段（以天表示）。</span><span class="sxs-lookup"><span data-stu-id="a9fea-216">Controls the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="a9fea-217">这必须设置为 0 到 730 之间（包含这两者）。</span><span class="sxs-lookup"><span data-stu-id="a9fea-217">This must be set between 0 and 730, inclusive.</span></span> <span data-ttu-id="a9fea-218">如果设置为 0，则用户的 PIN 永不过期</span><span class="sxs-lookup"><span data-stu-id="a9fea-218">If set to 0, the user's PIN will never expire</span></span>|
|<span data-ttu-id="a9fea-219">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="a9fea-219">enhancedBiometricsState</span></span>|[<span data-ttu-id="a9fea-220">enablement</span><span class="sxs-lookup"><span data-stu-id="a9fea-220">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a9fea-221">控制在支持防欺骗功能的设备上使用反欺骗功能进行面部识别的能力。</span><span class="sxs-lookup"><span data-stu-id="a9fea-221">Controls the ability to use the anti-spoofing features for facial recognition on devices which support it.</span></span> <span data-ttu-id="a9fea-222">如果设置为禁用，则不允许使用反欺骗功能。</span><span class="sxs-lookup"><span data-stu-id="a9fea-222">If set to disabled, anti-spoofing features are not allowed.</span></span> <span data-ttu-id="a9fea-223">如果设置为"未配置"，用户可以选择是否要使用反欺骗。</span><span class="sxs-lookup"><span data-stu-id="a9fea-223">If set to Not Configured, the user can choose whether they want to use anti-spoofing.</span></span> <span data-ttu-id="a9fea-224">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a9fea-224">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a9fea-225">securityKeyForSignIn</span><span class="sxs-lookup"><span data-stu-id="a9fea-225">securityKeyForSignIn</span></span>|[<span data-ttu-id="a9fea-226">enablement</span><span class="sxs-lookup"><span data-stu-id="a9fea-226">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a9fea-227">登录安全密钥提供远程打开/关闭 Windows Hello 递归键未配置的容量将采用在 clinet 上完成的配置。</span><span class="sxs-lookup"><span data-stu-id="a9fea-227">Security key for Sign In provides the capacity for remotely turning ON/OFF Windows Hello Sercurity Keyl Not configured will honor configurations done on the clinet.</span></span> <span data-ttu-id="a9fea-228">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a9fea-228">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a9fea-229">响应</span><span class="sxs-lookup"><span data-stu-id="a9fea-229">Response</span></span>
<span data-ttu-id="a9fea-230">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9fea-230">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9fea-231">示例</span><span class="sxs-lookup"><span data-stu-id="a9fea-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9fea-232">请求</span><span class="sxs-lookup"><span data-stu-id="a9fea-232">Request</span></span>
<span data-ttu-id="a9fea-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9fea-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 729

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="a9fea-234">响应</span><span class="sxs-lookup"><span data-stu-id="a9fea-234">Response</span></span>
<span data-ttu-id="a9fea-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9fea-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




