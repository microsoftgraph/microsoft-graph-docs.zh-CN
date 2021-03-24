---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343798542aab40e769b18cf8e4a33993d40af3f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137257"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="c91d8-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c91d8-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="c91d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c91d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c91d8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c91d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c91d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c91d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c91d8-107">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c91d8-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c91d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c91d8-108">Prerequisites</span></span>
<span data-ttu-id="c91d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c91d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c91d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c91d8-111">Permission type</span></span>|<span data-ttu-id="c91d8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c91d8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c91d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c91d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c91d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c91d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c91d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c91d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c91d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c91d8-116">Not supported.</span></span>|
|<span data-ttu-id="c91d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c91d8-117">Application</span></span>|<span data-ttu-id="c91d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c91d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c91d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c91d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c91d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c91d8-120">Request headers</span></span>
|<span data-ttu-id="c91d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="c91d8-121">Header</span></span>|<span data-ttu-id="c91d8-122">值</span><span class="sxs-lookup"><span data-stu-id="c91d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c91d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c91d8-123">Authorization</span></span>|<span data-ttu-id="c91d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c91d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c91d8-125">接受</span><span class="sxs-lookup"><span data-stu-id="c91d8-125">Accept</span></span>|<span data-ttu-id="c91d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c91d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c91d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c91d8-127">Request body</span></span>
<span data-ttu-id="c91d8-128">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c91d8-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c91d8-129">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c91d8-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c91d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="c91d8-130">Property</span></span>|<span data-ttu-id="c91d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="c91d8-131">Type</span></span>|<span data-ttu-id="c91d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="c91d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c91d8-133">id</span><span class="sxs-lookup"><span data-stu-id="c91d8-133">id</span></span>|<span data-ttu-id="c91d8-134">String</span><span class="sxs-lookup"><span data-stu-id="c91d8-134">String</span></span>|<span data-ttu-id="c91d8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c91d8-135">Key of the entity.</span></span> <span data-ttu-id="c91d8-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c91d8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c91d8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91d8-138">DateTimeOffset</span></span>|<span data-ttu-id="c91d8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c91d8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c91d8-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c91d8-141">roleScopeTagIds</span></span>|<span data-ttu-id="c91d8-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c91d8-142">String collection</span></span>|<span data-ttu-id="c91d8-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c91d8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c91d8-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c91d8-145">supportsScopeTags</span></span>|<span data-ttu-id="c91d8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-146">Boolean</span></span>|<span data-ttu-id="c91d8-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c91d8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c91d8-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c91d8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c91d8-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c91d8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c91d8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c91d8-150">This property is read-only.</span></span> <span data-ttu-id="c91d8-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c91d8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c91d8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c91d8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c91d8-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c91d8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c91d8-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c91d8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c91d8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c91d8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c91d8-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c91d8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c91d8-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c91d8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c91d8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c91d8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c91d8-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c91d8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c91d8-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c91d8-164">createdDateTime</span></span>|<span data-ttu-id="c91d8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91d8-165">DateTimeOffset</span></span>|<span data-ttu-id="c91d8-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c91d8-166">DateTime the object was created.</span></span> <span data-ttu-id="c91d8-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-168">说明</span><span class="sxs-lookup"><span data-stu-id="c91d8-168">description</span></span>|<span data-ttu-id="c91d8-169">String</span><span class="sxs-lookup"><span data-stu-id="c91d8-169">String</span></span>|<span data-ttu-id="c91d8-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c91d8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c91d8-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c91d8-172">displayName</span></span>|<span data-ttu-id="c91d8-173">String</span><span class="sxs-lookup"><span data-stu-id="c91d8-173">String</span></span>|<span data-ttu-id="c91d8-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c91d8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c91d8-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-176">version</span><span class="sxs-lookup"><span data-stu-id="c91d8-176">version</span></span>|<span data-ttu-id="c91d8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-177">Int32</span></span>|<span data-ttu-id="c91d8-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c91d8-178">Version of the device configuration.</span></span> <span data-ttu-id="c91d8-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c91d8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c91d8-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c91d8-180">compliantAppsList</span></span>|<span data-ttu-id="c91d8-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c91d8-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c91d8-182">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="c91d8-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c91d8-183">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c91d8-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c91d8-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c91d8-184">compliantAppListType</span></span>|[<span data-ttu-id="c91d8-185">appListType</span><span class="sxs-lookup"><span data-stu-id="c91d8-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c91d8-186">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="c91d8-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="c91d8-187">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="c91d8-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c91d8-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c91d8-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="c91d8-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="c91d8-189">String collection</span></span>|<span data-ttu-id="c91d8-190">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="c91d8-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c91d8-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c91d8-191">passwordBlockSimple</span></span>|<span data-ttu-id="c91d8-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-192">Boolean</span></span>|<span data-ttu-id="c91d8-193">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="c91d8-193">Block simple passwords.</span></span>|
|<span data-ttu-id="c91d8-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c91d8-194">passwordExpirationDays</span></span>|<span data-ttu-id="c91d8-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-195">Int32</span></span>|<span data-ttu-id="c91d8-196">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c91d8-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c91d8-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c91d8-198">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-198">Int32</span></span>|<span data-ttu-id="c91d8-199">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="c91d8-200">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="c91d8-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c91d8-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c91d8-201">passwordMinimumLength</span></span>|<span data-ttu-id="c91d8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-202">Int32</span></span>|<span data-ttu-id="c91d8-203">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c91d8-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c91d8-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c91d8-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c91d8-205">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-205">Int32</span></span>|<span data-ttu-id="c91d8-206">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="c91d8-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c91d8-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c91d8-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-208">Int32</span></span>|<span data-ttu-id="c91d8-209">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="c91d8-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c91d8-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c91d8-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-211">Int32</span></span>|<span data-ttu-id="c91d8-212">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c91d8-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="c91d8-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c91d8-213">passwordRequiredType</span></span>|[<span data-ttu-id="c91d8-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c91d8-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c91d8-215">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c91d8-215">Type of password that is required.</span></span> <span data-ttu-id="c91d8-216">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c91d8-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c91d8-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c91d8-217">passwordRequired</span></span>|<span data-ttu-id="c91d8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-218">Boolean</span></span>|<span data-ttu-id="c91d8-219">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c91d8-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c91d8-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="c91d8-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="c91d8-221">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-221">Int32</span></span>|<span data-ttu-id="c91d8-222">在设备的锁屏界面上输入密码的允许失败尝试次数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="c91d8-223">有效值为 2 至 11</span><span class="sxs-lookup"><span data-stu-id="c91d8-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="c91d8-224">passwordMinutesUntilFailedLoginReset</span><span class="sxs-lookup"><span data-stu-id="c91d8-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="c91d8-225">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-225">Int32</span></span>|<span data-ttu-id="c91d8-226">达到最大登录尝试失败次数后重置登录前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="c91d8-227">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="c91d8-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="c91d8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-228">Boolean</span></span>|<span data-ttu-id="c91d8-229">指示在 macOS 10.12 (是否阻止 iCloud 密钥链) 。</span><span class="sxs-lookup"><span data-stu-id="c91d8-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c91d8-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="c91d8-230">airPrintBlocked</span></span>|<span data-ttu-id="c91d8-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-231">Boolean</span></span>|<span data-ttu-id="c91d8-232">指示在 macOS 10.12 (是否阻止 AirPrint) 。</span><span class="sxs-lookup"><span data-stu-id="c91d8-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c91d8-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="c91d8-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="c91d8-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-234">Boolean</span></span>|<span data-ttu-id="c91d8-235">指示在 macOS 10.13 及更高版本中，TLS 打印通信 (所需的受信任证书) 。</span><span class="sxs-lookup"><span data-stu-id="c91d8-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="c91d8-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="c91d8-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="c91d8-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-237">Boolean</span></span>|<span data-ttu-id="c91d8-238">指示是否阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="c91d8-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="c91d8-239">这可以防止恶意的 AirPrint Bluetooth信号对 macOS 10.3 (及更高版本的网络通信进行网络钓鱼) 。</span><span class="sxs-lookup"><span data-stu-id="c91d8-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="c91d8-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c91d8-240">safariBlockAutofill</span></span>|<span data-ttu-id="c91d8-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-241">Boolean</span></span>|<span data-ttu-id="c91d8-242">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="c91d8-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="c91d8-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c91d8-243">cameraBlocked</span></span>|<span data-ttu-id="c91d8-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-244">Boolean</span></span>|<span data-ttu-id="c91d8-245">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="c91d8-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="c91d8-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="c91d8-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="c91d8-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-247">Boolean</span></span>|<span data-ttu-id="c91d8-248">指示是否阻止应用音乐应用音乐经典模式。</span><span class="sxs-lookup"><span data-stu-id="c91d8-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="c91d8-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="c91d8-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="c91d8-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-250">Boolean</span></span>|<span data-ttu-id="c91d8-251">指示是否阻止聚焦从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="c91d8-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="c91d8-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="c91d8-252">keyboardBlockDictation</span></span>|<span data-ttu-id="c91d8-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-253">Boolean</span></span>|<span data-ttu-id="c91d8-254">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="c91d8-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="c91d8-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="c91d8-255">definitionLookupBlocked</span></span>|<span data-ttu-id="c91d8-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-256">Boolean</span></span>|<span data-ttu-id="c91d8-257">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="c91d8-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="c91d8-258">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="c91d8-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="c91d8-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-259">Boolean</span></span>|<span data-ttu-id="c91d8-260">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="c91d8-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="c91d8-261">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="c91d8-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="c91d8-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-262">Boolean</span></span>|<span data-ttu-id="c91d8-263">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="c91d8-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="c91d8-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="c91d8-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="c91d8-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-265">Boolean</span></span>|<span data-ttu-id="c91d8-266">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="c91d8-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="c91d8-267">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="c91d8-267">iCloudBlockMail</span></span>|<span data-ttu-id="c91d8-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-268">Boolean</span></span>|<span data-ttu-id="c91d8-269">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="c91d8-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="c91d8-270">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="c91d8-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="c91d8-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-271">Boolean</span></span>|<span data-ttu-id="c91d8-272">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="c91d8-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="c91d8-273">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="c91d8-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="c91d8-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-274">Boolean</span></span>|<span data-ttu-id="c91d8-275">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="c91d8-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="c91d8-276">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="c91d8-276">iCloudBlockReminders</span></span>|<span data-ttu-id="c91d8-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-277">Boolean</span></span>|<span data-ttu-id="c91d8-278">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="c91d8-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="c91d8-279">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="c91d8-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="c91d8-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-280">Boolean</span></span>|<span data-ttu-id="c91d8-281">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="c91d8-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="c91d8-282">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="c91d8-282">iCloudBlockNotes</span></span>|<span data-ttu-id="c91d8-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-283">Boolean</span></span>|<span data-ttu-id="c91d8-284">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="c91d8-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="c91d8-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="c91d8-285">airDropBlocked</span></span>|<span data-ttu-id="c91d8-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-286">Boolean</span></span>|<span data-ttu-id="c91d8-287">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="c91d8-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="c91d8-288">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="c91d8-288">passwordBlockModification</span></span>|<span data-ttu-id="c91d8-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-289">Boolean</span></span>|<span data-ttu-id="c91d8-290">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="c91d8-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="c91d8-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c91d8-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c91d8-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-292">Boolean</span></span>|<span data-ttu-id="c91d8-293">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="c91d8-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c91d8-294">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="c91d8-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="c91d8-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-295">Boolean</span></span>|<span data-ttu-id="c91d8-296">指示是否阻止"自动填充密码"功能。</span><span class="sxs-lookup"><span data-stu-id="c91d8-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="c91d8-297">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="c91d8-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="c91d8-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-298">Boolean</span></span>|<span data-ttu-id="c91d8-299">指示是否阻止从附近设备请求密码。</span><span class="sxs-lookup"><span data-stu-id="c91d8-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="c91d8-300">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="c91d8-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="c91d8-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-301">Boolean</span></span>|<span data-ttu-id="c91d8-302">指示是否阻止与 AirDrop 密码功能共享密码。</span><span class="sxs-lookup"><span data-stu-id="c91d8-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="c91d8-303">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="c91d8-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="c91d8-304">Int32</span><span class="sxs-lookup"><span data-stu-id="c91d8-304">Int32</span></span>|<span data-ttu-id="c91d8-305">设置对受监督设备取消软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="c91d8-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="c91d8-306">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="c91d8-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="c91d8-307">updateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="c91d8-307">updateDelayPolicy</span></span>|[<span data-ttu-id="c91d8-308">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="c91d8-308">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="c91d8-309">确定是否延迟 macOS 的操作系统和/或应用更新。</span><span class="sxs-lookup"><span data-stu-id="c91d8-309">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="c91d8-310">可取值为：`none`、`delayOSUpdateVisibility`、`delayAppUpdateVisibility`。</span><span class="sxs-lookup"><span data-stu-id="c91d8-310">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="c91d8-311">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="c91d8-311">contentCachingBlocked</span></span>|<span data-ttu-id="c91d8-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-312">Boolean</span></span>|<span data-ttu-id="c91d8-313">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="c91d8-313">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="c91d8-314">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="c91d8-314">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="c91d8-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-315">Boolean</span></span>|<span data-ttu-id="c91d8-316">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="c91d8-316">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="c91d8-317">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c91d8-317">screenCaptureBlocked</span></span>|<span data-ttu-id="c91d8-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-318">Boolean</span></span>|<span data-ttu-id="c91d8-319">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="c91d8-319">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="c91d8-320">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c91d8-320">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="c91d8-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-321">Boolean</span></span>|<span data-ttu-id="c91d8-322">指示是否允许 Classroom 应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="c91d8-322">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="c91d8-323">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="c91d8-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c91d8-324">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c91d8-324">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="c91d8-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-325">Boolean</span></span>|<span data-ttu-id="c91d8-326">指示是否自动授予课堂应用上托管课程的教师查看学生屏幕的权限，而不提示。</span><span class="sxs-lookup"><span data-stu-id="c91d8-326">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="c91d8-327">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="c91d8-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c91d8-328">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="c91d8-328">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="c91d8-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-329">Boolean</span></span>|<span data-ttu-id="c91d8-330">指示是否自动授予对教师请求的权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="c91d8-330">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="c91d8-331">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="c91d8-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c91d8-332">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="c91d8-332">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="c91d8-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-333">Boolean</span></span>|<span data-ttu-id="c91d8-334">指示在尝试离开课程时，是否要求通过 Classroom 在非托管课程注册的学生向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="c91d8-334">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="c91d8-335">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="c91d8-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c91d8-336">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="c91d8-336">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="c91d8-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-337">Boolean</span></span>|<span data-ttu-id="c91d8-338">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="c91d8-338">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="c91d8-339">需要通过 Apple School Manager 或 Apple Business Manager 注册 MDM。</span><span class="sxs-lookup"><span data-stu-id="c91d8-339">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c91d8-340">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="c91d8-340">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="c91d8-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="c91d8-341">Boolean</span></span>|<span data-ttu-id="c91d8-342">指示是否阻止用户在 MacOS 10.15 或更高版本上其他 iOS 或 MacOS (MacOS 设备上启动的工作) 。</span><span class="sxs-lookup"><span data-stu-id="c91d8-342">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="c91d8-343">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="c91d8-343">privacyAccessControls</span></span>|<span data-ttu-id="c91d8-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c91d8-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="c91d8-345">隐私首选项策略控件的列表。</span><span class="sxs-lookup"><span data-stu-id="c91d8-345">List of privacy preference policy controls.</span></span> <span data-ttu-id="c91d8-346">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c91d8-346">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c91d8-347">响应</span><span class="sxs-lookup"><span data-stu-id="c91d8-347">Response</span></span>
<span data-ttu-id="c91d8-348">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c91d8-348">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c91d8-349">示例</span><span class="sxs-lookup"><span data-stu-id="c91d8-349">Example</span></span>

### <a name="request"></a><span data-ttu-id="c91d8-350">请求</span><span class="sxs-lookup"><span data-stu-id="c91d8-350">Request</span></span>
<span data-ttu-id="c91d8-351">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c91d8-351">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c91d8-352">响应</span><span class="sxs-lookup"><span data-stu-id="c91d8-352">Response</span></span>
<span data-ttu-id="c91d8-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c91d8-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




