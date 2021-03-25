---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 12598e21e0842ad95ea053a9a9b93e4914c0f315
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155272"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="dd8a6-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd8a6-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="dd8a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd8a6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd8a6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd8a6-107">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd8a6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd8a6-108">Prerequisites</span></span>
<span data-ttu-id="dd8a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd8a6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd8a6-111">Permission type</span></span>|<span data-ttu-id="dd8a6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd8a6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd8a6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd8a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd8a6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd8a6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd8a6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd8a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd8a6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-116">Not supported.</span></span>|
|<span data-ttu-id="dd8a6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd8a6-117">Application</span></span>|<span data-ttu-id="dd8a6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd8a6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd8a6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd8a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dd8a6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd8a6-120">Request headers</span></span>
|<span data-ttu-id="dd8a6-121">标头</span><span class="sxs-lookup"><span data-stu-id="dd8a6-121">Header</span></span>|<span data-ttu-id="dd8a6-122">值</span><span class="sxs-lookup"><span data-stu-id="dd8a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd8a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd8a6-123">Authorization</span></span>|<span data-ttu-id="dd8a6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd8a6-125">接受</span><span class="sxs-lookup"><span data-stu-id="dd8a6-125">Accept</span></span>|<span data-ttu-id="dd8a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd8a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd8a6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd8a6-127">Request body</span></span>
<span data-ttu-id="dd8a6-128">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="dd8a6-129">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="dd8a6-130">属性</span><span class="sxs-lookup"><span data-stu-id="dd8a6-130">Property</span></span>|<span data-ttu-id="dd8a6-131">类型</span><span class="sxs-lookup"><span data-stu-id="dd8a6-131">Type</span></span>|<span data-ttu-id="dd8a6-132">说明</span><span class="sxs-lookup"><span data-stu-id="dd8a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd8a6-133">id</span><span class="sxs-lookup"><span data-stu-id="dd8a6-133">id</span></span>|<span data-ttu-id="dd8a6-134">String</span><span class="sxs-lookup"><span data-stu-id="dd8a6-134">String</span></span>|<span data-ttu-id="dd8a6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-135">Key of the entity.</span></span> <span data-ttu-id="dd8a6-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd8a6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dd8a6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd8a6-138">DateTimeOffset</span></span>|<span data-ttu-id="dd8a6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dd8a6-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd8a6-141">roleScopeTagIds</span></span>|<span data-ttu-id="dd8a6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="dd8a6-142">String collection</span></span>|<span data-ttu-id="dd8a6-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd8a6-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dd8a6-145">supportsScopeTags</span></span>|<span data-ttu-id="dd8a6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-146">Boolean</span></span>|<span data-ttu-id="dd8a6-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dd8a6-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dd8a6-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dd8a6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-150">This property is read-only.</span></span> <span data-ttu-id="dd8a6-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dd8a6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dd8a6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dd8a6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dd8a6-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dd8a6-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dd8a6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dd8a6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dd8a6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dd8a6-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dd8a6-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dd8a6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dd8a6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dd8a6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dd8a6-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dd8a6-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd8a6-164">createdDateTime</span></span>|<span data-ttu-id="dd8a6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd8a6-165">DateTimeOffset</span></span>|<span data-ttu-id="dd8a6-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-166">DateTime the object was created.</span></span> <span data-ttu-id="dd8a6-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-168">说明</span><span class="sxs-lookup"><span data-stu-id="dd8a6-168">description</span></span>|<span data-ttu-id="dd8a6-169">String</span><span class="sxs-lookup"><span data-stu-id="dd8a6-169">String</span></span>|<span data-ttu-id="dd8a6-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd8a6-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="dd8a6-172">displayName</span></span>|<span data-ttu-id="dd8a6-173">String</span><span class="sxs-lookup"><span data-stu-id="dd8a6-173">String</span></span>|<span data-ttu-id="dd8a6-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd8a6-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-176">version</span><span class="sxs-lookup"><span data-stu-id="dd8a6-176">version</span></span>|<span data-ttu-id="dd8a6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-177">Int32</span></span>|<span data-ttu-id="dd8a6-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-178">Version of the device configuration.</span></span> <span data-ttu-id="dd8a6-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd8a6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd8a6-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="dd8a6-180">compliantAppsList</span></span>|<span data-ttu-id="dd8a6-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd8a6-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dd8a6-182">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="dd8a6-183">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dd8a6-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="dd8a6-184">compliantAppListType</span></span>|[<span data-ttu-id="dd8a6-185">appListType</span><span class="sxs-lookup"><span data-stu-id="dd8a6-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="dd8a6-186">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="dd8a6-187">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="dd8a6-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="dd8a6-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="dd8a6-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd8a6-189">String collection</span></span>|<span data-ttu-id="dd8a6-190">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="dd8a6-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dd8a6-191">passwordBlockSimple</span></span>|<span data-ttu-id="dd8a6-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-192">Boolean</span></span>|<span data-ttu-id="dd8a6-193">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-193">Block simple passwords.</span></span>|
|<span data-ttu-id="dd8a6-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dd8a6-194">passwordExpirationDays</span></span>|<span data-ttu-id="dd8a6-195">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-195">Int32</span></span>|<span data-ttu-id="dd8a6-196">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="dd8a6-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dd8a6-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dd8a6-198">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-198">Int32</span></span>|<span data-ttu-id="dd8a6-199">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="dd8a6-200">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="dd8a6-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="dd8a6-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dd8a6-201">passwordMinimumLength</span></span>|<span data-ttu-id="dd8a6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-202">Int32</span></span>|<span data-ttu-id="dd8a6-203">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="dd8a6-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dd8a6-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dd8a6-205">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-205">Int32</span></span>|<span data-ttu-id="dd8a6-206">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="dd8a6-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dd8a6-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dd8a6-208">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-208">Int32</span></span>|<span data-ttu-id="dd8a6-209">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="dd8a6-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dd8a6-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dd8a6-211">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-211">Int32</span></span>|<span data-ttu-id="dd8a6-212">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="dd8a6-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dd8a6-213">passwordRequiredType</span></span>|[<span data-ttu-id="dd8a6-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dd8a6-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dd8a6-215">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-215">Type of password that is required.</span></span> <span data-ttu-id="dd8a6-216">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dd8a6-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dd8a6-217">passwordRequired</span></span>|<span data-ttu-id="dd8a6-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-218">Boolean</span></span>|<span data-ttu-id="dd8a6-219">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="dd8a6-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="dd8a6-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="dd8a6-221">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-221">Int32</span></span>|<span data-ttu-id="dd8a6-222">在设备的锁屏界面上输入密码的允许失败尝试次数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="dd8a6-223">有效值为 2 至 11</span><span class="sxs-lookup"><span data-stu-id="dd8a6-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="dd8a6-224">passwordMinutesUntilFailedLoginReset</span><span class="sxs-lookup"><span data-stu-id="dd8a6-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="dd8a6-225">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-225">Int32</span></span>|<span data-ttu-id="dd8a6-226">达到最大登录尝试失败次数后重置登录前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="dd8a6-227">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="dd8a6-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="dd8a6-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-228">Boolean</span></span>|<span data-ttu-id="dd8a6-229">指示在 macOS 10.12 (是否阻止 iCloud 密钥链) 。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="dd8a6-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="dd8a6-230">airPrintBlocked</span></span>|<span data-ttu-id="dd8a6-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-231">Boolean</span></span>|<span data-ttu-id="dd8a6-232">指示在 macOS 10.12 (是否阻止 AirPrint) 。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="dd8a6-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="dd8a6-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="dd8a6-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-234">Boolean</span></span>|<span data-ttu-id="dd8a6-235">指示在 macOS 10.13 及更高版本中，TLS 打印通信 (所需的受信任证书) 。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="dd8a6-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="dd8a6-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="dd8a6-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-237">Boolean</span></span>|<span data-ttu-id="dd8a6-238">指示是否阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="dd8a6-239">这可以防止恶意的 AirPrint Bluetooth信号对 macOS 10.3 (及更高版本的网络通信进行网络钓鱼) 。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="dd8a6-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="dd8a6-240">safariBlockAutofill</span></span>|<span data-ttu-id="dd8a6-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-241">Boolean</span></span>|<span data-ttu-id="dd8a6-242">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="dd8a6-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="dd8a6-243">cameraBlocked</span></span>|<span data-ttu-id="dd8a6-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-244">Boolean</span></span>|<span data-ttu-id="dd8a6-245">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="dd8a6-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="dd8a6-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="dd8a6-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-247">Boolean</span></span>|<span data-ttu-id="dd8a6-248">指示是否阻止应用音乐应用音乐经典模式。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="dd8a6-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="dd8a6-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="dd8a6-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-250">Boolean</span></span>|<span data-ttu-id="dd8a6-251">指示是否阻止聚焦从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="dd8a6-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="dd8a6-252">keyboardBlockDictation</span></span>|<span data-ttu-id="dd8a6-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-253">Boolean</span></span>|<span data-ttu-id="dd8a6-254">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="dd8a6-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="dd8a6-255">definitionLookupBlocked</span></span>|<span data-ttu-id="dd8a6-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-256">Boolean</span></span>|<span data-ttu-id="dd8a6-257">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="dd8a6-258">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="dd8a6-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="dd8a6-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-259">Boolean</span></span>|<span data-ttu-id="dd8a6-260">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="dd8a6-261">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="dd8a6-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="dd8a6-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-262">Boolean</span></span>|<span data-ttu-id="dd8a6-263">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="dd8a6-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="dd8a6-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="dd8a6-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-265">Boolean</span></span>|<span data-ttu-id="dd8a6-266">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="dd8a6-267">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="dd8a6-267">iCloudBlockMail</span></span>|<span data-ttu-id="dd8a6-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-268">Boolean</span></span>|<span data-ttu-id="dd8a6-269">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="dd8a6-270">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="dd8a6-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="dd8a6-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-271">Boolean</span></span>|<span data-ttu-id="dd8a6-272">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="dd8a6-273">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="dd8a6-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="dd8a6-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-274">Boolean</span></span>|<span data-ttu-id="dd8a6-275">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="dd8a6-276">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="dd8a6-276">iCloudBlockReminders</span></span>|<span data-ttu-id="dd8a6-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-277">Boolean</span></span>|<span data-ttu-id="dd8a6-278">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="dd8a6-279">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="dd8a6-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="dd8a6-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-280">Boolean</span></span>|<span data-ttu-id="dd8a6-281">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="dd8a6-282">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="dd8a6-282">iCloudBlockNotes</span></span>|<span data-ttu-id="dd8a6-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-283">Boolean</span></span>|<span data-ttu-id="dd8a6-284">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="dd8a6-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="dd8a6-285">airDropBlocked</span></span>|<span data-ttu-id="dd8a6-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-286">Boolean</span></span>|<span data-ttu-id="dd8a6-287">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="dd8a6-288">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="dd8a6-288">passwordBlockModification</span></span>|<span data-ttu-id="dd8a6-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-289">Boolean</span></span>|<span data-ttu-id="dd8a6-290">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="dd8a6-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="dd8a6-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="dd8a6-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-292">Boolean</span></span>|<span data-ttu-id="dd8a6-293">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="dd8a6-294">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="dd8a6-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="dd8a6-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-295">Boolean</span></span>|<span data-ttu-id="dd8a6-296">指示是否阻止"自动填充密码"功能。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="dd8a6-297">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="dd8a6-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="dd8a6-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-298">Boolean</span></span>|<span data-ttu-id="dd8a6-299">指示是否阻止从附近设备请求密码。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="dd8a6-300">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="dd8a6-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="dd8a6-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-301">Boolean</span></span>|<span data-ttu-id="dd8a6-302">指示是否阻止与 AirDrop 密码功能共享密码。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="dd8a6-303">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="dd8a6-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="dd8a6-304">Int32</span><span class="sxs-lookup"><span data-stu-id="dd8a6-304">Int32</span></span>|<span data-ttu-id="dd8a6-305">设置对受监督设备取消软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="dd8a6-306">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="dd8a6-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="dd8a6-307">updateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="dd8a6-307">updateDelayPolicy</span></span>|[<span data-ttu-id="dd8a6-308">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="dd8a6-308">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="dd8a6-309">确定是否延迟 macOS 的操作系统和/或应用更新。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-309">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="dd8a6-310">可取值为：`none`、`delayOSUpdateVisibility`、`delayAppUpdateVisibility`。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-310">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="dd8a6-311">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="dd8a6-311">contentCachingBlocked</span></span>|<span data-ttu-id="dd8a6-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-312">Boolean</span></span>|<span data-ttu-id="dd8a6-313">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-313">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="dd8a6-314">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="dd8a6-314">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="dd8a6-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-315">Boolean</span></span>|<span data-ttu-id="dd8a6-316">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-316">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="dd8a6-317">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="dd8a6-317">screenCaptureBlocked</span></span>|<span data-ttu-id="dd8a6-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-318">Boolean</span></span>|<span data-ttu-id="dd8a6-319">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-319">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="dd8a6-320">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="dd8a6-320">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="dd8a6-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-321">Boolean</span></span>|<span data-ttu-id="dd8a6-322">指示是否允许 Classroom 应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-322">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="dd8a6-323">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="dd8a6-324">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="dd8a6-324">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="dd8a6-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-325">Boolean</span></span>|<span data-ttu-id="dd8a6-326">指示是否自动授予课堂应用上托管课程的教师查看学生屏幕的权限，而不提示。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-326">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="dd8a6-327">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="dd8a6-328">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="dd8a6-328">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="dd8a6-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-329">Boolean</span></span>|<span data-ttu-id="dd8a6-330">指示是否自动授予对教师请求的权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-330">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="dd8a6-331">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="dd8a6-332">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="dd8a6-332">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="dd8a6-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-333">Boolean</span></span>|<span data-ttu-id="dd8a6-334">指示在尝试离开课程时，是否要求通过 Classroom 在非托管课程注册的学生向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-334">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="dd8a6-335">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="dd8a6-336">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="dd8a6-336">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="dd8a6-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-337">Boolean</span></span>|<span data-ttu-id="dd8a6-338">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-338">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="dd8a6-339">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-339">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="dd8a6-340">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="dd8a6-340">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="dd8a6-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8a6-341">Boolean</span></span>|<span data-ttu-id="dd8a6-342">指示是否阻止用户在 MacOS 10.15 或更高版本上其他 iOS 或 MacOS (MacOS 设备上启动的工作) 。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-342">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="dd8a6-343">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="dd8a6-343">privacyAccessControls</span></span>|<span data-ttu-id="dd8a6-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd8a6-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="dd8a6-345">隐私首选项策略控件的列表。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-345">List of privacy preference policy controls.</span></span> <span data-ttu-id="dd8a6-346">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-346">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="dd8a6-347">响应</span><span class="sxs-lookup"><span data-stu-id="dd8a6-347">Response</span></span>
<span data-ttu-id="dd8a6-348">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-348">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd8a6-349">示例</span><span class="sxs-lookup"><span data-stu-id="dd8a6-349">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd8a6-350">请求</span><span class="sxs-lookup"><span data-stu-id="dd8a6-350">Request</span></span>
<span data-ttu-id="dd8a6-351">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-351">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4640

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dd8a6-352">响应</span><span class="sxs-lookup"><span data-stu-id="dd8a6-352">Response</span></span>
<span data-ttu-id="dd8a6-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd8a6-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4812

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```




