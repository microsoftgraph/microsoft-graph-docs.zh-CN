---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0dfe362a28d90ba4216b923f68d8f3f33777d703
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265645"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="526e7-103">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="526e7-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="526e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="526e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="526e7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="526e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="526e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="526e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="526e7-107">创建新的 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="526e7-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="526e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="526e7-108">Prerequisites</span></span>
<span data-ttu-id="526e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="526e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="526e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="526e7-111">Permission type</span></span>|<span data-ttu-id="526e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="526e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="526e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="526e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="526e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="526e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="526e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="526e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="526e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="526e7-116">Not supported.</span></span>|
|<span data-ttu-id="526e7-117">Application</span><span class="sxs-lookup"><span data-stu-id="526e7-117">Application</span></span>|<span data-ttu-id="526e7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="526e7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="526e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="526e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="526e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="526e7-120">Request headers</span></span>
|<span data-ttu-id="526e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="526e7-121">Header</span></span>|<span data-ttu-id="526e7-122">值</span><span class="sxs-lookup"><span data-stu-id="526e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="526e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="526e7-123">Authorization</span></span>|<span data-ttu-id="526e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="526e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="526e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="526e7-125">Accept</span></span>|<span data-ttu-id="526e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="526e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="526e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="526e7-127">Request body</span></span>
<span data-ttu-id="526e7-128">在请求正文中，提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="526e7-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="526e7-129">下表显示创建 androidWorkProfileGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="526e7-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="526e7-130">属性</span><span class="sxs-lookup"><span data-stu-id="526e7-130">Property</span></span>|<span data-ttu-id="526e7-131">类型</span><span class="sxs-lookup"><span data-stu-id="526e7-131">Type</span></span>|<span data-ttu-id="526e7-132">说明</span><span class="sxs-lookup"><span data-stu-id="526e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="526e7-133">id</span><span class="sxs-lookup"><span data-stu-id="526e7-133">id</span></span>|<span data-ttu-id="526e7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="526e7-134">String</span></span>|<span data-ttu-id="526e7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="526e7-135">Key of the entity.</span></span> <span data-ttu-id="526e7-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="526e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="526e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="526e7-138">DateTimeOffset</span></span>|<span data-ttu-id="526e7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="526e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="526e7-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="526e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="526e7-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="526e7-142">String collection</span></span>|<span data-ttu-id="526e7-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="526e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="526e7-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="526e7-145">supportsScopeTags</span></span>|<span data-ttu-id="526e7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-146">Boolean</span></span>|<span data-ttu-id="526e7-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="526e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="526e7-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="526e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="526e7-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="526e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="526e7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="526e7-150">This property is read-only.</span></span> <span data-ttu-id="526e7-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="526e7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="526e7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="526e7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="526e7-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="526e7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="526e7-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="526e7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="526e7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="526e7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="526e7-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="526e7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="526e7-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="526e7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="526e7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="526e7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="526e7-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="526e7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="526e7-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="526e7-164">createdDateTime</span></span>|<span data-ttu-id="526e7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="526e7-165">DateTimeOffset</span></span>|<span data-ttu-id="526e7-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="526e7-166">DateTime the object was created.</span></span> <span data-ttu-id="526e7-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-168">description</span><span class="sxs-lookup"><span data-stu-id="526e7-168">description</span></span>|<span data-ttu-id="526e7-169">字符串</span><span class="sxs-lookup"><span data-stu-id="526e7-169">String</span></span>|<span data-ttu-id="526e7-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="526e7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="526e7-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="526e7-172">displayName</span></span>|<span data-ttu-id="526e7-173">字符串</span><span class="sxs-lookup"><span data-stu-id="526e7-173">String</span></span>|<span data-ttu-id="526e7-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="526e7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="526e7-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-176">version</span><span class="sxs-lookup"><span data-stu-id="526e7-176">version</span></span>|<span data-ttu-id="526e7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-177">Int32</span></span>|<span data-ttu-id="526e7-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="526e7-178">Version of the device configuration.</span></span> <span data-ttu-id="526e7-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="526e7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="526e7-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="526e7-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="526e7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-181">Boolean</span></span>|<span data-ttu-id="526e7-182">指示是否阻止人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="526e7-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="526e7-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="526e7-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="526e7-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-184">Boolean</span></span>|<span data-ttu-id="526e7-185">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="526e7-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="526e7-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="526e7-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="526e7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-187">Boolean</span></span>|<span data-ttu-id="526e7-188">指示是否阻止 iri 解锁。</span><span class="sxs-lookup"><span data-stu-id="526e7-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="526e7-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="526e7-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="526e7-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-190">Boolean</span></span>|<span data-ttu-id="526e7-191">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="526e7-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="526e7-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="526e7-192">passwordExpirationDays</span></span>|<span data-ttu-id="526e7-193">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-193">Int32</span></span>|<span data-ttu-id="526e7-194">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="526e7-194">Number of days before the password expires.</span></span> <span data-ttu-id="526e7-195">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="526e7-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="526e7-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="526e7-196">passwordMinimumLength</span></span>|<span data-ttu-id="526e7-197">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-197">Int32</span></span>|<span data-ttu-id="526e7-198">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="526e7-198">Minimum length of passwords.</span></span> <span data-ttu-id="526e7-199">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="526e7-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="526e7-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="526e7-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="526e7-201">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-201">Int32</span></span>|<span data-ttu-id="526e7-202">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="526e7-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="526e7-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="526e7-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="526e7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-204">Int32</span></span>|<span data-ttu-id="526e7-205">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="526e7-205">Number of previous passwords to block.</span></span> <span data-ttu-id="526e7-206">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="526e7-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="526e7-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="526e7-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="526e7-208">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-208">Int32</span></span>|<span data-ttu-id="526e7-209">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="526e7-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="526e7-210">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="526e7-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="526e7-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="526e7-211">passwordRequiredType</span></span>|[<span data-ttu-id="526e7-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="526e7-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="526e7-213">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="526e7-213">Type of password that is required.</span></span> <span data-ttu-id="526e7-214">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="526e7-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="526e7-215">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="526e7-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="526e7-216">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="526e7-216">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="526e7-217">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="526e7-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="526e7-218">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="526e7-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="526e7-219">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="526e7-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="526e7-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-220">Boolean</span></span>|<span data-ttu-id="526e7-221">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="526e7-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="526e7-222">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="526e7-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="526e7-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-223">Boolean</span></span>|<span data-ttu-id="526e7-224">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="526e7-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="526e7-225">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="526e7-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="526e7-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-226">Boolean</span></span>|<span data-ttu-id="526e7-227">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="526e7-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="526e7-228">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="526e7-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="526e7-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-229">Boolean</span></span>|<span data-ttu-id="526e7-230">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="526e7-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="526e7-231">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="526e7-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="526e7-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-232">Boolean</span></span>|<span data-ttu-id="526e7-233">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="526e7-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="526e7-234">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="526e7-234">workProfileBlockCamera</span></span>|<span data-ttu-id="526e7-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-235">Boolean</span></span>|<span data-ttu-id="526e7-236">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="526e7-236">Block work profile camera.</span></span>|
|<span data-ttu-id="526e7-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="526e7-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="526e7-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-238">Boolean</span></span>|<span data-ttu-id="526e7-239">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="526e7-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="526e7-240">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="526e7-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="526e7-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-241">Boolean</span></span>|<span data-ttu-id="526e7-242">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="526e7-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="526e7-243">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="526e7-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="526e7-244">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="526e7-244">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="526e7-245">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="526e7-245">Type of password that is required.</span></span> <span data-ttu-id="526e7-246">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="526e7-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="526e7-247">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="526e7-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="526e7-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-248">Boolean</span></span>|<span data-ttu-id="526e7-249">指示是否阻止工作配置文件的人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="526e7-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="526e7-250">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="526e7-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="526e7-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-251">Boolean</span></span>|<span data-ttu-id="526e7-252">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="526e7-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="526e7-253">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="526e7-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="526e7-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-254">Boolean</span></span>|<span data-ttu-id="526e7-255">指示是否阻止对工作配置文件的 iri 解除锁定。</span><span class="sxs-lookup"><span data-stu-id="526e7-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="526e7-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="526e7-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="526e7-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-257">Boolean</span></span>|<span data-ttu-id="526e7-258">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="526e7-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="526e7-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="526e7-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="526e7-260">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-260">Int32</span></span>|<span data-ttu-id="526e7-261">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="526e7-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="526e7-262">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="526e7-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="526e7-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="526e7-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="526e7-264">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-264">Int32</span></span>|<span data-ttu-id="526e7-265">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="526e7-265">Minimum length of work profile password.</span></span> <span data-ttu-id="526e7-266">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="526e7-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="526e7-267">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="526e7-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="526e7-268">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-268">Int32</span></span>|<span data-ttu-id="526e7-269">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="526e7-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="526e7-270">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="526e7-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="526e7-271">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="526e7-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="526e7-272">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-272">Int32</span></span>|<span data-ttu-id="526e7-273">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="526e7-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="526e7-274">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="526e7-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="526e7-275">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="526e7-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="526e7-276">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-276">Int32</span></span>|<span data-ttu-id="526e7-277">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="526e7-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="526e7-278">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="526e7-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="526e7-279">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="526e7-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="526e7-280">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-280">Int32</span></span>|<span data-ttu-id="526e7-281">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="526e7-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="526e7-282">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="526e7-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="526e7-283">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="526e7-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="526e7-284">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-284">Int32</span></span>|<span data-ttu-id="526e7-285">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="526e7-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="526e7-286">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="526e7-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="526e7-287">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="526e7-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="526e7-288">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-288">Int32</span></span>|<span data-ttu-id="526e7-289">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="526e7-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="526e7-290">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="526e7-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="526e7-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="526e7-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="526e7-292">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-292">Int32</span></span>|<span data-ttu-id="526e7-293">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="526e7-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="526e7-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="526e7-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="526e7-295">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-295">Int32</span></span>|<span data-ttu-id="526e7-296">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="526e7-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="526e7-297">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="526e7-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="526e7-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="526e7-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="526e7-299">Int32</span><span class="sxs-lookup"><span data-stu-id="526e7-299">Int32</span></span>|<span data-ttu-id="526e7-300">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="526e7-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="526e7-301">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="526e7-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="526e7-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="526e7-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="526e7-303">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="526e7-303">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="526e7-304">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="526e7-304">Type of work profile password that is required.</span></span> <span data-ttu-id="526e7-305">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="526e7-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="526e7-306">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="526e7-306">workProfileRequirePassword</span></span>|<span data-ttu-id="526e7-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-307">Boolean</span></span>|<span data-ttu-id="526e7-308">对于工作配置文件，密码是必需的</span><span class="sxs-lookup"><span data-stu-id="526e7-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="526e7-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="526e7-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="526e7-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-310">Boolean</span></span>|<span data-ttu-id="526e7-311">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="526e7-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="526e7-312">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="526e7-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="526e7-313">字符串</span><span class="sxs-lookup"><span data-stu-id="526e7-313">String</span></span>|<span data-ttu-id="526e7-314">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="526e7-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="526e7-315">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="526e7-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="526e7-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-316">Boolean</span></span>|<span data-ttu-id="526e7-317">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="526e7-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="526e7-318">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="526e7-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="526e7-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-319">Boolean</span></span>|<span data-ttu-id="526e7-320">允许来自工作配置文件应用程序的小部件。</span><span class="sxs-lookup"><span data-stu-id="526e7-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="526e7-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="526e7-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="526e7-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="526e7-322">Boolean</span></span>|<span data-ttu-id="526e7-323">阻止从个人配置文件中的未知源进行应用程序安装。</span><span class="sxs-lookup"><span data-stu-id="526e7-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="526e7-324">响应</span><span class="sxs-lookup"><span data-stu-id="526e7-324">Response</span></span>
<span data-ttu-id="526e7-325">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="526e7-325">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="526e7-326">示例</span><span class="sxs-lookup"><span data-stu-id="526e7-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="526e7-327">请求</span><span class="sxs-lookup"><span data-stu-id="526e7-327">Request</span></span>
<span data-ttu-id="526e7-328">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="526e7-328">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3083

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="526e7-329">响应</span><span class="sxs-lookup"><span data-stu-id="526e7-329">Response</span></span>
<span data-ttu-id="526e7-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="526e7-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3255

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```




