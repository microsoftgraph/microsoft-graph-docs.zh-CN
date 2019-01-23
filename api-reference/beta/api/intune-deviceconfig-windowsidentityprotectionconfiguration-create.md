---
title: 创建 windowsIdentityProtectionConfiguration
description: 创建新的 windowsIdentityProtectionConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be9c6ad30eb869bfd47b20863fc41e103eabe1c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408990"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="9a63b-103">创建 windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a63b-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="9a63b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9a63b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a63b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9a63b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a63b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a63b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a63b-107">创建新的[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a63b-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a63b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a63b-108">Prerequisites</span></span>
<span data-ttu-id="9a63b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9a63b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a63b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a63b-111">Permission type</span></span>|<span data-ttu-id="9a63b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a63b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a63b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a63b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a63b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a63b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a63b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a63b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a63b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a63b-116">Not supported.</span></span>|
|<span data-ttu-id="9a63b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a63b-117">Application</span></span>|<span data-ttu-id="9a63b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a63b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a63b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a63b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9a63b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a63b-120">Request headers</span></span>
|<span data-ttu-id="9a63b-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a63b-121">Header</span></span>|<span data-ttu-id="9a63b-122">值</span><span class="sxs-lookup"><span data-stu-id="9a63b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a63b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a63b-123">Authorization</span></span>|<span data-ttu-id="9a63b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a63b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a63b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a63b-125">Accept</span></span>|<span data-ttu-id="9a63b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a63b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a63b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a63b-127">Request body</span></span>
<span data-ttu-id="9a63b-128">在请求正文中，提供 windowsIdentityProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a63b-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="9a63b-129">下表显示时创建 windowsIdentityProtectionConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a63b-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="9a63b-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a63b-130">Property</span></span>|<span data-ttu-id="9a63b-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a63b-131">Type</span></span>|<span data-ttu-id="9a63b-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a63b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a63b-133">id</span><span class="sxs-lookup"><span data-stu-id="9a63b-133">id</span></span>|<span data-ttu-id="9a63b-134">String</span><span class="sxs-lookup"><span data-stu-id="9a63b-134">String</span></span>|<span data-ttu-id="9a63b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9a63b-135">Key of the entity.</span></span> <span data-ttu-id="9a63b-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a63b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9a63b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a63b-138">DateTimeOffset</span></span>|<span data-ttu-id="9a63b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a63b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9a63b-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a63b-141">roleScopeTagIds</span></span>|<span data-ttu-id="9a63b-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9a63b-142">String collection</span></span>|<span data-ttu-id="9a63b-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="9a63b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a63b-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9a63b-145">supportsScopeTags</span></span>|<span data-ttu-id="9a63b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-146">Boolean</span></span>|<span data-ttu-id="9a63b-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="9a63b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9a63b-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="9a63b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9a63b-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="9a63b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9a63b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9a63b-150">This property is read-only.</span></span> <span data-ttu-id="9a63b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a63b-152">createdDateTime</span></span>|<span data-ttu-id="9a63b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a63b-153">DateTimeOffset</span></span>|<span data-ttu-id="9a63b-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a63b-154">DateTime the object was created.</span></span> <span data-ttu-id="9a63b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-156">description</span><span class="sxs-lookup"><span data-stu-id="9a63b-156">description</span></span>|<span data-ttu-id="9a63b-157">String</span><span class="sxs-lookup"><span data-stu-id="9a63b-157">String</span></span>|<span data-ttu-id="9a63b-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9a63b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a63b-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9a63b-160">displayName</span></span>|<span data-ttu-id="9a63b-161">String</span><span class="sxs-lookup"><span data-stu-id="9a63b-161">String</span></span>|<span data-ttu-id="9a63b-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9a63b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a63b-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-164">version</span><span class="sxs-lookup"><span data-stu-id="9a63b-164">version</span></span>|<span data-ttu-id="9a63b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9a63b-165">Int32</span></span>|<span data-ttu-id="9a63b-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9a63b-166">Version of the device configuration.</span></span> <span data-ttu-id="9a63b-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a63b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a63b-168">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="9a63b-168">useSecurityKeyForSignin</span></span>|<span data-ttu-id="9a63b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-169">Boolean</span></span>|<span data-ttu-id="9a63b-170">用于启用 Windows Hello 安全密钥作为登录凭据的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-170">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="9a63b-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="9a63b-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="9a63b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-172">Boolean</span></span>|<span data-ttu-id="9a63b-173">用于启用增强反欺骗 Windows Hello 图符身份验证的面部功能识别的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-173">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="9a63b-174">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9a63b-174">pinMinimumLength</span></span>|<span data-ttu-id="9a63b-175">Int32</span><span class="sxs-lookup"><span data-stu-id="9a63b-175">Int32</span></span>|<span data-ttu-id="9a63b-176">设置的最小所需的 Windows Hello 业务 PIN 的字符数的整数值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-176">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9a63b-177">有效值为 4 到 127 之间，因此小于或等于的值的最大 PIN 设置。</span><span class="sxs-lookup"><span data-stu-id="9a63b-177">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="9a63b-178">有效值 4 到 127</span><span class="sxs-lookup"><span data-stu-id="9a63b-178">Valid values 4 to 127</span></span>|
|<span data-ttu-id="9a63b-179">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="9a63b-179">pinMaximumLength</span></span>|<span data-ttu-id="9a63b-180">Int32</span><span class="sxs-lookup"><span data-stu-id="9a63b-180">Int32</span></span>|<span data-ttu-id="9a63b-181">设置的最大允许工作 PIN 的字符数的整数值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-181">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="9a63b-182">有效值为 4 到 127 非独占且大于或等于最小 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-182">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="9a63b-183">有效值 4 到 127</span><span class="sxs-lookup"><span data-stu-id="9a63b-183">Valid values 4 to 127</span></span>|
|<span data-ttu-id="9a63b-184">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9a63b-184">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="9a63b-185">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9a63b-185">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9a63b-186">此值将使用大写字符中 Windows Hello 配置的业务 PIN。</span><span class="sxs-lookup"><span data-stu-id="9a63b-186">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9a63b-187">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="9a63b-187">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="9a63b-188">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9a63b-188">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="9a63b-189">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9a63b-189">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9a63b-190">此值为业务 PIN 在 Windows Hello 配置使用小写字符。</span><span class="sxs-lookup"><span data-stu-id="9a63b-190">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9a63b-191">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="9a63b-191">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="9a63b-192">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9a63b-192">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="9a63b-193">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9a63b-193">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9a63b-194">控制能否使用特殊字符中 Windows Hello 业务 PIN。</span><span class="sxs-lookup"><span data-stu-id="9a63b-194">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9a63b-195">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="9a63b-195">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="9a63b-196">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="9a63b-196">pinExpirationInDays</span></span>|<span data-ttu-id="9a63b-197">Int32</span><span class="sxs-lookup"><span data-stu-id="9a63b-197">Int32</span></span>|<span data-ttu-id="9a63b-198">整数值，指定的时间段 （以天为单位） 的系统要求用户更改其之前，可以使用 PIN。</span><span class="sxs-lookup"><span data-stu-id="9a63b-198">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="9a63b-199">有效值为 0 到 730 之间。</span><span class="sxs-lookup"><span data-stu-id="9a63b-199">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="9a63b-200">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="9a63b-200">Valid values 0 to 730</span></span>|
|<span data-ttu-id="9a63b-201">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="9a63b-201">pinPreviousBlockCount</span></span>|<span data-ttu-id="9a63b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9a63b-202">Int32</span></span>|<span data-ttu-id="9a63b-203">控制能否阻止用户使用过旋转中心点。</span><span class="sxs-lookup"><span data-stu-id="9a63b-203">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="9a63b-204">这必须介于 0 到 50，含之间设置和用户的当前 PIN，包含在该计数。</span><span class="sxs-lookup"><span data-stu-id="9a63b-204">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="9a63b-205">如果设置为 0，以前 Pin 不会存储。</span><span class="sxs-lookup"><span data-stu-id="9a63b-205">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="9a63b-206">PIN 历史记录不保留通过 PIN 重置。</span><span class="sxs-lookup"><span data-stu-id="9a63b-206">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="9a63b-207">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="9a63b-207">Valid values 0 to 50</span></span>|
|<span data-ttu-id="9a63b-208">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="9a63b-208">pinRecoveryEnabled</span></span>|<span data-ttu-id="9a63b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-209">Boolean</span></span>|<span data-ttu-id="9a63b-210">布尔值，使用户能够通过使用 Windows Hello 业务 PIN 恢复服务更改其 PIN。</span><span class="sxs-lookup"><span data-stu-id="9a63b-210">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="9a63b-211">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="9a63b-211">securityDeviceRequired</span></span>|<span data-ttu-id="9a63b-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-212">Boolean</span></span>|<span data-ttu-id="9a63b-213">控制是否用于设置 Windows Hello 的业务要求受信任平台模块 (TPM)。</span><span class="sxs-lookup"><span data-stu-id="9a63b-213">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="9a63b-214">TPM 提供其他安全的优势，不能在其他设备上使用存储在其上的数据。</span><span class="sxs-lookup"><span data-stu-id="9a63b-214">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="9a63b-215">如果设置为 False，所有设备可以都设置 Windows Hello for Business 即使没有可用 TPM。</span><span class="sxs-lookup"><span data-stu-id="9a63b-215">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="9a63b-216">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="9a63b-216">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="9a63b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-217">Boolean</span></span>|<span data-ttu-id="9a63b-218">控制生物手势，如图符和指纹，用作的替代方法 Windows Hello 的业务 PIN。</span><span class="sxs-lookup"><span data-stu-id="9a63b-218">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="9a63b-219">如果不允许设置为 False，生物手势。</span><span class="sxs-lookup"><span data-stu-id="9a63b-219">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="9a63b-220">用户仍必须作为出现故障时备份配置 PIN。</span><span class="sxs-lookup"><span data-stu-id="9a63b-220">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="9a63b-221">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="9a63b-221">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="9a63b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-222">Boolean</span></span>|<span data-ttu-id="9a63b-223">启用 Windows Hello for Business 使用证书进行身份验证的本地资源的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-223">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="9a63b-224">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="9a63b-224">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="9a63b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a63b-225">Boolean</span></span>|<span data-ttu-id="9a63b-226">阻止 Windows Hello for Business 作为用于登录到 Windows 方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9a63b-226">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="9a63b-227">响应</span><span class="sxs-lookup"><span data-stu-id="9a63b-227">Response</span></span>
<span data-ttu-id="9a63b-228">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a63b-228">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a63b-229">示例</span><span class="sxs-lookup"><span data-stu-id="9a63b-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a63b-230">请求</span><span class="sxs-lookup"><span data-stu-id="9a63b-230">Request</span></span>
<span data-ttu-id="9a63b-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a63b-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="9a63b-232">响应</span><span class="sxs-lookup"><span data-stu-id="9a63b-232">Response</span></span>
<span data-ttu-id="9a63b-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a63b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




