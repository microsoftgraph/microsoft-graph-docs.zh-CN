---
title: 更新 windowsIdentityProtectionConfiguration
description: 更新 windowsIdentityProtectionConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9cfdbcd9a0e7b2bcbd8ccf84002f73dbcf72e1eb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936304"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="82393-103">更新 windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="82393-103">Update windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="82393-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="82393-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82393-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="82393-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82393-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="82393-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82393-107">更新[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82393-107">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82393-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="82393-108">Prerequisites</span></span>
<span data-ttu-id="82393-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="82393-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82393-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="82393-111">Permission type</span></span>|<span data-ttu-id="82393-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82393-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82393-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82393-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82393-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82393-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82393-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82393-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82393-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="82393-116">Not supported.</span></span>|
|<span data-ttu-id="82393-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="82393-117">Application</span></span>|<span data-ttu-id="82393-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="82393-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82393-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82393-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82393-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="82393-120">Request headers</span></span>
|<span data-ttu-id="82393-121">标头</span><span class="sxs-lookup"><span data-stu-id="82393-121">Header</span></span>|<span data-ttu-id="82393-122">值</span><span class="sxs-lookup"><span data-stu-id="82393-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82393-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82393-123">Authorization</span></span>|<span data-ttu-id="82393-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82393-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82393-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82393-125">Accept</span></span>|<span data-ttu-id="82393-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82393-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82393-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="82393-127">Request body</span></span>
<span data-ttu-id="82393-128">在请求正文中，提供[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82393-128">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="82393-129">下表显示时创建[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82393-129">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="82393-130">属性</span><span class="sxs-lookup"><span data-stu-id="82393-130">Property</span></span>|<span data-ttu-id="82393-131">类型</span><span class="sxs-lookup"><span data-stu-id="82393-131">Type</span></span>|<span data-ttu-id="82393-132">说明</span><span class="sxs-lookup"><span data-stu-id="82393-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82393-133">id</span><span class="sxs-lookup"><span data-stu-id="82393-133">id</span></span>|<span data-ttu-id="82393-134">String</span><span class="sxs-lookup"><span data-stu-id="82393-134">String</span></span>|<span data-ttu-id="82393-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="82393-135">Key of the entity.</span></span> <span data-ttu-id="82393-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82393-137">lastModifiedDateTime</span></span>|<span data-ttu-id="82393-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82393-138">DateTimeOffset</span></span>|<span data-ttu-id="82393-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82393-139">DateTime the object was last modified.</span></span> <span data-ttu-id="82393-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82393-141">roleScopeTagIds</span></span>|<span data-ttu-id="82393-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="82393-142">String collection</span></span>|<span data-ttu-id="82393-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="82393-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82393-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="82393-145">supportsScopeTags</span></span>|<span data-ttu-id="82393-146">布尔</span><span class="sxs-lookup"><span data-stu-id="82393-146">Boolean</span></span>|<span data-ttu-id="82393-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="82393-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82393-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="82393-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82393-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="82393-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82393-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="82393-150">This property is read-only.</span></span> <span data-ttu-id="82393-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82393-152">createdDateTime</span></span>|<span data-ttu-id="82393-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82393-153">DateTimeOffset</span></span>|<span data-ttu-id="82393-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82393-154">DateTime the object was created.</span></span> <span data-ttu-id="82393-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-156">description</span><span class="sxs-lookup"><span data-stu-id="82393-156">description</span></span>|<span data-ttu-id="82393-157">String</span><span class="sxs-lookup"><span data-stu-id="82393-157">String</span></span>|<span data-ttu-id="82393-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="82393-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82393-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-160">displayName</span><span class="sxs-lookup"><span data-stu-id="82393-160">displayName</span></span>|<span data-ttu-id="82393-161">String</span><span class="sxs-lookup"><span data-stu-id="82393-161">String</span></span>|<span data-ttu-id="82393-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="82393-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82393-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-164">version</span><span class="sxs-lookup"><span data-stu-id="82393-164">version</span></span>|<span data-ttu-id="82393-165">Int32</span><span class="sxs-lookup"><span data-stu-id="82393-165">Int32</span></span>|<span data-ttu-id="82393-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="82393-166">Version of the device configuration.</span></span> <span data-ttu-id="82393-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82393-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82393-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="82393-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="82393-169">布尔</span><span class="sxs-lookup"><span data-stu-id="82393-169">Boolean</span></span>|<span data-ttu-id="82393-170">用于启用增强反欺骗 Windows Hello 图符身份验证的面部功能识别的布尔值。</span><span class="sxs-lookup"><span data-stu-id="82393-170">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="82393-171">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82393-171">pinMinimumLength</span></span>|<span data-ttu-id="82393-172">Int32</span><span class="sxs-lookup"><span data-stu-id="82393-172">Int32</span></span>|<span data-ttu-id="82393-173">设置的最小所需的 Windows Hello 业务 PIN 的字符数的整数值。</span><span class="sxs-lookup"><span data-stu-id="82393-173">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82393-174">有效值为 4 到 127 之间，因此小于或等于的值的最大 PIN 设置。</span><span class="sxs-lookup"><span data-stu-id="82393-174">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="82393-175">有效值 4 到 127</span><span class="sxs-lookup"><span data-stu-id="82393-175">Valid values 4 to 127</span></span>|
|<span data-ttu-id="82393-176">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="82393-176">pinMaximumLength</span></span>|<span data-ttu-id="82393-177">Int32</span><span class="sxs-lookup"><span data-stu-id="82393-177">Int32</span></span>|<span data-ttu-id="82393-178">设置的最大允许工作 PIN 的字符数的整数值。</span><span class="sxs-lookup"><span data-stu-id="82393-178">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="82393-179">有效值为 4 到 127 非独占且大于或等于最小 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="82393-179">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="82393-180">有效值 4 到 127</span><span class="sxs-lookup"><span data-stu-id="82393-180">Valid values 4 to 127</span></span>|
|<span data-ttu-id="82393-181">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82393-181">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="82393-182">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82393-182">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82393-183">此值将使用大写字符中 Windows Hello 配置的业务 PIN。</span><span class="sxs-lookup"><span data-stu-id="82393-183">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82393-184">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82393-184">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82393-185">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82393-185">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="82393-186">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82393-186">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82393-187">此值为业务 PIN 在 Windows Hello 配置使用小写字符。</span><span class="sxs-lookup"><span data-stu-id="82393-187">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82393-188">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82393-188">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82393-189">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82393-189">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="82393-190">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82393-190">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82393-191">控制能否使用特殊字符中 Windows Hello 业务 PIN。</span><span class="sxs-lookup"><span data-stu-id="82393-191">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="82393-192">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82393-192">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82393-193">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="82393-193">pinExpirationInDays</span></span>|<span data-ttu-id="82393-194">Int32</span><span class="sxs-lookup"><span data-stu-id="82393-194">Int32</span></span>|<span data-ttu-id="82393-195">整数值，指定的时间段 （以天为单位） 的系统要求用户更改其之前，可以使用 PIN。</span><span class="sxs-lookup"><span data-stu-id="82393-195">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="82393-196">有效值为 0 到 730 之间。</span><span class="sxs-lookup"><span data-stu-id="82393-196">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="82393-197">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="82393-197">Valid values 0 to 730</span></span>|
|<span data-ttu-id="82393-198">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="82393-198">pinPreviousBlockCount</span></span>|<span data-ttu-id="82393-199">Int32</span><span class="sxs-lookup"><span data-stu-id="82393-199">Int32</span></span>|<span data-ttu-id="82393-200">控制能否阻止用户使用过旋转中心点。</span><span class="sxs-lookup"><span data-stu-id="82393-200">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="82393-201">这必须介于 0 到 50，含之间设置和用户的当前 PIN，包含在该计数。</span><span class="sxs-lookup"><span data-stu-id="82393-201">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="82393-202">如果设置为 0，以前 Pin 不会存储。</span><span class="sxs-lookup"><span data-stu-id="82393-202">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="82393-203">PIN 历史记录不保留通过 PIN 重置。</span><span class="sxs-lookup"><span data-stu-id="82393-203">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="82393-204">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="82393-204">Valid values 0 to 50</span></span>|
|<span data-ttu-id="82393-205">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="82393-205">pinRecoveryEnabled</span></span>|<span data-ttu-id="82393-206">布尔</span><span class="sxs-lookup"><span data-stu-id="82393-206">Boolean</span></span>|<span data-ttu-id="82393-207">布尔值，使用户能够通过使用 Windows Hello 业务 PIN 恢复服务更改其 PIN。</span><span class="sxs-lookup"><span data-stu-id="82393-207">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="82393-208">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="82393-208">securityDeviceRequired</span></span>|<span data-ttu-id="82393-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="82393-209">Boolean</span></span>|<span data-ttu-id="82393-210">控制是否用于设置 Windows Hello 的业务要求受信任平台模块 (TPM)。</span><span class="sxs-lookup"><span data-stu-id="82393-210">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="82393-211">TPM 提供其他安全的优势，不能在其他设备上使用存储在其上的数据。</span><span class="sxs-lookup"><span data-stu-id="82393-211">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="82393-212">如果设置为 False，所有设备可以都设置 Windows Hello for Business 即使没有可用 TPM。</span><span class="sxs-lookup"><span data-stu-id="82393-212">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="82393-213">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="82393-213">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="82393-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="82393-214">Boolean</span></span>|<span data-ttu-id="82393-215">控制生物手势，如图符和指纹，用作的替代方法 Windows Hello 的业务 PIN。</span><span class="sxs-lookup"><span data-stu-id="82393-215">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="82393-216">如果不允许设置为 False，生物手势。</span><span class="sxs-lookup"><span data-stu-id="82393-216">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="82393-217">用户仍必须作为出现故障时备份配置 PIN。</span><span class="sxs-lookup"><span data-stu-id="82393-217">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="82393-218">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="82393-218">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="82393-219">布尔</span><span class="sxs-lookup"><span data-stu-id="82393-219">Boolean</span></span>|<span data-ttu-id="82393-220">启用 Windows Hello for Business 使用证书进行身份验证的本地资源的布尔值。</span><span class="sxs-lookup"><span data-stu-id="82393-220">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="82393-221">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="82393-221">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="82393-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="82393-222">Boolean</span></span>|<span data-ttu-id="82393-223">阻止 Windows Hello for Business 作为用于登录到 Windows 方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="82393-223">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="82393-224">响应</span><span class="sxs-lookup"><span data-stu-id="82393-224">Response</span></span>
<span data-ttu-id="82393-225">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82393-225">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82393-226">示例</span><span class="sxs-lookup"><span data-stu-id="82393-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="82393-227">请求</span><span class="sxs-lookup"><span data-stu-id="82393-227">Request</span></span>
<span data-ttu-id="82393-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82393-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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

### <a name="response"></a><span data-ttu-id="82393-229">响应</span><span class="sxs-lookup"><span data-stu-id="82393-229">Response</span></span>
<span data-ttu-id="82393-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82393-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 946

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





